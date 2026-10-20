# FinCale Website

Official support website for the FinCale iOS app: landing page, technical support,
privacy policy and terms of service.

## Structure

```
FinCale_website/
├── index.html          Landing page (English)
├── support.html        Technical support (English)
├── support-zh.html     Technical support (Chinese)
├── privacy.html        Privacy policy (English)
├── privacy-zh.html     Privacy policy (Chinese)
├── terms.html          Terms of service (English)
├── terms-zh.html       Terms of service (Chinese)
└── assets/css/style.css  Shared stylesheet
```

Plain HTML5 + CSS3. No framework, no build step: edit the files and push.

## Deployment

GitHub Pages serves project sites at `https://wangjin2013.github.io/FinCale_website/`.

1. Repository → Settings → Pages → Source: `Deploy from a branch`, branch `main`,
   folder `/ (root)`.
2. Wait a minute, then verify every page loads:
   - `…/FinCale_website/support.html`
   - `…/FinCale_website/support-zh.html`
   - `…/FinCale_website/privacy.html`
   - `…/FinCale_website/privacy-zh.html`
   - `…/FinCale_website/terms.html`
   - `…/FinCale_website/terms-zh.html`

`app-ads.txt` does **not** belong in this repository. Google reads it from the domain
root only, so it lives in the separate `wangjin2013.github.io` repository.

## Editing notes

- File names are part of the public URLs. Renaming a page requires updating every link —
  and, if the app links to it, the app as well. A dead privacy-policy link is something
  App Review checks.
- Keep the English and Chinese versions in sync. The Chinese files use the `-zh` suffix.
- The landing page is intentionally English-only: it is the first impression for people
  who have not installed the app yet.
- Contact address: `michael.wangjin2012@gmail.com` — keep it identical to the address
  used in the App Store listing.
