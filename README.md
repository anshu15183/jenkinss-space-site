# Free Claude Code — Project Website

The source for the Free Claude Code project landing page published at **https://project.jenkinss.space** using GitHub Pages.

This repository contains the website only. It does **not** contain the Free Claude Code application source code. For the application, installation instructions, supported integrations, and current project status, visit the upstream repository:

- **Application repository:** https://github.com/Alishahryar1/free-claude-code
- **Live website:** https://project.jenkinss.space
- **Contact:** contact@jenkinss.space

> Free Claude Code is an independent open-source project and is not affiliated with, endorsed by, or sponsored by Anthropic. Claude and Claude Code are trademarks of Anthropic.

## Website features

- Responsive landing page for desktop, tablet, and mobile.
- Project overview and feature highlights.
- Quick-start section linking to the upstream installation instructions.
- Navigation to documentation and the application repository.
- Contact link using `contact@jenkinss.space`.
- Static HTML, CSS, and JavaScript; no backend or build step is required.
- Designed for deployment on GitHub Pages with a custom domain.

## Technology

- HTML5
- CSS3
- Vanilla JavaScript
- GitHub Pages

## Run locally

### Option 1: Clone and open the page

```bash
git clone https://github.com/anshu15183/jenkinss-space-site.git
cd jenkinss-space-site
```

Open `index.html` in your browser.

### Option 2: Use a local HTTP server

From the repository directory, run:

```bash
python3 -m http.server 8000
```

Then open http://localhost:8000.

If your browser blocks any functionality when opening the file directly, use the local HTTP server option.

## Deploy with GitHub Pages

1. Push the website files (`index.html`, `styles.css`, `script.js`, and any assets) to the `main` branch.
2. In GitHub, open **Settings → Pages**.
3. Set the source to **Deploy from a branch**.
4. Select branch `main` and folder `/(root)`, then save.
5. In the Pages custom-domain field, enter `project.jenkinss.space`.
6. In Cloudflare DNS, create a **DNS-only CNAME** record:
   - **Name:** `project`
   - **Target:** `anshu15183.github.io`
7. Wait for DNS and GitHub Pages certificate provisioning to complete. Enable **Enforce HTTPS** in Settings → Pages once GitHub makes it available.

DNS and certificate changes can take time to propagate. Do not publish private keys, API tokens, or other secrets in this static website repository.

## Updating the site

Edit the relevant files and commit your changes:

- `index.html` — page structure and content
- `styles.css` — layout, responsive behavior, and visual styling
- `script.js` — client-side interactions
- `favicon.svg` — browser icon, if present

Keep feature claims, supported-provider counts, model availability, and installation commands consistent with the upstream repository. Provider free tiers and limits can change, so avoid promising that a particular model or quota will always be free.

## Application features

The upstream Free Claude Code project describes capabilities including:

- Routing coding-agent requests through configurable hosted and local model providers.
- Supporting multiple coding-agent clients through a shared configuration and model catalog.
- Configurable model selection and fallback behavior.
- Streaming responses and tool-use support where supported by the configured provider and client.
- Optional integrations such as messaging and voice workflows, depending on the current release and configuration.
- A local administration interface for configuring supported settings.

The upstream repository is the source of truth for the current supported providers, clients, setup requirements, and feature availability. Review its README before relying on any specific feature.

## Install the application

This website is informational; it does not install or run the application. Follow the official upstream instructions:

**https://github.com/Alishahryar1/free-claude-code#quick-start**

The upstream README currently documents these installer commands. Review the installer scripts and upstream README before running them.

### macOS / Linux

```bash
curl -fsSL "https://raw.githubusercontent.com/Alishahryar1/free-claude-code/main/scripts/install.sh" | sh
```

After installation, follow the upstream README to start the app, configure a provider, and launch your chosen coding agent. On Linux, the documented server command is:

```bash
fcc-server
```

### Windows PowerShell

```powershell
& ([scriptblock]::Create((irm "https://raw.githubusercontent.com/Alishahryar1/free-claude-code/main/scripts/install.ps1")))
```

Follow the upstream README for platform-specific startup and configuration steps.

## Contributing

Contributions to the website are welcome. Before submitting a pull request:

1. Keep the page responsive and accessible.
2. Test it in a modern desktop and mobile browser.
3. Verify all links and contact details.
4. Ensure descriptions match the upstream project.
5. Do not commit credentials, tokens, or private information.

Open an issue or pull request in this website repository for website-specific changes. Report application bugs and request application features in the [upstream repository](https://github.com/Alishahryar1/free-claude-code).

## License

The website code in this repository is licensed under the MIT License; see [`LICENSE`](LICENSE).

This license applies to the website files in this repository only. The Free Claude Code application has its own license and terms in the [upstream repository](https://github.com/Alishahryar1/free-claude-code). Do not treat this website license as a license for the application, its name, or third-party trademarks.
