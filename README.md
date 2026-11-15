# adsgen.vrisama.in - Vrisama Ads video ad generator (early access preview)

Single-page site served by GitHub Pages. A visitor enters an invite code, describes a product and the goal of the ad, and gets a 10 or 15 second AI video ad.

- `index.html` - the whole site. It calls the n8n webhook set in `N8N_WEBHOOK_URL` near the top of its script.
- `CNAME` - custom domain for GitHub Pages.
- `robots.txt` and the `noindex` meta tag keep the page out of search engines while it is unlisted.

The n8n workflow (script, images, video clips, voiceover, invite codes and the 30 ads per month limit) is not stored in this repository.

## Publishing

1. Settings > Pages > Deploy from branch `main`, folder `/ (root)`.
2. Custom domain: `adsgen.vrisama.in`.
3. DNS: add a CNAME record, host `adsgen`, target `mjeenugara9663.github.io`.
4. When the certificate is ready, turn on Enforce HTTPS.
