# Daub

A fast, single-file paint and photo editor that runs entirely in the browser. No build step, no server, no accounts, no tracking — nothing you open or edit ever leaves your machine.

Built to paint *and* to scrub screenshots before you post them: crop, blur, pixelate, and a solid redact box.

## Features
- Paint tools: pencil, brush, eraser, line, rectangle, oval, fill, text, eyedropper, spray
- Color palette + custom color picker, adjustable brush size
- Open any image and edit it
- One-tap filters: grayscale, invert, sepia, brighten, darken, contrast, saturate, fade, blur
- Crop
- Privacy tools: blur, pixelate, redact — drag a box over anything you want hidden
- Undo / redo (`Ctrl+Z` / `Ctrl+Y`), brush size with `[` and `]`
- Light / dark

## Hiding sensitive information
For actually removing information — a wallet address, a username, a face — use **Redact**, the solid black box. Blur and pixelate look cleaner but can sometimes be partially reversed; a black box cannot.

## Saving
Click **Save**, then right-click the image and choose *Save image as…* (press and hold on mobile).

## Run locally
Open `index.html` in any browser. That is the whole install.

## Deploy to GitHub Pages
1. Put these files at the root of a repo.
2. Push to `main`.
3. Settings → Pages → Build and deployment → Source: **Deploy from a branch**, Branch: `main` / `/ (root)`.
4. It goes live at `https://<user>.github.io/<repo>/`.

Everything is static, so Pages serves it as-is. The only external request is the Google Fonts stylesheet for the wordmark; delete that one `<link>` in `index.html` to make it fully offline.

## License
MIT. See LICENSE.
