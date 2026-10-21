# FA design system

## Canonical FA sunmark

Confirmed by Finn Astle on 22 October 2026. Use these supplied SVGs whenever implementing the FA sunmark across websites, tools, favicons and other brand applications.

| File | Artwork | Use |
| --- | --- | --- |
| [fa-sunmark-dark.svg](assets/fa-sunmark-dark.svg) | Black mark, transparent background | Light backgrounds |
| [fa-sunmark-light.svg](assets/fa-sunmark-light.svg) | White mark, transparent background | Dark backgrounds |

“Dark” and “light” describe the mark colour, not the page theme.

These are the original supplied vectors, preserved byte-for-byte. Both have a 458 × 319 viewBox. Preserve the aspect ratio, irregular edges, FA lettering and sun geometry. Do not redraw, substitute a font, generate an approximation, stretch, crop or apply colour filters. Choose the supplied variant that contrasts with its actual background.

For production, copy the chosen SVGs into the application's own static assets. Reference them with an image element and proportional sizing (`height: auto` or `object-fit: contain`). Use meaningful alternative text when the mark conveys identity; use empty alt text when decorative.

For favicons, derive any required square canvas or PNG/ICO sizes from these originals, fitting the entire mark inside the canvas with transparent padding. Do not distort the artwork to fill a square. Test at 16 and 32 pixels and use the black version for light browser themes, white for dark themes.

Original filenames:
- FA Sunmark Vector (dark).svg
- FA Sunmark Vector (light).svg

SHA-256:
- Dark: `f370477fea88f421ea58445779e70903672581082a012205ea148df745b11278`
- Light: `6eb3d8b95ff3239e1b7f11ec9b9f847fa4a1cb39b694086f10ad82b1ed8ae233`

The existing `index.html` is the earlier brand reference. If its sunmark examples differ, the supplied SVGs above take precedence. Publishing these assets does not migrate existing applications automatically; apply them when implementing or updating each application.

Public availability does not grant ownership of Finn Astle's brand identity.
