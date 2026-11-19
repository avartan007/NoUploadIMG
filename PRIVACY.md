# Privacy by architecture

NoUpload IMG is designed so that privacy is a property of the system, not a promise in
a document.

## What happens when you use it

1. You drop, paste or select an image.
2. The browser decodes it into memory.
3. Platform APIs process it locally — Canvas, `createImageBitmap`, Web Crypto and
   Compression Streams.
4. The result is handed straight back to you as a download.
5. Closing the tab discards everything.

At no point does the file leave your device.

## What is not there

| Usually present elsewhere | Here |
| --- | --- |
| Upload endpoint | None |
| User accounts | None |
| Database | None |
| Analytics | None |
| CDN / external fonts | None |
| Tracking pixels | None |
| Cookies | None |

## The proof is visible

The Studio includes a live network audit. It watches outbound requests — `fetch`,
XHR, beacons and resource loads — and lists them in the interface while you work.
The default count is **zero**, and ordinary use keeps it there.

This is deliberately in-product rather than buried in documentation: the claim can be
checked by anyone, in seconds, without reading code.

## Offline is the easiest test

Turn on airplane mode, reload, and use the app. Everything still works because there
is nothing to fetch. That single check demonstrates the entire architecture.

## Distribution

The production build is a **single self-contained HTML file**. It can be double-clicked
locally or hosted on any static file server. There is no runtime service to operate,
no environment to configure and no data to retain.

> This document describes behaviour, not implementation. Source is private; see
> [`SHOWCASE_NOTICE.md`](SHOWCASE_NOTICE.md).
