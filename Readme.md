# Foundation 6 Webpack Compiler

> Compiles SCSS particles from Foundation, for those who need css file, but don't want to use Gulp/Grunt


Make sure you have LTS Node.js and Npm installed</br>

1. Import everything you need into `foundation.scss`</br>
2. Edit "includes" to add/remove particles you need:
```scss
...
// Global styles
@include foundation-global-styles;
@include foundation-forms;
@include foundation-typography;

// Grids (choose one)
@include foundation-xy-grid-classes;
...
```
3. Edit settings you need in `_settings.scss`
```scss
$global-font-size: 100%;
$global-width: rem-calc(1200);
$global-lineheight: 1.5;
$foundation-palette: (
  primary: #1779ba,
  secondary: #767676,
  success: #3adb76,
  warning: #ffae00,
  alert: #cc4b37,
);
$light-gray: #e6e6e6;
$medium-gray: #cacaca;
$dark-gray: #8a8a8a;
$black: #0a0a0a;
...
```
4. Install dependencies
> `npm install`
5. Bundle your package
> `npm start`

Get your buit file in `/dist/foundation_weberous.min.css`