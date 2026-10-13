# Breakdown

Phone app for Cameron's back row program (Pollock on the pitch, Laid off it). The full written program is in `~/LIFE/Training/Back-Row-Program.md`.

Plain HTML, no build step. Everything is in `index.html`; `sw.js` makes it work offline once installed; `manifest.webmanifest` and the icons make it installable.

- Data lives in the phone's local storage under the key `breakdown:v1`, so it never mixes with the old Form app on the same github.io address.
- Back up from Settings > Share backup.

## Run locally
```bash
python3 -m http.server 8791 --directory ~/Projects/breakdown
```

## Put it on the iPhone
It needs a real web address. Host the folder on GitHub Pages, open the address in Safari, then Share > Add to Home Screen.
After changing `index.html`, bump `V` in `sw.js` so installed copies pick up the new version.
