<div align="center">

# ✨ Registration Enhancer

**A modern, configurable registration experience for Pterodactyl Panel 2.0.**

[![Pterodactyl Panel 2.0](https://img.shields.io/badge/Pterodactyl-Panel%202.0-3b82f6?style=for-the-badge)](https://github.com/pterodactyl/panel)
[![GitHub release](https://img.shields.io/github/v/release/pterodactyl-v2/Registration-Enhancer?style=for-the-badge&label=latest%20release)](https://github.com/pterodactyl-v2/Registration-Enhancer/releases)
[![GitHub issues](https://img.shields.io/github/issues/pterodactyl-v2/Registration-Enhancer?style=flat-square)](https://github.com/pterodactyl-v2/Registration-Enhancer/issues)
[![License](https://img.shields.io/badge/license-not%20published-lightgrey?style=flat-square)](#-license)

[Features](#-features) · [Screenshots](#-screenshots) · [Installation](#-installation) · [Cache clearing](#-cache-clearing) · [Support](#-support)

</div>

---

## ✨ Features

- 🎨 **Registration themes** — customize the supported registration page appearance.
- 📱 **Responsive UI** — registration page and popup layouts for desktop and mobile.
- 🪟 **Registration popup** — alternate registration flow where enabled.
- 🛡️ **CAPTCHA options** — Cloudflare Turnstile and Google reCAPTCHA v2 (invisible), when supported by the installed release.
- 🖼️ **Logo controls** — configure supported registration logo visibility.
- 🔗 **Login integration** — convenient entry point to registration from the login page.
- 🔔 **Update notifications** — GitHub release checks are planned; check the release notes for current availability.

> **Note:** Only features included and documented in a published release should be considered available. CAPTCHA providers require correct keys and server-side verification.

## 🖼️ Screenshots

Screenshots will be added here after the updated extension UI is published and verified.

<!--
After adding real screenshots to the screenshots/ folder, uncomment and update these lines:
![Registration page](screenshots/registration-page.png)
![Registration popup](screenshots/registration-popup.png)
![Extension settings](screenshots/extension-settings.png)
![Mobile layout](screenshots/mobile-registration.png)
-->

## 📦 Installation

**Recommended: install through the Pterodactyl Extensions interface.**

1. Open [GitHub Releases](https://github.com/pterodactyl-v2/Registration-Enhancer/releases) and download the `.pteroext` asset for the version you want.
2. Sign in to your panel with an administrator account.
3. Open **Admin → Extensions**.
4. Upload/select the `.pteroext` package and follow the installation or replacement confirmation.
5. Read the release notes, configure any required CAPTCHA settings, and test registration in a private browser window.

Back up your panel files and database before upgrading. Confirm that the release supports your exact Panel 2.0 build before installing.

## ⚙️ Configuration

Available settings depend on the installed extension version. Where provided, configure the registration page, popup, theme/logo options, and CAPTCHA provider in the extension settings.

### 🛡️ CAPTCHA providers

- **Cloudflare Turnstile** — configure the site key and secret key from the Cloudflare dashboard.
- **Google reCAPTCHA v2 (invisible)** — configure the matching site key and secret key from the Google reCAPTCHA admin console.

Use the provider type and settings shown by your installed release. Keep secret keys private, and verify that server-side validation is enabled. Never put secret keys in screenshots, issues, or public source files.

## 🧹 Cache clearing

After installing or upgrading, if changes do not appear, run these commands on the panel host. Adjust the PHP-FPM service name if your system uses a different PHP version.

```bash
cd /var/www/pterodactyl
php artisan optimize:clear
systemctl restart php8.4-fpm
systemctl restart nginx
```

Then hard-refresh your browser with **Ctrl + Shift + R**. These commands clear Laravel's optimized caches and restart services; they do not repair an incompatible or failed extension installation.

## 🧩 Compatibility

- **Target:** Pterodactyl Panel 2.0 extension system.
- Check each release's notes for the supported panel build and requirements.
- Panel 2.0 and its extension ecosystem may change; test upgrades on a staging instance when possible.

## 🐛 Support

- [Open an issue](https://github.com/pterodactyl-v2/Registration-Enhancer/issues/new)
- [Browse existing issues](https://github.com/pterodactyl-v2/Registration-Enhancer/issues)
- [Download releases](https://github.com/pterodactyl-v2/Registration-Enhancer/releases)

Include the panel build, extension version, reproduction steps, and sanitized logs. **Never share passwords, API keys, CAPTCHA secrets, session cookies, or private user data.**

## 📄 License

A license has not yet been published. Until one is added, do not assume permission to reuse, redistribute, or modify the source.

<div align="center">

Made for the Pterodactyl community 🪽

</div>
