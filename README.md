# ShotPDF website

Landing page, support page and privacy policy for the ShotPDF Chrome extension.
It is a plain static site with no build step, cookies or trackers.

## Publish on GitHub Pages (user site)

1. Create a repository named exactly `YOUR-USERNAME.github.io` (use your GitHub username).
2. Replace every `YOUR-USERNAME` in these files with your GitHub username:
   `index.html`, `privacy.html`, `support.html`, `404.html`, `robots.txt`, `sitemap.xml`, `llms.txt`.
   (In VS Code: Ctrl+Shift+H, find `YOUR-USERNAME`, replace all.)
3. Upload all files and folders to the repository root, including the hidden `.nojekyll` file.
4. Go to Settings → Pages → Source: "Deploy from a branch", branch `main`, folder `/ (root)`.
5. After a minute the site is live at `https://YOUR-USERNAME.github.io/`.

## After it is live

- Chrome Web Store dashboard: set the **Privacy policy URL** to `https://YOUR-USERNAME.github.io/privacy.html`,
  the **Support URL** to `https://YOUR-USERNAME.github.io/support.html`, and the **Homepage URL** to the home page.
- Google Search Console: add the site, then submit `sitemap.xml`.
- Bing Webmaster Tools: import from Search Console (Bing also feeds ChatGPT and Copilot search).
- Check the share preview with https://www.opengraph.xyz and the structured data with
  https://search.google.com/test/rich-results

## Files

| File | Purpose |
|---|---|
| `index.html` | Landing page with SoftwareApplication, FAQPage, Organization and WebSite structured data |
| `support.html` | Help and contact page (saqibsohaib48@gmail.com) with FAQPage data |
| `privacy.html` | Privacy policy for the extension and this website |
| `404.html` | Page GitHub Pages shows for broken links |
| `robots.txt` | Allows all search engines and AI crawlers, points to the sitemap |
| `sitemap.xml` | List of pages for search engines |
| `llms.txt` | Plain-text summary for AI assistants (ChatGPT, Claude, Perplexity, Gemini) |
| `site.webmanifest` | App name, colors and icons for browsers |
| `.nojekyll` | Tells GitHub Pages to serve the files as they are |
| `assets/site.css` | All styles |
| `assets/fonts/` | Self-hosted fonts (Bricolage Grotesque, Atkinson Hyperlegible; SIL Open Font License) |
| `assets/img/` | Icons, share image and product screenshots |
