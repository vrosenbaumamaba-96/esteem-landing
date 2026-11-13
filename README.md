# Esteem Academy of Beauty — Landing Page (Staging)

Static landing page built from the approved wireframe.

- `index.html` — landing page
- `thank-you.html` — form confirmation page

Both pages are set to `noindex, nofollow` for staging. Remove that meta tag from each page's `<head>` before launch.

## Put it on GitHub Pages
1. In GitHub, create a new repository (for example `esteem-landing`).
2. Choose **Add file → Upload files**, drag in `index.html`, `thank-you.html` and this README, then **Commit changes**.
3. Go to **Settings → Pages**. Under *Build and deployment*, set Source to **Deploy from a branch**, Branch to **main**, folder to **/ (root)**, then **Save**.
4. After a minute or two, the staging link appears at the top of that page: `https://<your-account>.github.io/esteem-landing/`

Note: on a private repo, GitHub Pages needs a paid GitHub plan, and the published site is still public.

## Before launch (dev)
- Connect the form to info@esteem-academy.com and Prestige CRM. The staging form only redirects to `thank-you.html`.
- Swap the dashed placeholder boxes for the real logo, photos, partner logos, Google Map embed and Instagram feed.
- Add the Privacy Policy URL (search for `privacy-policy-url-needed`).
- Add the sticky mobile bar with Call and Get Info buttons.
- Remove the `noindex` meta tag.
