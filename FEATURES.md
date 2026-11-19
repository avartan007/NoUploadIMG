# Feature reference

A plain-language inventory of what the product does. No implementation details.

## Optimize

| Feature | Notes |
| --- | --- |
| Compress | WebP, AVIF (browser-dependent), JPEG and palette PNG. Quality mode or exact target file size. Presets for web, blog, email, thumbnails and near-lossless output. Never outputs a larger file. |
| Upscale | 1.5× to 4× multi-pass resampling with adaptive unsharp masking. Classical image processing — not generative AI. 64 MP output safety limit. |

## Convert

| Feature | Notes |
| --- | --- |
| Convert | Bulk PNG / JPEG / WebP / AVIF / PNG-8 / BMP / ICO / PDF, bundled as a ZIP. |
| SVG rasterising | Render SVG artwork to PNG at 1×–8×. |
| Image → SVG | Colour quantisation, contour tracing, simplification and Bézier smoothing, written from first principles. |
| SVG Studio | Clean up markup, export as JSX, CSS `url()` or Base64, and rasterise. |

## Modify

| Feature | Notes |
| --- | --- |
| Resize & presets | Exact pixels, percentages or 40+ platform presets exported together as a ZIP. Cover, contain and stretch modes. |
| Crop & rotate | Drag handles, locked ratios, rotation, flips and straighten with auto-fill. |
| Adjust & looks | Nine grading sliders and nine one-tap looks, applicable to a whole batch. |

## Create

| Feature | Notes |
| --- | --- |
| Beautify | Turn screenshots into finished visuals with gradients, macOS/browser frames, shadows and canvas ratios. |
| Favicons & icons | One logo produces `favicon.ico`, Apple touch, Android and maskable icons, a web manifest and the `<head>` snippet. |

## Secure

| Feature | Notes |
| --- | --- |
| Metadata scrub | Inspect EXIF, GPS, XMP and IPTC, then strip losslessly — JPEG and PNG bytes are cut without touching pixels, and the result is verified. |
| Redact | Pixelate, blur or black-bar regions. Optional face detection where the browser supports it. Irreversible. |
| Watermark | Single or tiled text with rotation, opacity and soft shadow. |

## Developer

| Feature | Notes |
| --- | --- |
| Dev Kit | Base64 / data URIs, tiny LQIP placeholders, palette → CSS variables or Tailwind tokens, responsive `srcset` ZIP with `<picture>` markup, SHA-256 and perceptual hashes. |

## Across the whole app

- Live preview before export
- Multi-file batch processing with ZIP download
- Drag-and-drop and paste support
- Keyboard-accessible controls and visible focus states
- `prefers-reduced-motion` support
- Six themes: Original, Mono, Paper, Linen, Slate and Graphite
- Theme choice persisted locally; applied before first paint
- Inline product film with clickable chapter timestamps
- Offline operation — no network required after load
