# Icon font for arma.events [![NPM](https://img.shields.io/npm/v/%40arma-events%2Ficon-font?style=flat-square)](https://npmjs.com/package/@arma-events/icon-font)

This package contains the icon font for [arma.events](https://arma.events) and related projects.

The font uses [font ligatures](https://fonts.google.com/knowledge/glossary/ligature) and is basically a subset of [Lucide Icons](https://github.com/lucide-icons/lucide) together with some icons that were created specifically for [arma.events](https://arma.events). All icons originating from Lucide have the same name as in Lucide, but `-` (minus) has been changed to `_` (underscore).

You can find a detailed breakdown of where each icon comes from in the [icon sources section](#icon-sources) at the bottom of this readme.

## Installation

```
npm i @arma-events/icon-font
```

## Usage

Simply include the css file, which includes font-face and a class:

```css
@import '@arma-events/icon-font/dist/index.css';
```

Then use it in your HTML:

```html
<span class="arma-eventicons" aria-hidden="true">crown</span>
```

> [!TIP]
> You can find a list of all icons by simply checking the [`svg`-directory](./svg/)

## Advanced Usage

This package also includes a SCSS file which allows some configuration and can be used instead of the CSS file:

```scss
// the values used here are the default values
@use '@arma-events/icon-font/dist/index.scss' as icon-font with (
  $base-path: '@arma-events/icon-font/dist',
  // set $class to '' to disable a generation of the css class selector
  $class: 'arma-eventicons',
  $font-family: 'arma.events Icon Font',
  $font-family-fallback: 'arma.events Icon Font Fallback' !default
);

// use the styles-mixin to include the relevant
// styles for icons in your own selectors:
#icon {
  @include icon-font.styles;
}
```

## Icon Sources

Most icons are from [Lucide Icons](https://github.com/lucide-icons/lucide), but there are a few exceptions:

The following icons are from [Simple Icons](https://github.com/simple-icons/simple-icons):

- `discord`
- `twitter`
- `youtube`

The following icons are custom made for arma.events:

- `condensed`
- `crown`
- `crown_off`
- `edit_2`
- `expanded`
- `grip`
- `reorder`
- `text`
- `plus_small`
- `calendar_dashed`
