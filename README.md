# LiveKit landscape

A map of LiveKit drawn from GitHub issues. Each simulation has its own entry link. Opening that link starts on that behavior.

- [Airplane mode](https://emms21.github.io/livekit-landscape/#airplane-mode) (#4477) — the websocket does not start when they expect it to, after airplane mode.
- [Delete, then the same name](https://emms21.github.io/livekit-landscape/#delete-same-name) (#4726) — they delete a room, create that name again, people join, then everyone is kicked.

Ticket numbers work too: `#4477`, `#4726`. Or open `index.html` in a browser.

## Analytics

[Umami](https://cloud.umami.is) records visits on GitHub Pages. Local `localhost` is skipped.

Custom events: `place` (where you are), `ticket` (issue opened), `lab` (simulation run), `engaged` (stayed 20s or visited 3 places).

In Umami, the website domain must be `emms21.github.io` (hostname only, no path).
