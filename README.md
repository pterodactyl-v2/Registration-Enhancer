<div align="center">

# Registration Enhancer

### A more flexible registration experience for Pterodactyl Panel 2.0

Customizable registration pages, responsive layouts, CAPTCHA integrations, and a streamlined sign-up experience.

[Features](#features) · [Installation](#installation) · [Support](#support) · [Contributing](CONTRIBUTING.md)

![Pterodactyl](https://img.shields.io/badge/Pterodactyl-Panel%202.0-10539f?style=flat-square)
![Status](https://img.shields.io/badge/status-in%20development-orange?style=flat-square)

</div>

---

> **Project status:** Repository preparation / active development. Installation instructions and release downloads will be published when the first verified release is available. Do not treat unreleased source as a production-ready package.

## Overview

Registration Enhancer is an extension project for Pterodactyl Panel 2.0 focused on making account registration easier to customize while keeping the experience responsive and consistent with the panel.

The goal is to provide a modern registration experience without requiring panel owners to maintain a collection of manual theme edits.

## Features

The development scope includes:

- **Dedicated registration page** — customize the public registration experience.
- **Registration popup** — provide an alternate sign-up flow where enabled.
- **Responsive layout** — adapt forms and controls for desktop and mobile screens.
- **CAPTCHA integrations** — support work for Cloudflare Turnstile and invisible reCAPTCHA v2.
- **Theme controls** — customize supported registration-page styling from extension settings.
- **Logo controls** — control supported registration logo visibility.
- **Login-page entry point** — provide a registration route from the panel login screen.
- **Release-based updates** — planned GitHub release checks and update notifications.

Features may change during development. Only features documented for a tagged release should be considered available in that release.

## Compatibility

- **Target:** Pterodactyl Panel 2.0 extension system.
- **PHP / panel requirements:** Follow the requirements listed for the specific extension release and your installed panel build.
- **CAPTCHA providers:** Require valid provider configuration and matching site/secret keys where applicable.

Panel 2.0 is evolving, so check release notes before upgrading a production panel or installing a new extension version.

## Installation

Installation instructions will be added alongside the first verified `.pteroext` release.

1. Check the [Releases](https://github.com/YOUR_GITHUB_USERNAME/Registration-Enhancer/releases) page for a published stable release.
2. Read its release notes and compatibility information.
3. Back up your panel and extension settings before installing or upgrading.
4. Follow the instructions documented for that exact release.

**Do not install packages from unverified third-party mirrors.** Prefer release assets published in this repository.

## Configuration

Settings and screenshots will be documented as the public release is prepared. Available controls can vary by extension version.

A visual CAPTCHA widget alone does not guarantee server-side verification is configured correctly.

## Updates

The intended update experience is to check the latest stable GitHub release, notify panel administrators when a newer version is available, and link to release notes and the official package asset.

An automatic installer is **not promised**. It will only be documented if a safe, compatible installation flow is implemented and tested.

## Support

- **Bug reports:** use the [Bug Report](https://github.com/YOUR_GITHUB_USERNAME/Registration-Enhancer/issues/new?template=bug_report.yml) form.
- **Feature requests:** use the [Feature Request](https://github.com/YOUR_GITHUB_USERNAME/Registration-Enhancer/issues/new?template=feature_request.yml) form.
- **Security issues:** follow [SECURITY.md](SECURITY.md); do not post exploitable details in a public issue.
- **Questions:** search existing issues first and include your panel version, extension version, and relevant sanitized logs.

Remove passwords, API keys, CAPTCHA secrets, session cookies, and private user data from logs and screenshots.

## Contributing

Contributions, clear bug reports, and focused suggestions are welcome. Read [CONTRIBUTING.md](CONTRIBUTING.md) before opening a pull request.

## License

A license will be added before the first public source release. Until a license is present, do not assume that the code is available for unrestricted reuse, modification, or redistribution.

## Acknowledgements

- [Pterodactyl Panel](https://github.com/pterodactyl/panel) — the panel this extension is built for.
- [Pterodactyl SSO Extension](https://github.com/pterodactyl/SSO-Extension) — an example of a public Pterodactyl 2.0 extension repository.

---

<div align="center">Made for panel owners who want a better registration experience.</div>
