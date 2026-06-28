# Nethraja Kandula Personal Webpage

This project is a one-page professional portfolio built with plain HTML, CSS, and vanilla JavaScript. It is designed for recruiters, collaborators, and conference contacts who scan the printed QR code and land on a polished overview page.

## Project Structure

```text
Webpage/
├── .gitignore
├── index.html
├── styles.css
├── script.js
├── index.html.bak
├── styles.css.bak
├── script.js.bak
├── assets/
│   ├── headshot.JPG
│   ├── nethraja-kandula-cv.pdf
│   ├── documents/
│   │   ├── nethraja-kandula-cv.pdf
│   │   └── nethraja-kandula-resume.pdf
│   ├── presentations/
│   │   ├── fafp-2023.jpeg
│   │   ├── ift-2024-1.jpeg
│   │   ├── ift-2024-2.jpeg
│   │   └── iafp-2025.jpeg
│   └── media/
│       ├── three-minute-thesis-2026.png
│       ├── grad-impact-profile.png
│       ├── seafood-mislabeling.png
│       ├── nsf-icorps.png
│       └── shrimp-research.png
└── README.md
```

## Page Sections

The webpage currently includes:

1. About
2. Expertise
3. Presentations
4. Featured Stories & Media
5. CV & Résumé
6. Contact

## Presentation Images

Presentation photographs are stored in:

```text
assets/presentations/
```

Current files:

- `fafp-2023.jpeg`
- `ift-2024-1.jpeg`
- `ift-2024-2.jpeg`
- `iafp-2025.jpeg`

## Media Thumbnails

Featured Stories & Media thumbnails are stored in:

```text
assets/media/
```

Current files:

- `three-minute-thesis-2026.png`
- `grad-impact-profile.png`
- `seafood-mislabeling.png`
- `nsf-icorps.png`
- `shrimp-research.png`

These are local image files used directly in the cards. The cards link to the original external articles, profiles, videos, and galleries in new tabs.

## Preview Locally

From the project folder, start a local server:

```bash
python3 -m http.server 8000
```

Then open:

```text
http://localhost:8000
```

## Live Website

Published site:

```text
https://nethrajak.github.io/
```

GitHub repository:

```text
https://github.com/NethrajaK/NethrajaK.github.io
```

## GitHub Pages Settings

This project is already configured for GitHub Pages.

```text
Repository: NethrajaK/NethrajaK.github.io
Branch: main
Folder: / (root)
```

To verify the deployment settings later:

1. Open the repository on GitHub.
2. Go to `Settings`.
3. Open `Pages`.
4. Confirm the source is `Deploy from a branch`.
5. Confirm the branch is `main` and the folder is `/ (root)`.

## Replacing the CV

The live CV link points to:

```text
assets/documents/nethraja-kandula-cv.pdf
```

To replace it:

1. Export the updated CV as a PDF.
2. Replace `assets/documents/nethraja-kandula-cv.pdf`.
3. Keep the same filename.

Keeping the same filename allows future updates without editing the HTML.

## Replacing the Résumé

The live résumé link points to:

```text
assets/documents/nethraja-kandula-resume.pdf
```

To replace it:

1. Export the updated résumé as a PDF.
2. Replace `assets/documents/nethraja-kandula-resume.pdf`.
3. Keep the same filename.

Keeping the same filename allows future updates without editing the HTML.

## Replacing a Media Thumbnail

To replace a Featured Stories & Media thumbnail:

1. Prepare the new image.
2. Save it in `assets/media/`.
3. Reuse the same filename when possible.
4. If the filename changes, update the corresponding `src` in `index.html`.

Examples:

- `assets/media/seafood-mislabeling.png`
- `assets/media/shrimp-research.png`

## Adding Another Presentation

To add another presentation card:

1. Copy the new image into `assets/presentations/`.
2. Add a new card inside the `#presentations` section in `index.html`.
3. Follow the same structure as the existing presentation cards.
4. Add descriptive alt text.
5. Keep the order intentional, usually chronological.

## Adding Another Story, Profile, Video, or Media Article

To add another Featured Stories & Media card:

1. Save a local thumbnail into `assets/media/`.
2. Add a new card inside the `#featured-stories` section in `index.html`.
3. Link the full card to the original external URL.
4. Use:

```html
target="_blank" rel="noopener noreferrer"
```

5. Add:

- a source label
- a concise title
- a short description
- a short action label such as `Read article` or `Watch video`

## Updating the Website Later

For normal content or design changes:

1. Edit the files in this folder.
2. Preview locally with `python3 -m http.server 8000`.
3. Commit the changes:

```bash
git add index.html styles.css script.js README.md assets
git commit -m "Update website content"
```

4. Push the changes:

```bash
git push origin main
```

5. Wait a minute or two for GitHub Pages to refresh the live site.

## Why `.gitignore` Is Included

The `.gitignore` file keeps local-only source files out of the published repository:

- `CV Nethraja.pdf`
- `headshot.JPG`
- `.DS_Store`

The webpage uses copied web-ready files inside `assets/`, so the original source files stay in the project without being published.

## QR Code Stability

The main webpage URL and printed QR code remain unchanged when:

- the CV is updated
- the résumé is updated
- presentation images are replaced
- media thumbnails are replaced
- page content is edited

As long as the site continues to be published at the same URL, the QR code does not need to be reprinted:

```text
https://nethrajak.github.io/
```
