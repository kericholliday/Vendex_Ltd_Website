# Vendex Ltd – static site

## Deploy on GitHub Pages
1. Create a repo and upload everything in this folder (index.html at the root).
2. Settings → Pages → Deploy from a branch → main / (root) → Save.

## Use your own domain (vendex-ltd.com)
1. Rename `CNAME.example` to `CNAME` (file contents: your domain, e.g. `www.vendex-ltd.com`), commit it.
2. In your domain registrar's DNS: add a CNAME record `www` → `USERNAME.github.io`, and for the bare domain add GitHub's A records (see docs.github.com → "Managing a custom domain for GitHub Pages").
3. Settings → Pages → enable "Enforce HTTPS" once the certificate is ready.
Only switch DNS when you're ready to leave Squarespace. The canonical, og:image, sitemap and robots URLs already assume https://www.vendex-ltd.com.

## Placeholders to replace before going live
- **Phone number**: `(864) 555-0100` / `+18645550100` appears in header, contact section, footer, mobile bar (search & replace). Also add it to the JSON-LD block.
- **Contact form**: create a free form at formspree.io and replace `YOUR_FORM_ID` in index.html.
- **Family/machine photo**: add `images/family.jpg` and change the src in the yellow "Family Owned and Operated" section near the top.
- **Testimonials**: fill in real quotes and remove the `hidden` attribute on the #testimonials section.
- **FAQ answers**: edit to match your real terms (minimums, contract, etc.).
- **service-area.html**: paste your original page text.
