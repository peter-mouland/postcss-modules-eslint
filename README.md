# postcss-modules-eslint

> minimal test case for https://github.com/bmatcuk/eslint-plugin-postcss-modules/issues/3

Run `yarn lint`

errors: 

```
/postcss-modules-eslint/scopes/b/index.js
  1:1   warning  Class classNameA is exported but unused       postcss-modules/no-unused-class
  3:13  error    classNameB does not exist in ./file-name.css  postcss-modules/no-undef-class

````

## Problem

 * `1:1` warning: `scopes/b/index.js` does not actually have a `classNameA`
 * `3:13` error:  `classNameB` does actually exist
