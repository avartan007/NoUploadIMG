# Public repo setup

This repository is a **portfolio showcase only**. It contains no source code. Use this
file to configure the GitHub repository before publishing.

## 1. Repository description

Copy into *Settings → General → Description*:

> Privacy-first browser image toolkit — 14 tools, zero uploads, single-file build. Portfolio showcase by Avartan Thlay.

## 2. Topics

Copy into *Settings → General → Topics* (also in [`TOPICS.txt`](TOPICS.txt)):

```text
react, typescript, vite, tailwindcss, frontend, webapp, image-processing,
privacy, offline-first, client-side, browser-api, portfolio, ui-design,
design-systems, developer-tools, no-backend
```

## 3. Settings

| Setting | Value |
| --- | --- |
| Visibility | Public |
| Default branch | `main` |
| Homepage | Add a live demo URL if one exists, otherwise leave blank |
| Issues | Off (unless you want recruiter questions there) |
| Wiki | Off |
| Projects | Off |
| Allow fork | Off — the source is not in this repository |
| Template repository | Off |

## 4. Social preview

Use `docs/hero.png` as the social preview image
(*Settings → General → Social preview → Upload an image*).

## 5. What this repo contains

| File | Purpose |
| --- | --- |
| `README.md` | Main showcase — video, tour, feature overview |
| `PROJECT_SUMMARY.md` | One-page product brief |
| `FEATURES.md` | Full feature inventory |
| `PRIVACY.md` | Privacy architecture explained |
| `MEDIA.md` | Asset catalogue and video details |
| `SHOWCASE_NOTICE.md` | What is and isn't public |
| `TOPICS.txt` | Copy-paste topic list |
| `docs/` | Logo, screenshots, GIF tours and the launch film MP4 |

## 6. Pushing from this folder

Run these commands **from the showcase folder**, not from the source project:

```bash
cd public-repo
git init
git add .
git commit -m "Docs: add NoUpload IMG portfolio showcase"
git branch -M main
git remote add origin https://github.com/avartan007/NoUploadIMG.git
git push -u origin main
```

If the repository was created with a default commit, pull first:

```bash
git pull origin main --allow-unrelated-histories
```

## 7. Safety checklist before pushing

- [ ] No `src/` directory
- [ ] No `package.json`, lockfile or config files
- [ ] No `.ts`, `.tsx`, `.js`, `.css` or `.html` source files
- [ ] No terminal commands that reveal internal paths
- [ ] Only Markdown, images, the SVG logo and the MP4/GIF tours
- [ ] Source repository is confirmed **private**

## 8. Suggested README badge line (optional)

```markdown
![Static single-file app](https://img.shields.io/badge/backend-none-30d158?style=for-the-badge)
![Bytes uploaded](https://img.shields.io/badge/bytes%20uploaded-0-30d158?style=for-the-badge)
```
