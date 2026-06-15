# pacer-publish

Public https host for the **TDL race-day pacer** PWA, so mobile Geolocation works
(a `file://` page is not a secure context on Android, so GPS is denied there).

This repo contains a single generated artifact, `index.html` — the self-contained
offline pacer. It is **built from the private `pace-planning` repo** (the model,
GPX, and Strava-calibrated code live there and stay private); only the built PWA
is published here.

Live: https://l-gonz.github.io/pacer-publish/

Do not edit `index.html` by hand — regenerate it with `python3 -m web.build_pacer`
in the private repo and push from `pacer-publish/`.
