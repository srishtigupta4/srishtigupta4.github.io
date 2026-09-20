# Srishti Gupta — personal site (Kigen-styled template)

Plain HTML/CSS, no build step, no WordPress needed. Styled after the look of the "Kigen" WordPress.com theme you gave me (cream background, black ink, italic Newsreader serif headings, a narrow reading column, and the six-color striped rule at the bottom of every page) — but rebuilt as static files so it works on GitHub Pages, since the original theme only runs inside WordPress.

Six pages, same as before: `index.html` (Home), `research.html`, `teaching.html`, `cv.html`, `personal.html`, `contact.html`, all sharing `assets/style.css`.

**Every page is a placeholder shell.** Anything in `[brackets, italic]` is text for you to write. Every photo is a plain cream box with a dashed border and its required size printed right on it — that's not decoration, it's the spec for the image that goes there.

## Filling in text

Open each `.html` file in a text editor (or GitHub's own editor) and replace the bracketed text. The section headings and page structure (Education, Positions, the four research project names, etc.) are already in place from your earlier version — just the prose, bios, and paper lists were cleared out per your request.

## Filling in images

Replace each placeholder file in `assets/images/` with your own photo **using the exact same filename**, so you don't have to touch the HTML at all. Sizes below are recommended, not strict — a little off is fine, but matching the aspect ratio (square / portrait / landscape) keeps the layout from looking stretched or cropped oddly.

| File to replace | Used on | Recommended size | Shape |
|---|---|---|---|
| `assets/images/placeholder-headshot.jpg` | Home (circle photo by your name) | 400 &times; 400px | Square |
| `assets/images/placeholder-gallery-1.jpg` through `-6.jpg` | Home (photo grid) | 800 &times; 1000px each | Portrait |
| `assets/images/placeholder-research-community.jpg` | Research &mdash; Community science & sustainability | 1200 &times; 800px | Landscape |
| `assets/images/placeholder-research-indigenous.jpg` | Research &mdash; Indigenous AI | 1200 &times; 800px | Landscape |
| `assets/images/placeholder-research-health.jpg` | Research &mdash; Public health & wellbeing | 1200 &times; 800px | Landscape |
| `assets/images/placeholder-research-civic.jpg` | Research &mdash; Community life & civic technology | 1200 &times; 800px | Landscape |
| `assets/images/placeholder-teaching.jpg` | Teaching | 1200 &times; 800px | Landscape |
| `assets/images/placeholder-personal-1.jpg` through `-3.jpg` | Personal | 800 &times; 1000px each | Portrait |

No image is required on the CV or Contact pages.

## Your papers are still here, just not linked

The 16 paper PDFs I tracked down and hosted earlier are still sitting in `assets/papers/` (same file names as before), but the Research page now shows `[Paper title]` placeholders instead of linking to them, since you asked for placeholder text throughout. When you write the real paper list for each project, you can link straight to these existing files, for example:

```html
<li><a href="assets/papers/distance-matters-cscw.pdf">Distance Matters in Citizen-Based Water Quality Monitoring</a>
<div class="venue">Proceedings of the ACM on Human-Computer Interaction, 9(7), 2025</div></li>
```

Two papers still aren't in there at all (an anonymized review draft and a manuscript with tracked changes still in it) — see the note in the previous version's history if you need the details, or just ask me again.

Your CV PDF is at `assets/Srishti_Gupta_CV.pdf` — the "Download full CV" button on the CV page already points to it. Swap in a newer version any time by replacing that file (same name).

## Publish with GitHub Pages

Your GitHub username is **srishtigupta4**.

1. Go to your existing repo at `srishtigupta4.github.io` (or create it at [github.com/new](https://github.com/new) if you haven't yet, named exactly `srishtigupta4.github.io`).
2. **If you're replacing the previous version:** delete the old files first (select them on the repo's file list → the "..." menu or trash icon → delete → commit), or just upload the new ones with the same names, GitHub will overwrite files that share a path. The `assets/papers/` and `assets/images/` folders are new paths, so drag those in fully.
3. Click **Add file → Upload files**, then drag in everything from this package: `index.html`, `research.html`, `teaching.html`, `cv.html`, `personal.html`, `contact.html`, `README.md`, and the whole `assets` folder (including `assets/images` and `assets/papers` as subfolders — check the file list GitHub shows before committing to make sure it says `assets/images/...` and not just flat filenames).
4. Commit. If Pages was already turned on from before, it redeploys automatically within a minute or two. If not: **Settings → Pages**, Source: "Deploy from a branch," branch **main**, folder **/ (root)**.
5. Visit `https://srishtigupta4.github.io` to see it live.
