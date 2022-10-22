# Karaka Website

Built using Hugo, Tailwind CSS and the awesome template by [ttntm](https://github.com/ttntm).

## Deployment

1. `npm install`
2. `npm run deploy`

## Local Development

**Requirements:**

1. Hugo
2. npm

**Setup:**

1. Fork, clone or download
2. `cd` into the root folder
3. run `npm install`
4. run `npm run start`
5. open a browser and go to `http://localhost:1313`

**Basic configuration:**

1. Hugo -> `./config.toml`
2. Tailwind -> `./tailwind.config.js`

> For better development experience, please have a look at `./tailwind.config.js` and either disable `purge` or comment it - otherwise you'll have a very limited selection of Tailwind classes available.

Keep in mind that `page.css` can be re-built anytime via `gulp css` - no need to make changes to the generated files in `./static/css`.

Please note that `gulp css` _does not_ include that `normalize.css` file used for the 2 regular pages (imprint, privacy).

**Change Content:**

All page content is stored in `./content`.

`./content/sections/` is where each section's content can be found.

The individual tile/card elements for the "Features" screen are stored in `./content/sections/features/`

**Change Templates/Layout:**

Page structure and templates are stored in `./layouts` and can be edited there.

Best have a look at `./layouts/_default/baseof.html` first to understand how it all comes together - the page itself is constructed from partials in `./layouts/partials` and each section has a corresponding template file stored in the folder `./layouts/partials/sections`.

`index.html` in `./layouts` simply arranges everything, i.e. sections can be re-ordered/removed/... there.

**Change images:**

Images are stored in `./static/img`; everything in there can be considered a placeholder that should eventually be replaced with your actual production images.
