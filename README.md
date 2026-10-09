<div align="center">

<img src="assets/registration-enhancer-banner.svg" alt="Registration Enhancer — Pterodactyl v2.0" width="100%">

# ✨ Registration Enhancer

**A modern, configurable registration experience for Pterodactyl v2.0.**

<p>
  <img src="https://img.shields.io/badge/Pterodactyl-v2.0-3B82F6?style=for-the-badge&logo=pterodactyl&logoColor=white" alt="Pterodactyl v2.0">
  <img src="https://img.shields.io/badge/status-in%20development-8B5CF6?style=for-the-badge" alt="In development">
  <a href="https://github.com/pterodactyl-v2/Registration-Enhancer/issues"><img src="https://img.shields.io/github/issues/pterodactyl-v2/Registration-Enhancer?style=flat-square&color=2563eb" alt="Issues"></a>
</p>

[✨ Features](#-features) · [🖼️ Preview](#️-preview) · [📦 Installation](#-installation) · [⚙️ Configuration](#️-configuration) · [🧹 Cache clearing](#-cache-clearing) · [🛠️ Troubleshooting](#️-troubleshooting)

</div>

---

> [!IMPORTANT]
> **In development.** This repository is being prepared while the extension is updated. Check the release notes for compatibility and available features. Only functionality included in a published package should be considered available.

## ✨ Features

<table>
<tr>
<td width="50%">

### 🎨 Theme controls
Customize the supported registration-page appearance using extension settings.

</td>
<td width="50%">

### 📱 Responsive layouts
Registration page and popup layouts designed for desktop and mobile.

</td>
</tr>
<tr>
<td width="50%">

### 🛡️ CAPTCHA integrations
Cloudflare Turnstile and Google reCAPTCHA v2 (invisible), subject to the installed release.

</td>
<td width="50%">

### 🖼️ Logo controls
Configure supported registration logo visibility.

</td>
</tr>
<tr>
<td width="50%">

### 🔗 Login integration
A convenient entry point from the login page to registration.

</td>
<td width="50%">

### 🔔 Update notifications
GitHub release notifications are planned. Check release notes for current availability.

</td>
</tr>
</table>

## 🖼️ Preview

The updated extension screenshots will be published here after the UI is verified. For now, the banner above is project branding, not a screenshot of the working interface.

<!-- Replace these with genuine screenshots saved in assets/ when available.
<div align="center">
  <img src="assets/registration-page.png" alt="Registration page" width="49%">
  <img src="assets/registration-popup.png" alt="Registration popup" width="49%">
  <img src="assets/extension-settings.png" alt="Extension settings" width="49%">
  <img src="assets/mobile-registration.png" alt="Mobile registration" width="49%">
</div>
-->

## 📦 Installation

**Recommended: install through the Pterodactyl Extensions interface.**

1. Open [**GitHub Releases**](https://github.com/pterodactyl-v2/Registration-Enhancer/releases).
2. Download the `.pteroext` package for a published version.
3. Sign in to your panel with an administrator account.
4. Open **Admin → Extensions**.
5. Upload the package and follow the installation or replacement prompts.
6. Review the release notes, configure required options, and test registration in a private browser window.

> [!CAUTION]
> Back up your panel files and database before upgrading. Confirm that the release supports your exact Pterodactyl v2.0 build. Avoid unofficial package mirrors.

## ⚙️ Configuration

Available settings depend on the installed extension version. Use the extension settings interface and its release notes as the source of truth.

### 🛡️ CAPTCHA providers

| Provider | Configuration |
|---|---|
| **Cloudflare Turnstile** | Configure the matching site key and secret key in Cloudflare. |
| **Google reCAPTCHA v2 (invisible)** | Configure the matching site key and secret key in the Google reCAPTCHA admin console. |

Provider availability depends on the published version. Keep secret keys private and confirm server-side verification is active; showing a widget alone is not sufficient protection.

## 🧹 Cache clearing

If changes do not appear after installation or an upgrade, run these commands on the panel host. Change the PHP-FPM service name if your server uses another PHP version.

```bash
cd /var/www/pterodactyl
php artisan optimize:clear
systemctl restart php8.4-fpm
systemctl restart nginx
```

Then hard-refresh the browser with **Ctrl + Shift + R**. These commands clear Laravel's optimized caches and restart services; they cannot repair an incompatible package or failed installation.

## 🧩 Compatibility

- **Target:** Pterodactyl v2.0 extension system.
- Check each release's notes for the supported panel build and requirements.
- The v2.0 ecosystem can evolve; test upgrades on a staging instance when possible.

## 🛠️ Troubleshooting

- **Changes not visible:** clear the cache, restart the relevant services, and hard-refresh the browser.
- **Installation fails:** verify package integrity and panel compatibility, then review panel logs.
- **CAPTCHA fails:** check the selected provider, keys, allowed hostnames, and server-side verification.
- **Need help?** [Open an issue](https://github.com/pterodactyl-v2/Registration-Enhancer/issues/new) with reproduction steps and sanitized logs.

Never post passwords, API keys, CAPTCHA secrets, session cookies, or private user data.

## 🔗 Project links

<p>
  <a href="https://github.com/pterodactyl-v2/Registration-Enhancer/releases">📦 Releases</a> ·
  <a href="https://github.com/pterodactyl-v2/Registration-Enhancer/issues">🐛 Issues</a> ·
  <a href="https://github.com/pterodactyl-v2/Registration-Enhancer/issues/new">💡 Feature request</a>
</p>

## 📄 License

No license has been published yet. Until a license is added, do not assume permission to reuse, modify, or redistribute the source.

<div align="center">

**Made for the Pterodactyl community** 🪽

</div>
