# Project summary — NoUpload IMG

**One-line pitch:** A complete image editor that never uploads your images, shipped as a
single static file with a live network audit to prove it.

## The problem

Every mainstream online image tool works the same way: your file travels to someone
else's server, gets processed there, and comes back. Even with good intentions, that
means trusting a privacy policy and a third party with private photos, screenshots and
client work.

## The solution

Move the entire editor into the browser. NoUpload IMG decodes images into memory and
uses platform APIs — Canvas, `createImageBitmap`, Web Crypto, Compression Streams — to
do the work locally. The build output is one HTML file with everything inlined.

The product doesn't ask you to trust a claim. A live audit panel in the Studio records
every outbound request the page attempts and shows the count in real time. It stays at
zero.

## Scope delivered

- 14 tools across optimize, convert, modify, create, secure and developer workflows
- Batch processing and ZIP export throughout
- 40+ size presets for web, social, app store and PWA outputs
- Hand-written image → SVG tracing and palette PNG writer
- Byte-level EXIF/GPS metadata removal
- Six switchable themes with local persistence
- A 48-second generated product film with seekable chapters
- Fully static, offline-capable, no dependencies at runtime

## Why it stands out

1. **Zero-infrastructure product** — no server, no database, no accounts, no analytics.
2. **Verifiable privacy** — the proof is in the UI, not a policy document.
3. **Real algorithms** — tracing, quantisation, upscaling and compression are implemented rather than delegated to a service.
4. **Production polish** — live previews, drag-and-drop, keyboard support, reduced-motion support, responsive layout and a designed theme system.

## Outcome

A working, shippable image toolkit that demonstrates end-to-end frontend engineering:
complex browser APIs, performance-conscious processing, careful UI design and a clear
product argument.

> Source is private. See [`SHOWCASE_NOTICE.md`](SHOWCASE_NOTICE.md).
