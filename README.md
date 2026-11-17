# KIPS — Kerala Invasive Plant Survey

Independent static website starter for the Kerala Invasive Plant Survey.

## Included
- `index.html` — public project homepage
- `login.html` — placeholder surveyor portal (authentication is not active)
- `style.css` — responsive visual design
- `app.js` — mobile navigation and Leaflet basemap
- `assets/favicon.svg` — project favicon

## Publish with GitHub Pages
1. Create a GitHub repository named **KIPS**.
2. Upload the contents of this folder to the repository root (not the enclosing ZIP).
3. In GitHub, open **Settings → Pages**.
4. Under Build and deployment, select **Deploy from a branch**.
5. Select branch `main` and folder `/ (root)`, then Save.
6. Wait for the Pages deployment to finish.

## Custom domain: survey.bioinvasion.in
1. In repository **Settings → Pages → Custom domain**, enter `survey.bioinvasion.in` and save.
2. In the DNS manager for `bioinvasion.in`, create a CNAME record:
   - Type: `CNAME`
   - Name/Host: `survey`
   - Target/Value: `unaisbot.github.io` (replace with the GitHub account's Pages hostname if different)
   - TTL: default
3. Wait for DNS propagation. Return to GitHub Pages and enable **Enforce HTTPS** when available.

Do not remove or change existing DNS records for `bioinvasion.in` or other subdomains.

## Important next stages
- Connect the KIPS GeoJSON layers exported from the pilot GIS package.
- Configure Firebase Authentication, Firestore and Storage.
- Implement surveyor assignments, quadrat forms, validation workflow and live status dashboard.
- Replace placeholder statistics with live database values.

The current website is a visual and navigation foundation only. It does not yet accept, store, or verify survey data. The map currently displays an OpenStreetMap basemap only.
