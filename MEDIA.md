# Media catalogue

All media lives in `docs/`. Nothing here contains source code.

| File | Type | Use |
| --- | --- | --- |
| `launch-film.mp4` | Video, 1280×720, ~48 s | Main product film. Embedded in `README.md`. Chapters: 0:00 Intro, 0:06 The problem, 0:13 Drop & edit, 0:20 Compress, 0:25 Upscale & convert, 0:28 For developers, 0:35 Privacy, 0:41 Presets. |
| `launch-film.gif` | Animated GIF, 640×360 | Lightweight looping preview of the same film. |
| `logo.svg` | Vector logo | Header mark and favicon artwork. |
| `hero.png` | Screenshot | Landing page hero — also recommended as the GitHub social preview. |
| `landing-tour.gif` | Animated GIF | Walkthrough of the landing page sections. |
| `studio-compress.gif` | Animated GIF | Compression workflow with before/after comparison. |
| `studio-compress.png` | Screenshot | Compression UI still. |
| `studio-scrub.png` | Screenshot | Metadata scrubber still. |
| `studio-svg.png` | Screenshot | SVG export still. |
| `studio-tools.gif` | Animated GIF | Tour of the Studio tool groups. |

## Notes on the film

- The film is **generated**, not screen-recorded: each frame is rendered from the same
  interface code as the app, then assembled to video.
- The MP4 was encoded from the source animation at 24 fps with H.264 and fast-start
  metadata so it plays immediately on GitHub and in browsers.
- It has no audio track; the on-screen captions carry the narrative.

## Suggested placement in a GitHub README

```markdown
<video src="docs/launch-film.mp4" controls playsinline preload="metadata" width="100%"></video>
```

Already configured in [`README.md`](README.md).
