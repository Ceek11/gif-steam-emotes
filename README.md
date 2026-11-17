# gif-steam-emotes

Assets for **FaFa_EmotesMenu** (FaFaDev / Tebex) — **one resource only**.

## What is in this repo

| Path | Role |
|------|------|
| `stream/` | Props & custom emotes. Copy **into** `FaFa_EmotesMenu/stream/`. |
| `previews/` | GIF/PNG emote previews. Served via CDN (jsDelivr) — **no need to download**. |

## Install (buyers)

1. Install `FaFa_EmotesMenu` from Tebex / Keymaster.
2. If your zip has no `stream/` folder: download this repo → copy the `stream/` folder **inside** `FaFa_EmotesMenu/` (so you get `FaFa_EmotesMenu/stream/...`).
3. `server.cfg`:

```cfg
ensure FaFa_EmotesMenu
```

4. GIF previews load automatically from:

`https://cdn.jsdelivr.net/gh/Ceek11/gif-steam-emotes@main/previews/...`

(`config.json` → `previewCdn.enabled = true`)

## Dev notes

- Keep `previews/` and `stream/` out of the Tebex escrow zip so it stays light.
- After updating GIFs, refresh jsDelivr if needed (commit SHA in `previewCdn.baseUrl`).
