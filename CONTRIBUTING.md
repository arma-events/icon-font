## Adding an icon

To add a new icon simply add the SVG in the `./svg/` subdirectory. The filename should only consist of letter, numbers and underscores.

> [!IMPORTANT]  
> SVGs must only consist of simple shapes. Neither texts, nor outlines are allowed. Sometimes it helps to split complex shapes (especially with holes) into multiple paths.

## Building the font

> [!TIP]
> If you do not have Node.js installed, you can also download the artifact that is automatically made available by GitHub Actions as soon as the repository is updated. (see [this guide](https://docs.github.com/en/actions/managing-workflow-runs/downloading-workflow-artifacts))

To build the font, `npm` and Node.js is required. Simply install all dependencies (run `npm ci`) and then run `npm run build` in the root directory of this repository.

The output directory (`./out/`) includes an `example.html`-file, which can be used to check whether all icons are rendered correctly.
