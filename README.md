# Ghost Heist heists

`feed.json` is downloaded by the Ghost Heist app when it opens. It lets new or fixed heists reach players without an app update.

- Append new heists to `levels`. Never reorder or remove them: stars are saved by position.
- Give every change a new `version`, e.g. `2026-11-05-1`. The app only re-applies the file when the version changes.
- Check it first with `npm run feed:check -- path/to/feed.json` in the game repo.

Phones pick up a change the next time the game opens (GitHub may serve the old copy for up to 5 minutes).
