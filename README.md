# Free Claude Code landing page

A responsive, static landing page for the public `Alishahryar1/free-claude-code` repository. It uses plain HTML, CSS, and JavaScript and is suitable for GitHub Pages.

## Files

- `index.html` — page structure and content
- `styles.css` — responsive visual styling
- `script.js` — mobile navigation, copy buttons, and footer year
- `favicon.svg` — simple site icon

## Before publishing

1. Confirm that `https://github.com/Alishahryar1/free-claude-code` is the correct repository you want to represent.
2. Review the copy against the current README and remove any feature that is no longer supported.
3. The page explicitly states that this is an independent project and is not affiliated with or endorsed by Anthropic.
4. The contact address shown is `contact@jenkinss.space`. Cloudflare Email Routing only forwards incoming mail; it does not by itself enable sending as that address.
5. No API keys, credentials, or backend secrets belong in this static website.

## Preview locally

Open `index.html` in a browser. For a local HTTP preview, run from this directory:

```bash
python3 -m http.server 8000
```

Then visit `http://localhost:8000`.

## Deploy to GitHub Pages

1. Create a repository such as `jenkinss-space-site` under your GitHub account.
2. Upload the four site files and this README to the repository root.
3. In the repository, open **Settings → Pages**.
4. Under **Build and deployment**, choose **Deploy from a branch**.
5. Select the `main` branch and `/ (root)`, then save.
6. In the Pages custom-domain field, enter `jenkinss.space` (or a subdomain such as `project.jenkinss.space`) and save.
7. Configure the DNS records in Cloudflare using the exact values shown in GitHub's Pages instructions. For an apex domain, GitHub Pages commonly uses four A records; confirm the current official documentation before editing DNS.
8. Once GitHub Pages verifies the domain, enable **Enforce HTTPS** when that option becomes available.

Official guide: https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site

## Updating the site

Edit the files, commit the changes, and push to the branch selected in Settings → Pages. GitHub Pages will rebuild the static site.

## Notes

- This site is static and does not run the Free Claude Code application or provide a hosted model/API.
- The project's own README is the source of truth for install steps, providers, supported clients, and current features.
- Provider availability, pricing, quotas, and terms may change.
