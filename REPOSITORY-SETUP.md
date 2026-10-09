# GitHub repository setup checklist

## Repository identity

**Suggested repository name:** `Registration-Enhancer`

**Suggested short description:**

> Customizable registration experience for Pterodactyl Panel 2.0, with responsive layouts, CAPTCHA integrations, and theme controls.

Leave the website field blank until official documentation or a project page exists.

## Topics

Use relevant topics such as:

- `pterodactyl`
- `pterodactyl-panel`
- `pterodactyl-extension`
- `pterodactyl-2`
- `registration`
- `captcha`
- `cloudflare-turnstile`
- `recaptcha`
- `php`
- `laravel`

Only use topics that accurately describe the published project. GitHub supports up to 20 topics; relevance is more useful than keyword stuffing.

## Suggested repository settings

- Visibility: **Public**
- Enable Issues.
- Enable Discussions only if you intend to actively answer questions there.
- Enable private vulnerability reporting if available.
- Protect the default branch once contributors or automation begin pushing.
- Add a license only after choosing the terms you want others to have.
- Upload a custom social preview image in Settings → Social preview.
- Pin the repository to your profile after the first useful release.

## First publication sequence

1. Create a public repository named `Registration-Enhancer`.
2. Upload the starter files.
3. Replace `YOUR_GITHUB_USERNAME` in `.github/ISSUE_TEMPLATE/config.yml` with your GitHub username.
4. Review README feature claims against the exact code you publish.
5. Add source, build/package instructions, and a license before presenting it as a complete open-source release.
6. Publish a tagged GitHub Release with a matching `.pteroext` asset only after testing it.
7. Add real screenshots or GIFs from the extension UI.

## Upload with Git

Run these commands from the directory containing the repository files after creating an empty GitHub repository:

```bash
git init
git add .
git commit -m "docs: prepare public repository"
git branch -M main
git remote add origin https://github.com/YOUR_GITHUB_USERNAME/Registration-Enhancer.git
git push -u origin main
```

Replace `YOUR_GITHUB_USERNAME` with your account name. If GitHub created a README or license automatically, reconcile those files before pushing.

## Discoverability and Trending

A clear README, accurate topics, real screenshots, useful releases, working installation instructions, active maintenance, and responsive issue handling improve discoverability and trust. They do not guarantee GitHub Trending placement or a particular ranking. Avoid fake stars, engagement exchanges, keyword stuffing, and copied content.
