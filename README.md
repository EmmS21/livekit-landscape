# LiveKit landscape

A map of LiveKit drawn from GitHub issues. Open [the site](https://emms21.github.io/livekit-landscape/) or `index.html` in a browser.

## Analytics

[Umami](https://cloud.umami.is) is in the page but **off** until you paste a website id into `UMAMI_WEBSITE_ID` near the top of the script in `index.html`.

Until then the tracker script never loads — including on this GitHub Pages host. Local `localhost` is also skipped, so opening the file on your machine will not count as a visit.

After you add an id:

1. In Umami, allow the domain `emms21.github.io`
2. Push the change. Page views start. Custom events: `place` (where you are), `ticket` (issue opened), `lab` (airplane-mode lab), `engaged` (stayed 20s or visited 3 places)

The website id is public. It is not a secret; it only names which Umami site the events belong to.
