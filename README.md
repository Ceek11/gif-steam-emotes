# gif-steam-emotes

Assets for **FaFa_EmotesMenu** (FaFaDev / Tebex).

## What is in this repo

| Path | Role |
|------|------|
| `FaFa_EmotesMenu_Stream/` | FiveM resource — props & custom emotes (`stream/`). **Drag into `resources/`**. |
| `previews/` | GIF/PNG emote previews. Served via CDN (jsDelivr) — **no need to download** for players. |

## Install (buyers)

1. Download this repo (Code → Download ZIP) or clone it.
2. Copy the folder `FaFa_EmotesMenu_Stream` into your server `resources/` (next to `FaFa_EmotesMenu`).
3. In `server.cfg`:

```cfg
ensure FaFa_EmotesMenu_Stream
ensure FaFa_EmotesMenu
```

4. GIF previews load automatically from:

`https://cdn.jsdelivr.net/gh/Ceek11/gif-steam-emotes@main/previews/...`

(`config.json` → `previewCdn.enabled = true`)

## Dev notes

- Do not put `previews/` or `stream/` back into the Tebex escrow zip — keep that package light.
- After updating GIFs, bump / refresh jsDelivr cache if needed: append `@main` or a commit SHA in `previewCdn.baseUrl`.
