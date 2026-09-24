# TiddlyWiki (live static build)

A public, ready-to-use copy of [TiddlyWiki](https://tiddlywiki.com) — the complete
personal wiki in a single self-contained HTML file — hosted on GitHub Pages.

**Live:** https://coattails-droid.github.io/tiddlywiki-live/

## Provenance

| Item          | Detail                                                                 |
|---------------|------------------------------------------------------------------------|
| Source repo   | [`Jermolene/TiddlyWiki5`](https://github.com/Jermolene/TiddlyWiki5)    |
| Commit SHA    | `8c599e64c093cc9254c067ae1442c09bb5fa9341`                               |
| Edition       | `empty` (the standard empty TiddlyWiki edition)                         |
| Build command | `node tiddlywiki.js mynewwiki --build index` (run from the repo root, `mynewwiki` initialized with `--init empty`) |
| Build date    | 2026-09-24                                                              |
| License       | BSD-3-Clause (copy in `LICENSE`)                                        |

This repository contains **only** the built static artifacts (`index.html`, `LICENSE`,
this README). The full development repo, build tooling, and `node_modules` are
deliberately not mirrored here — the build can be reproduced from the upstream
repo at the commit above.

## Saving changes (static-host behavior)

TiddlyWiki is normally a single HTML file that saves back to itself when hosted
on a server that allows file writes (or served from the local filesystem).
On a **static host** like GitHub Pages there is no server write-back, so edits
made in the browser cannot be saved in place. Instead, use the wiki's
**save changes** button to download the updated file, then replace `index.html`
with the downloaded copy (and push it here to persist it).

This is inherent to static hosting — not a defect of this build.

## License

BSD-3-Clause, same as upstream. See [`LICENSE`](LICENSE).
