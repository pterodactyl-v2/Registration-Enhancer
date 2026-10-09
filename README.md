<div align="center">

# ✨ Registration Enhancer

**A customizable, responsive registration experience for Pterodactyl Panel 2.0.**

[![Pterodactyl](https://img.shields.io/badge/Pterodactyl-Panel%202.0-3b82f6?style=for-the-badge)](https://github.com/pterodactyl/panel)
[![Status](https://img.shields.io/badge/status-in%20development-f59e0b?style=for-the-badge)](https://github.com/pterodactyl-v2/Registration-Enhancer/releases)
[![GitHub issues](https://img.shields.io/github/issues/pterodactyl-v2/Registration-Enhancer?style=flat-square)](https://github.com/pterodactyl-v2/Registration-Enhancer/issues)

[✨ Features](#-features) · [📦 Installation](#-installation) · [🧹 Clear-cache](#-clear-cache) · [🐛 Support](#-support)

</div>

---

## ✨ Features

- 🎨 Customizable registration-page themes and layout.
- 📱 Responsive registration page and popup.
- 🛡️ CAPTCHA integration options, depending on the released version.
- 🖼️ Configurable registration logo visibility.
- 🔔 GitHub release update notifications planned.

> 🚧 **In development:** This repository is being prepared while the extension is updated. Features, compatibility, and installation steps will be confirmed against the first published release.

## 📦 Installation

**Recommended — install through the Pterodactyl Extensions interface.**

1. Download the `.pteroext` asset from [GitHub Releases](https://github.com/pterodactyl-v2/Registration-Enhancer/releases) when a release is published.
2. Sign in to the panel as an administrator.
3. Open **Admin → Extensions**.
4. Upload/select the `.pteroext` package and follow the install or replacement confirmation.
5. Apply any release-specific instructions and verify registration in a private/incognito window.

Do not install a release until its compatibility notes match your panel build. Back up the panel and database before upgrades.

## 🧹 Clear cache

Run on the panel server after an installation or upgrade if changes do not appear. Adjust the PHP-FPM service name if your system uses a different PHP version.

```bash
cd /var/www/pterodactyl
php artisan optimize:clear
systemctl restart php8.4-fpm
systemctl restart nginx
```

Then hard-refresh the browser (`Ctrl` + `Shift` + `R`). These commands clear Laravel's optimized caches and restart PHP-FPM/Nginx; they do not replace a failed or incompatible extension installation.

## 🧩 Compatibility

- **Target:** Pterodactyl Panel 2.0 extension system.
- Check the release notes for the exact supported panel build and requirements.
- CAPTCHA services require correct provider configuration and server-side verification.

## 🐛 Support

- [Report a bug](https://github.com/pterodactyl-v2/Registration-Enhancer/issues/new)
- [Browse issues](https://github.com/pterodactyl-v2/Registration-Enhancer/issues)
- [View releases](https://github.com/pterodactyl-v2/Registration-Enhancer/releases)

When reporting an issue, include the panel build, extension version, steps to reproduce, and sanitized logs. **Never post passwords, API keys, CAPTCHA secrets, session cookies, or private user data.**

## 📄 License

A license will be added when the public source release is ready. Until then, do not assume permission to redistribute or reuse the code.

<div align="center">

Made for the Pterodactyl community 🪽

</div>
