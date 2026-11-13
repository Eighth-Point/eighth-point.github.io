# site/
The public website for Eighth Point: a landing page and the privacy policy (rendered from `legal/privacy-policy.md`), plain static HTML with no build step.
Published by pushing this folder as the root of `Eighth-Point/eighth-point.github.io` (branch `main`, GitHub Pages) to https://eighth-point.github.io/; `scripts/test/site.test.mjs` keeps the policy page in step.

The landing page is the `showcase` direction (RC-375, `docs/mocks/2026-11-13-site-round/`). `assets/` holds what it loads: Archivo and its licence, the icon, and four store frames from `store/screenshots/iphone-63` scaled to 1700 px tall (`sips -Z 1700 -s format jpeg -s formatOptions 78`); re-scale them when the store frames change.

`assets/app-store-badge.svg` is Apple's black US badge, unaltered (`https://toolbox.marketingtools.apple.com/api/v2/badges/download-on-the-app-store/black/en-us`).
`assets/app-store-qr.svg` encodes `https://apps.apple.com/app/id6829878445` (29 modules, level M, made with `toqr`, the encoder Expo ships, and checked with Core Image's QR detector); remake it if the link ever changes. It shows beside the hero's badge on a desktop only.

Publish only the files that changed: a policy dated for a feature that has not shipped stays out until it ships (RC-352's `tally_opened`).
