# Grounded Phoenix LLC — Static Website

This is a lightweight static website starter for **Grounded Phoenix LLC**.

## Quick start (local)
Open `index.html` in a browser, or run a simple local server:

- Python 3:
  - `python -m http.server 8000`
  - Then open http://localhost:8000

## Deploy options
- **Netlify**: drag-and-drop the folder or connect a Git repo.
- **GitHub Pages**: push to a repo and enable Pages.
- **Any host**: upload the folder contents.

## Customize
Search for:
- `hello@groundedphoenixllc.com` (email)
- `(your phone)` (phone)
- `groundedphoenixllc.com` (domain/canonical)

If you want the contact form to submit without opening an email client, add a form service (e.g., Netlify Forms) or a small backend.

## Deploy to GitHub Pages

### Option A (recommended): Deploy from the `main` branch using `/docs`
1. Create a new GitHub repository (e.g., `grounded-phoenix-website`).
2. In the repo root, create a folder named `docs/`.
3. Copy **all website files** (everything in this folder) into `docs/` (keep the same structure).
4. Commit and push to GitHub.
5. In GitHub: **Settings → Pages**
   - **Source:** Deploy from a branch
   - **Branch:** `main`
   - **Folder:** `/docs`
6. Wait for GitHub to publish. Your site will be available at:
   - `https://<your-username>.github.io/<repo-name>/`

### Option B: Deploy from the `main` branch root
1. Put the website files in the repo root.
2. GitHub: **Settings → Pages**
   - **Branch:** `main`
   - **Folder:** `/ (root)`

### Custom domain (optional)
1. Buy/own a domain.
2. GitHub: **Settings → Pages → Custom domain** (enter your domain)
3. Create DNS records at your domain registrar:
   - For an apex domain (e.g., `groundedphoenixllc.com`): add `A` records pointing to GitHub Pages IPs.
   - For a subdomain (e.g., `www.groundedphoenixllc.com`): add a `CNAME` to `<your-username>.github.io`.
4. If you use a custom domain, add a `CNAME` file in the publishing folder containing the domain.

### Notes
- This site includes a `.nojekyll` file so GitHub Pages will serve all folders as-is.
- The contact form uses `mailto:` (it opens the visitor’s email client). If you want a real form inbox, use a form backend (e.g., Formspree) and I can wire it up.
