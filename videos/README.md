# Video assets

Drop `.mp4` files here, then open `index.html` and set the matching
`data-src` on each `<div class="slot">`. The `data-path` hint already shown
in each empty slot is the suggested location:

```
videos/
├── teaser.mp4
├── attention/
│   ├── baseline.mp4
│   └── ours.mp4
├── davis/
│   ├── scene1/  { reference, ours, pcd_ref, pcd_tgt }.mp4
│   └── scene2/  { ... }
├── iphone/
│   ├── scene1/  { reference, ours, gt }.mp4
│   └── scene2/  { ... }
└── compare/
    ├── scene1/  { reference, ours, recammaster, redirector,
    │              trajectorycrafter, gen3c, cognvs }.mp4
    └── scene2/  { ... }
```

To fill a slot, change e.g.

```html
<div class="slot" data-src="" data-path="videos/teaser.mp4"></div>
```
to
```html
<div class="slot" data-src="videos/teaser.mp4"></div>
```

Recommended: H.264 `.mp4`, ≤ 1280px wide, muted (they autoplay-loop on hover/click).
