# Brand asset implementation

This repository holds canonical assets and nothing else. The design system —
palette, type, layout, image language, motion — is published at
**<https://finnastle.com/tools/design-system>** and generated from the
website's own stylesheet and asset directory. Read it there before implementing
anything. Do not reconstruct those rules from memory or from an older document.

## The mark

Use `assets/fa-sunmark-dark.svg` (black artwork, for light backgrounds) and
`assets/fa-sunmark-light.svg` (white artwork, for dark backgrounds) as the
canonical FA sunmark. Read `README.md` for usage and favicon guidance.

Preserve the supplied SVGs exactly. Do not recreate the mark using text, CSS,
generated artwork or alternate paths. Do not redraw, trace, regenerate,
stretch, crop or apply colour filters to it. Copy the originals into consuming
applications and preserve their aspect ratio. Choose the variant that contrasts
with the actual background rather than recolouring one.

Verify SHA-256 against the values in `README.md` before trusting any copy.

## If you are looking for index.html

It was deleted on 25 October 2026. It was a 505KB v2 brand reference that
existed in two repositories, was maintained by hand in both, and had drifted
from the site it described. The published page linked above replaced it and is
generated from the running code.
