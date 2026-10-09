<div align="center">

# ✨ Registration Enhancer

**A modern, customizable registration experience for Pterodactyl Panel 2.0.**

[![Pterodactyl Panel 2.0](https://img.shields.io/badge/Pterodactyl-Panel%202.0-3B82F6?style=for-the-badge&logo=pterodactyl&logoColor=white)](https://github.com/pterodactyl/panel)
[![Latest Release](https://img.shields.io/github/v/release/pterodactyl-v2/Registration-Enhancer?style=for-the-badge&label=release)](https://github.com/pterodactyl-v2/Registration-Enhancer/releases)
[![Issues](https://img.shields.io/github/issues/pterodactyl-v2/Registration-Enhancer?style=flat-square)](https://github.com/pterodactyl-v2/Registration-Enhancer/issues)
[![License](https://img.shields.io/badge/license-not%20published-lightgrey?style=flat-square)](#-license)

[Features](#-features) · [Preview](#-preview) · [Installation](#-installation) · [Configuration](#-configuration) · [Troubleshooting](#-troubleshooting)

</div>

---

> [!IMPORTANT]
> **Under active preparation.** This repository's documentation is being prepared while the extension is updated. Check Releases and the compatibility notes before installing. Only features present in a published package are available.

## ✨ Features

- 🎨 **Theme controls** — customize the supported registration-page appearance.
- 📱 **Responsive registration** — layouts designed for desktop and mobile.
- 🪟 **Registration popup** — an alternate sign-up flow where enabled.
- 🛡️ **CAPTCHA options** — Cloudflare Turnstile and Google reCAPTCHA v2 (invisible), subject to the installed release.
- 🖼️ **Logo controls** — configure supported registration logo visibility.
- 🔗 **Login integration** — an entry point to the registration flow from the login page.
- 🔔 **Update notifications** — check release notes for current availability; the GitHub updater is planned.

## 🖼️ Preview

Real screenshots will be added after the updated extension has been published and verified.

<!-- Add actual screenshots to the screenshots/ directory, then uncomment:
<p align="center">
  <img src="screenshots/registration-page.png" alt="Registration page" width="48%">
  <img src="screenshots/registration-popup.png" alt="Registration popup" width="48%">
</p>
<p align="center">
  <img src="screenshots/extension-settings.png" alt="Extension settings" width="48%">
  <img src="screenshots/mobile-registration.png" alt="Mobile registration" width="48%">
</p>
-->

## 📦 Installation

**Recommended: use the panel's Extensions interface.**

1. Open [Releases](https://github.com/pterodactyl-v2/Registration-Enhancer/releases).
2. Download the `.pteroext` asset for the desired version, if a verified release is available.
3. Sign in to Pterodactyl with an administrator account.
4. Navigate to **Admin → Extensions**.
5. Upload the package and follow the installation or replacement prompts.
6. Read the release notes, configure any required settings, and test registration in a private/incognito window.

> [!CAUTION]
> Back up your panel files and database before upgrading. Confirm that the release supports your exact Panel 2.0 build. Do not install packages from unofficial mirrors.

## ⚙️ Configuration

Available settings depend on the installed release. Use the extension's settings interface and follow the release notes for the supported options.

### 🛡️ CAPTCHA

| Provider | Setup |
|---|---|
| **Cloudflare Turnstile** | Configure the matching site key and secret key from the Cloudflare dashboard. |
| **Google reCAPTCHA v2 (invisible)** | Configure the matching site key and secret key from the Google reCAPTCHA admin console. |

CAPTCHA availability depends on the published extension version. Keep secret keys private and ensure server-side verification is configured; displaying a widget alone is not sufficient protection.

## 🧹 Clear cache

If changes do not appear after installation or an upgrade, run these commands on the panel host. Change `php8.4-fpm` if your PHP-FPM service uses a different version.

```bash
cd /var/www/pterodactyl
php artisan optimize:clear
systemctl restart php8.4-fpm
systemctl restart nginx
```

Then hard-refresh the browser with **Ctrl + Shift + R**. These commands clear Laravel's optimized caches and restart services; they cannot fix an incompatible package or failed installation.

## 🧩 Compatibility

- **Target:** Pterodactyl Panel 2.0 extension system.
- Check the specific release notes for supported panel builds and requirements.
- Panel 2.0 and its extension ecosystem may evolve; test upgrades on a staging instance where possible.

## 🛠️ Troubleshooting

- **Changes not visible:** clear the panel cache, restart the relevant services, and hard-refresh the browser.
- **Installation fails:** verify package integrity and panel-version compatibility; review the panel logs.
- **CAPTCHA fails:** check the selected provider, matching keys, allowed hostnames, and server-side verification.
- **Still stuck?** [Open an issue](https://github.com/pterodactyl-v2/Registration-Enhancer/issues/new) with sanitized logs and reproduction steps.

Never publish passwords, API keys, CAPTCHA secrets, session cookies, or private user data in issues.

## 🔗 Links

- [📦 Releases](https://github.com/pterodactyl-v2/Registration-Enhancer/releases)
- [🐛 Issues](https://github.com/pterodactyl-v2/Registration-Enhancer/issues)
- [💡 Feature requests](https://github.com/pterodactyl-v2/Registration-Enhancer/issues/new)

## 📄 License

No license has been published yet. Until a license is added, do not assume permission to reuse, modify, or redistribute the source.

<div align="center">

Made for the Pterodactyl community 🪽

</div>
