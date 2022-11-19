1. npm install carbon-components
2. npm install carbon-components
3. svelte npx svelte-add@latest scss
4. yarn install

5. copy to app.scss

```$css--font-face: true;

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
```

6. npm i -D carbon-preprocess-svelte

7. add import { optimizeImports } from "carbon-preprocess-svelte"; to svelte.config.js

8. add optimizeImports() to preprocessor array in svelte.config.js

9. import component scss as needed in script tag: (e.g., import 'carbon-components/scss/components/button/button';)

    _see all component scss paths at https://github.com/carbon-design-system/carbon/tree/main/packages/carbon-components/scss/components_

10. check that it works in chrome dev tools by opening up network tab and looking at bundle size (filter up top using .scss)
