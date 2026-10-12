# El Plan

A free, non-commercial fan companion for Formula 1 race weekends.

> **Status:** early development. Nothing is deployed yet.

## What it does

- **Race-event memes** – detects race events from public timing data (safety cars, retirements, pit stops, penalties, race finish) and shows fans a relevant meme in the app or as an opt-in notification.
- **Strategy game** – players call pit stops and tyre choices for a driver during a race (or a replay of a past race). After the race, a lap-time simulation estimates whether their strategy would have beaten the team's real one.

## Planned stack

- Python (FastAPI) backend and worker, using [FastF1](https://github.com/theOehrly/Fast-F1) and the [jolpica-f1](https://github.com/jolpica/jolpica-f1) API
- Next.js progressive web app with Web Push notifications
- Postgres

## Reddit data use

El Plan is applying for read-only, non-commercial access to the Reddit Data API to surface posts from r/formuladank. If access is granted, the app will:

- show every post with attribution and a link back to the original post, preferably using official Reddit embeds
- not re-host or re-upload Reddit media
- store only post IDs, links and minimal metadata
- delete removed or deleted content within 48 hours, and re-check a post's status before showing it or sending a notification
- filter out NSFW posts
- never sell, license or share Reddit data, and never use it to train AI models
- stay free: no ads, subscriptions or paid features

## Disclaimer

This website is unofficial and is not associated in any way with the Formula 1 companies. F1, FORMULA ONE, FORMULA 1, FIA FORMULA ONE WORLD CHAMPIONSHIP, GRAND PRIX and related marks are trade marks of Formula One Licensing B.V.
