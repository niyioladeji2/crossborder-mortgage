# CrossBorder Mortgage Calculator — phone app

This folder is an installable web app (PWA). Once it's online, you add it to your
home screen and it opens full-screen like a regular app, keeps your inputs, and
works offline.

## 1. Put it online (free, about 2 minutes)

**Netlify Drop (easiest)**
1. On a computer, go to https://app.netlify.com/drop
2. Drag this whole `crossborder-mortgage` folder onto the page.
3. You get a link like `https://something.netlify.app`. Sign up (free) to keep it
   permanently and give it a nicer name.

**Other free options:** GitHub Pages, Cloudflare Pages or Vercel. Upload the folder
contents as a static site; no build step is needed.

The app must be served over https for the install and offline features to work.

## 2. Install it on your phone

**iPhone / iPad (Safari)**
1. Open your link in Safari.
2. Tap the Share button, then **Add to Home Screen**, then **Add**.

**Android (Chrome)**
1. Open your link in Chrome.
2. Tap **Install app** when prompted, or the ⋮ menu → **Install app**
   (some versions say **Add to Home screen**).

## Updating

Replace the files on your host with a new version. Open the app while online and
it picks up the changes. If you change `sw.js`, bump `CACHE` (e.g. `crossborder-v2`).

## Files

- `index.html` — the whole calculator
- `manifest.webmanifest` — app name, colors and icons
- `sw.js` — offline support
- `icons/` — home-screen icons

## Want it in the App Store or Google Play?

Wrap this same folder with Capacitor (https://capacitorjs.com) to produce native
iOS and Android projects. Publishing needs an Apple Developer account ($99 USD/yr)
and a Google Play developer account ($25 USD one-time).
