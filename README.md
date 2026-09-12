# BRIX — website

Static multi-page site for **BRIX London Bridge**. Plain HTML/CSS/JS, no build step.

## Pages
`index.html` (home), `restaurant.html`, `sixt33n.html`, `hire.html`, `menu.html`, `roast.html`,
`brunch.html`, `cocktails.html`, `events.html`, `membership.html`, `contact.html`.
Shared assets: `img/` (photos), `vid/` (background loops), `favicon.png`, `apple-touch-icon.png`, `og.jpg`.
`.nojekyll` tells GitHub Pages to serve files as-is.

## Deploy to GitHub Pages
1. Create a repo under **thewondergroup** (e.g. `brix-website`).
2. Put all these files at the **repo root** (keep the `img/` and `vid/` folders).
3. Settings -> Pages -> Deploy from a branch -> `main` -> `/ (root)`, Save.
4. Live at `https://thewondergroup.github.io/brix-website/` in a minute.

### Custom domain (brixldn.com)
- Add a `CNAME` file at the root containing `brixldn.com`, point DNS at GitHub Pages, set the domain in Settings -> Pages, enable HTTPS.
- Then update `og:image` in each page to the absolute `https://brixldn.com/og.jpg`.

## Before it's fully live
- The **membership sign-up** and **private-hire enquiry** forms are front-end only — wire them to a handler (Google Sheet / mailing tool) or submissions go nowhere.
- Give the menu prices/wording and members-club T&Cs a final check.
- `events@brixldn.com` and the member-questions address are placeholders — swap if needed.
