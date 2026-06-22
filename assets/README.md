# Figure assets

Static images (architecture diagram, attention maps, etc.) go here.
Set them on a slot exactly like videos — the page auto-detects image
extensions (`.png/.jpg/.webp/.gif/.svg`) and renders an `<img>`:

```html
<div class="slot" data-src="assets/architecture.png"></div>
```

Suggested exports from the paper's `main_figure/`:

| file                    | source PDF                          |
|-------------------------|-------------------------------------|
| `assets/architecture.png` | `main_figure/Model_architecture_4.pdf` |
| `assets/teaser.png`       | `main_figure/teaser.pdf`               |
| `assets/motivation.png`   | `main_figure/motivation.pdf`           |

Convert with e.g. `pdftoppm -png -r 200 input.pdf out` or ImageMagick `convert`.
