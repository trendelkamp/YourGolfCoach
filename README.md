# Your Golf Coach — Landing Page

This repository powers the public marketing, privacy, and changelog website that Apple requires for the **Your Golf Coach** iOS + watchOS TestFlight beta. It is based on Emil Baehr’s automatic app landing page template but the configuration, copy, and assets have been replaced with product-specific content.

## Structure

| Path | Purpose |
| --- | --- |
| `_config.yml` | Brand colors, feature list, contact details, and store links rendered on the homepage. |
| `_pages/privacypolicy.md` | GDPR/CCPA-compliant Privacy Policy referenced inside the app. |
| `_pages/CHANGELOG.md` | Public release notes surfaced in the site header. |
| `assets/appicon.png` | 1024 × 1024 icon exported from the iOS project. |
| `assets/screenshot/` | Optional screenshot displayed inside the iPhone mockup (replace `yourscreenshot.png`). |
| `assets/videos/` | Optional promo video clips (webm/ogg/mp4). |

The rest of the files belong to the upstream theme (layouts, includes, Sass partials).

## Updating Content

1. **App / Store metadata**  
   - `ios_app_id` is already set to `6753873848` and the App Store link points to `https://apps.apple.com/app/id6753873848`. Update these if Apple changes the region slug or if you later ship a separate edition.  
   - Update `presskit_download_link` if you host a press kit ZIP either locally under `assets/` or on another service.

2. **Screenshots or video**  
   - Current screenshots live as `assets/screenshot/screenshot-01.png` … `screenshot-04.png`. Replace them with updated PNGs sized 1242×2688, 1125×2436, or 828×1792 (the last alphabetical file is what shows on the homepage).  
   - For video previews, drop appropriately encoded `.mp4/.mov` (Safari) and `.webm/.ogg` (Chrome/Firefox) files into `assets/videos/`.

3. **Legal documents**  
   - Update `_pages/privacypolicy.md` whenever data practices change (and adjust the “Last updated” date).  
   - Add more Markdown pages (e.g., Terms of Service) by duplicating files in `_pages/` and setting `include_in_header: true` if they should appear in the navigation.

4. **Brand tweaks**  
   - Modify colors, gradients, or device shell color in `_config.yml`.  
   - Swap `cover_image` with another hero illustration placed in `assets/`.

## Development & Deployment

1. Install Ruby + Bundler if you want to run Jekyll locally.
2. `bundle install` (uses the provided `Gemfile`).  
3. `bundle exec jekyll serve` to preview at `http://localhost:4000`.  
4. Push to the `main` branch — GitHub Pages will rebuild automatically (ensure Pages is enabled in the repo settings, targeting the `main` branch and `/ (root)` folder).  
5. If you configure a custom domain, fill the `CNAME` file with your hostname and update DNS (A/AAAA for GitHub Pages).

## Support

For content or legal questions email [app@fabianbuenker.de](mailto:app@fabianbuenker.de). For upstream theme issues see [Emil Baehr’s repository](https://github.com/emilbaehr/automatic-app-landing-page).
