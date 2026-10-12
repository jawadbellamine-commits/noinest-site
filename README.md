# NoïNest coming-soon website

Static site served at https://noinest.com (decisions D99 and D101 in the project dossier).

- `public/` is the whole website: `index.html`, `privacy.html`, `styles.css`, self-hosted fonts (SIL Open Font License), photos and icons.
- Sign-ups are posted by the page's own form to Brevo (list "Coming soon", double opt-in). The form address is the `BREVO_FORM_URL` constant in `public/index.html`.
- Hosting: Replit static deployment (`.replit`, `publicDir = "public"`). To preview locally: `python3 -m http.server 8000 --directory public`.
- No cookies and no third-party scripts except Replit's cookieless visit analytics (enabled in the Replit publishing settings, disclosed in `privacy.html`). Any new tracker or script must be added to `privacy.html` first.
