# siyf-web-cdn

Static JSON and media for the [Syif! Web](https://github.com/Sports-in-your-face) app. Served via [jsDelivr](https://www.jsdelivr.com/?docs=gh).

## CDN URL

```
https://cdn.jsdelivr.net/gh/Sports-in-your-face/siyf-web-cdn@main
```

Used by `siyf-engine` in the web app for team logos, registry JSON, special-event catalogs, and favicons.

## Layout

```
meta/          manifest, aliases, special-events, soccer-leagues
teams/         nba.json, nfl.json, epl.json, mlb.json, nhl.json
media/logos/   per-sport team PNGs
favicon/       site favicon
stats/         optional cached player history JSON
```

## Publish

```bash
git add -A
git commit -m "Update CDN assets"
git push
```

jsDelivr picks up changes from `main` automatically. Purge a path if needed:

```
https://purge.jsdelivr.net/gh/Sports-in-your-face/siyf-web-cdn@main/{path}
```
