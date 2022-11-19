npm install carbon-components
npm install carbon-components svelte
npx svelte-add@latest scss
yarn install

copy to app.scss
$css--font-face: true;
$css--helpers: true;
$css--body: true;
$css--use-layer: true;
$css--reset: true;
$css--default-type: true;
$css--plex: true;

@import 'carbon-components/scss/globals/scss/\_css--reset.scss';
@import 'carbon-components/scss/globals/scss/\_css--font-face.scss';
@import 'carbon-components/scss/globals/scss/\_css--helpers.scss';
@import 'carbon-components/scss/globals/scss/\_css--body.scss';

npm i -D carbon-preprocess-svelte
add import { optimizeImports } from "carbon-preprocess-svelte"; to svelte.config.js
add optimizeImports() to preprocessor array

import component scss as needed in script tag:
import 'carbon-components/scss/components/button/button';

see all component scss paths at
https://github.com/carbon-design-system/carbon/tree/main/packages/carbon-components/scss/components

check that it works in chrome dev tools by opening up network tab and looking at bundle size (filter up top using .scss)
