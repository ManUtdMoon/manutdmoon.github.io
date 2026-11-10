# Dongjie Yu — personal homepage

The homepage is plain HTML and CSS. It requires no build step or external fonts/scripts. Lato is bundled locally in `fonts/`, with its SIL Open Font License.

## Local preview

Open `index.html` using your VS Code preview extension. No Python server is needed; the page also works when opened directly in a browser.

## Editing

- Edit `index.html` for the biography, contact links, news, publications, services, and teaching.
- Services and Teaching were transcribed from page 2 of `pdf/CV_Dongjie-Yu.pdf`. The CV does not specify teaching semesters; none have been inferred.
- Edit `style.css` for layout, typography, and responsive breakpoints.
- The full publication list links directly to Google Scholar.
- Images live in `img/`; the existing CV remains at `pdf/CV_Dongjie-Yu.pdf`.
- The old jemdoc sources, configuration, stylesheet, and extra pages have been removed. `index.html` is the source of truth.
- Update the footer's visible date and its `datetime` attribute, plus the homepage's `lastmod` in `sitemap.xml`, when page content changes. These are editorial dates, not the visitor's current date.
- `sitemap.xml` lists the canonical homepage and CV, with no removed pages or duplicate homepage URLs.

## Analytics and search verification

No Google Analytics script is enabled. `google-site-verification` and the Google verification HTML file are Search Console ownership checks, not visitor tracking; keep them intact.

If analytics is added later:

- Use the owner's GA4 web-stream measurement ID (`G-…`), never an ID from a reference template.
- Load analytics only on the production hostname (`manutdmoon.github.io`) over HTTPS. Do not load it on localhost, file previews, or temporary preview hosts.
- Install it once, either directly or through Tag Manager. Avoid sending a second manual `page_view` on top of GA4's automatic pageview.
- Decide the consent/privacy behavior before enabling collection. Consent mode itself does not provide a consent banner.
- Verify the deployed setup with Tag Assistant and GA4 Realtime/DebugView. This local-only redesign does not enable or validate analytics.

References: [GA4 measurement IDs](https://support.google.com/analytics/answer/12270356), [pageviews](https://developers.google.com/analytics/devguides/collection/ga4/views), [consent mode](https://developers.google.com/tag-platform/security/concepts/consent-mode).

## Research image sources

The current teaser images were supplied by the site owner on November 10, 2026, replacing the initial preview figures. All six are served locally and displayed without cropping.

- ZPRL: `img/research/zprl.png`
- RL-100: `img/research/rl100.png`
- BiKC+: `img/research/bikc-plus.png`
- BiKC: `img/research/bikc.png`
- Safe Model-Based RL (DRPO): `img/research/drpo.png`
- Reachability Constrained RL (RCRL): `img/research/rcrl.png`

When replacing an image, update its `width` and `height` attributes in `index.html` to match the file's actual dimensions.

Layout inspiration: [Jon Barron](https://jonbarron.info/), [Mitsuhiko Nakamoto](https://nakamotoo.github.io/), and [Ruihai Wu](https://warshallrho.github.io/). The HTML and CSS were written for this site.

The Lato Latin font files match the normal/italic, regular/bold faces in the reference templates' stylesheets. Font source: [Google Fonts](https://fonts.google.com/specimen/Lato); license: `fonts/OFL.txt`.
