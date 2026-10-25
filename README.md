# FA design system

This repository holds the canonical brand assets and the rules for using them.
Nothing else.

**The design system itself is published at
<https://finnastle.com/tools/design-system>.** That page is generated from the
website's own stylesheet and asset directory, so its palette, type scale,
component rules and image language are read out of the running code rather than
restated. Read it there. It cannot be out of date with the site in the way a
written copy can.

## Canonical FA sunmark

Confirmed by Finn Astle on 22 October 2026. Use these supplied SVGs whenever
implementing the FA sunmark across websites, tools, favicons and other brand
applications.

| File | Artwork | Use |
| --- | --- | --- |
| [fa-sunmark-dark.svg](assets/fa-sunmark-dark.svg) | Black mark, transparent background | Light backgrounds |
| [fa-sunmark-light.svg](assets/fa-sunmark-light.svg) | White mark, transparent background | Dark backgrounds |

"Dark" and "light" describe the mark colour, not the page theme.

These are the original supplied vectors, preserved byte-for-byte. Both have a
458 × 319 viewBox. Preserve the aspect ratio, irregular edges, FA lettering and
sun geometry. Do not redraw, substitute a font, generate an approximation,
stretch, crop or apply colour filters. Choose the supplied variant that
contrasts with its actual background.

For production, copy the chosen SVGs into the application's own static assets.
Reference them with an image element and proportional sizing (`height: auto` or
`object-fit: contain`). Use meaningful alternative text when the mark conveys
identity; use empty alt text when decorative.

Original filenames:

- FA Sunmark Vector (dark).svg
- FA Sunmark Vector (light).svg

SHA-256:

- Dark: `f370477fea88f421ea58445779e70903672581082a012205ea148df745b11278`
- Light: `6eb3d8b95ff3239e1b7f11ec9b9f847fa4a1cb39b694086f10ad82b1ed8ae233`

Raw URLs for agents without local access:

- https://raw.githubusercontent.com/finnastle-lab/fa-design-system/main/assets/fa-sunmark-dark.svg
- https://raw.githubusercontent.com/finnastle-lab/fa-design-system/main/assets/fa-sunmark-light.svg

Check the hash before trusting a copy.

## Favicons

Derive them from these originals: fit the whole mark inside a square canvas
with transparent padding, and do not distort it to fill. Test at 16px and 32px.

Ship both variants and select between them with
`media="(prefers-color-scheme: ...)"` on the `rel="icon"` links: the black mark
for light browser chrome, the white mark for dark. Order the links with the
black mark last, because `media` on `rel="icon"` is honoured unevenly and a
browser that ignores it takes the final link, which should be the variant that
reads on a default light tab strip.

One exception: an Apple touch icon needs an opaque ground. iOS composites it
onto the home screen, where transparency renders black.

The website's implementation of all of the above is at
[`scripts/make-favicons.py`](https://github.com/finnastle-lab/finnastle-com/blob/main/scripts/make-favicons.py).

## What used to be here

`index.html` was a 505KB brand reference, v2, dated 30 August 2026. It was
deleted on 25 October 2026.

It existed twice, once here and once in the website repository, each maintained
by hand. The two copies had already drifted: they differed by a single em dash,
cleaned in one and left standing in the other. It also documented a palette, a
content width and a type scale the website had moved away from, and had no
image or motion section at all.

Its replacement is generated from the code it describes. See the link at the
top of this file.

Publishing these assets does not grant ownership of Finn Astle's brand
identity.
