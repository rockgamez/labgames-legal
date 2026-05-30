# labgames-legal

Static legal pages hosted on GitHub Pages — used as the Privacy Policy and Terms of Service
URLs for the LabGames automated pipeline (TikTok Content Posting API + Meta Graph API
applications).

## Files

- `index.html` — landing page linking to both documents
- `privacy.html` — Privacy Policy
- `terms.html` — Terms of Service

## Deploy (GitHub Pages, do this once)

1. Create a **public** GitHub repo named `labgames-legal` (or any name — but URL changes).
2. Push these files:
   ```bash
   cd C:\Users\TIfas\labgames-legal
   git init
   git add .
   git commit -m "Initial legal pages"
   git branch -M main
   git remote add origin https://github.com/<your-user>/labgames-legal.git
   git push -u origin main
   ```
3. On GitHub: **Settings → Pages → Build and deployment**:
   - Source: **Deploy from a branch**
   - Branch: **main** / Folder: **/ (root)** → Save
4. Wait ~30s. Your URLs will be:
   - `https://<your-user>.github.io/labgames-legal/` (landing)
   - `https://<your-user>.github.io/labgames-legal/privacy.html`
   - `https://<your-user>.github.io/labgames-legal/terms.html`

Use the `privacy.html` and `terms.html` URLs in the TikTok Developer Portal app submission.

## Updating

After editing locally:
```bash
git add . && git commit -m "Update legal text" && git push
```

Changes appear at the public URL in ~30 seconds.
