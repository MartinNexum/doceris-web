# doceris-web

Static marketing/landing + privacy-policy site for the Doceris digital-signature product. Plain HTML (Spanish), no build system, no dependencies, no backend.

## Cursor Cloud specific instructions

- This repo is just static HTML files (`index.html`, `privacy.html`). There is nothing to install or build; there is no `package.json`, lockfile, or test suite.
- To run locally, serve the directory with any static file server, then open the pages. Per `README.md`: `npx http-server -p 8000`, then visit `http://localhost:8000/index.html`. `python3 -m http.server 8000` works equally well.
- There is no backend/API/database; "end-to-end" testing means loading `index.html` and `privacy.html` in a browser. Pages also open directly via `file://` since there is no server-side logic.
- `npx http-server` is a long-running process — start it in a background/tmux session, not as a blocking foreground command.
