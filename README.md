# daub

Live at <https://xanimo.github.io/daub/>.

A fast, single-file paint and photo editor that runs entirely in the browser. No build step, no server, no accounts, no tracking — nothing you open or edit ever leaves your machine.

Built to paint *and* to scrub screenshots before you post them: crop, blur, pixelate, and a solid redact box. With a large helping of Kid Pix bolted on, since that is the paint program that understood kids would rather be surprised than be precise.

## Features
- Paint tools: pencil, brush, eraser, line, rectangle, oval, fill, text, eyedropper, spray
- Path: click point to point, double-click or `Enter` to finish, click the first point again to close the shape
- Select: drag a box (`Shift` constrains it to a square), drag it again to move the pixels, `Del` clears it, `Esc` drops it. Filters apply only inside a selection when one is up
- Zoom from 25% to 800% or fit to the window, with `-`, `+`, `0` and `1`
- Color palette + custom color picker, adjustable brush size
- Open any image and edit it
- One-tap filters: grayscale, invert, sepia, brighten, darken, contrast, saturate, fade, blur
- Crop
- Privacy tools: blur, pixelate, redact — drag a box over anything you want hidden
- Undo / redo (`Ctrl+Z` / `Ctrl+Y`), brush size with `[` and `]`
- Light / dark

## The Kid Pix bits
- Symmetry: Off, Mirror, Quad, Kaleido 8 and Kaleido 12 replay every stroke as rotated and mirrored copies about the centre of the canvas. Works with pencil, brush, eraser, spray, stamps and path
- Wacky brush: nine modes behind the Brush tool, so rainbow, drip, echo, fur, bubbles, pies, confetti and web as well as plain
- Rubber stamps: 65 of them, placed on click and laid as a trail on drag
- Wacky erasers: pick anything but Plain and clicking the canvas takes the whole picture away with a firecracker, a black hole, a fade, a drip, a shred or a sweep. All undoable
- Electric mixer: the **Mix** button mangles the whole picture a different way each press, nine effects deep, never the same one twice running
- Noises on everything, synthesised rather than sampled. The speaker button mutes it
- An undo button with a face on it

Reduced-motion settings skip the eraser animations and go straight to the cleared canvas.

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

Everything is static, so Pages serves it as-is, and the page makes no external requests at all. The wordmark prefers a locally installed Comic Sans and falls back to Comic Neue, which is embedded in `index.html` as a base64 woff2 so it renders the same on Linux and Android where Comic Sans is not installed.

## License
MIT. See LICENSE.

Comic Neue is licensed separately under the SIL Open Font License 1.1. See FONT-LICENSE.txt.
