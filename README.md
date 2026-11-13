# site/
The public website for Eighth Point: a landing page and the privacy policy (rendered from `legal/privacy-policy.md`), plain static HTML with no build step.
Published by pushing this folder as the root of `Eighth-Point/eighth-point.github.io` (branch `main`, GitHub Pages) to https://eighth-point.github.io/; `scripts/test/site.test.mjs` keeps the policy page in step.

The landing page is the `showcase` direction (RC-375, `docs/mocks/2026-11-13-site-round/`). `assets/` holds what it loads: Archivo and its licence, the icon, and four store frames from `store/screenshots/iphone-63` scaled to 1700 px tall (`sips -Z 1700 -s format jpeg -s formatOptions 78`); re-scale them when the store frames change.

Before the first publish of this page, once 1.0 is released (so the badge's link resolves): put Apple's black "Download on the App Store" badge in `assets/app-store-badge.svg` (Apple's marketing resources) and swap it into both `.badge` links as the CSS comment says.
