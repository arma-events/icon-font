# Arma Events Icon font
This repository contains the icon font for [arma.events](https://arma.events) using [font ligatures](https://fonts.google.com/knowledge/glossary/ligature).  

This font is basically a subset of [Lucide Icons](https://github.com/lucide-icons/lucide) together with some icons that were created specifically for [arma.events](https://arma.events). All icons originating from Lucide have the same name as in Lucide, but `-` (minus) has been changed to `_` (underscore). 

You can find a detailed breakdown of where each icon comes from in the [icon sources section](#icon-sources) at the bottom of this readme.

## Adding a icon

To add a new icon simply add the SVG in the `./svg/` subdirectory. The filename should only consist of letter, numbers and underscores.

> [!IMPORTANT]  
> SVGs must only consist of simple shapes. Neither texts, nor outlines are allowed. Sometimes it helps to split complex shapes (especially with holes) into multiple paths.  

## Building the font

> [!TIP]
> If you do not have Node.js installed, you can also download the artifact that is automatically made available by GitHub Actions as soon as the repository is updated. (see [this guide](https://docs.github.com/en/actions/managing-workflow-runs/downloading-workflow-artifacts))

To build the font, `npm` and Node.js is required. Simply install all dependencies (run `npm ci`) and then run `npm run build` in the root directory of this repository.

The output directory (`./out/`) includes an `example.html`-file, which can be used to check whether all icons are rendered correctly.

## Usage

To use the font, simply include the `arma-eventicons.css` from the output directory. You may have to adjust the paths to the font files. 

## Icon Sources

Most icons are from  [Lucide Icons](https://github.com/lucide-icons/lucide), but there are a few exceptions:

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



