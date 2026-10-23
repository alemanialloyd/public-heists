# Ghost Heist heists

`feed.json` is downloaded by the Ghost Heist app when it opens. It lets new or fixed heists reach players without an app update.

- Append new heists to `levels`. Never reorder or remove them: stars are saved by position.
- Give every change a new `version`, e.g. `2026-11-05-1`. The app only re-applies the file when the version changes.
- Check it first with `npm run feed:check -- path/to/feed.json` in the game repo.

Phones pick up a change the next time the game opens (GitHub may serve the old copy for up to 5 minutes).

## Website

GitHub Pages serves this repo at https://alemanialloyd.github.io/public-heists/. The privacy policy linked from the store listings is `privacy/index.html` (https://alemanialloyd.github.io/public-heists/privacy/). `.nojekyll` makes Pages serve the files as they are, so `feed.json` is untouched.
