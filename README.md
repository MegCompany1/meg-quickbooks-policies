# MEG QuickBooks Integration – policy pages

Public policy pages (End-User License Agreement and Privacy Policy) for Meg Company Inc.'s private QuickBooks Online integration. Served by GitHub Pages from the `main` branch, root directory.

This repository is public. It must contain only these pages: no credentials, tokens, `.env` files, accounting data or application code.

## Files

| File | Purpose |
|---|---|
| `index.html` | Landing page linking to both policies |
| `eula.html` | End-User License Agreement |
| `privacy.html` | Privacy Policy |
| `launch.html` | Intuit "Launch URL" |
| `connect.html` | Intuit "Connect/Reconnect URL" |
| `disconnect.html` | Intuit "Disconnect URL" |
| `style.css` | Shared styling |
| `.nojekyll` | Tells GitHub Pages to serve files as-is |

## Editing and republishing

1. Edit the HTML file(s). Plain HTML, no build step. Open a file in a browser to preview it.
2. If the policy content changes, update the "Effective" date on every page that changed (and on `index.html`).
3. Check what you are about to commit: `git status` and `git diff --staged`.
4. Commit and push to `main`:
   ```sh
   git add *.html style.css README.md
   git commit -m "Update policies"
   git push origin main
   ```
5. GitHub Pages redeploys automatically within a minute or two. Check progress under the repository's **Actions** tab, or **Settings → Pages**.

Keep the file names unchanged: Intuit's developer settings point at the `eula.html`, `privacy.html`, `launch.html`, `connect.html` and `disconnect.html` URLs. When adding files, include them in the `git add` line above.
