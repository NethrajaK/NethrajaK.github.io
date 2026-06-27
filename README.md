# Nethraja Kandula Personal Webpage

This project is a simple one-page professional portfolio built with plain HTML, CSS, and vanilla JavaScript. It is designed to work well from a QR code on a conference business card and to provide a stable webpage URL for recruiters and collaborators.

## Project Structure

```text
Webpage/
├── .gitignore
├── index.html
├── styles.css
├── script.js
├── assets/
│   ├── nethraja-kandula-cv.pdf
│   └── headshot.JPG
└── README.md
```

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

This site is published at:

```text
https://nethrajak.github.io/
```

The GitHub repository is:

```text
https://github.com/NethrajaK/NethrajaK.github.io
```

## Replacing the CV Later

Keep the public filename exactly the same:

```text
assets/nethraja-kandula-cv.pdf
```

To update the CV:

1. Export the new CV as a PDF.
2. Replace the file at `assets/nethraja-kandula-cv.pdf`.
3. Do not change the filename unless you also update the links in `index.html`.

Using the same filename keeps the webpage buttons, embedded CV section, and QR-linked site working without changing the page address.

## Replacing the Headshot

The webpage currently uses:

```text
assets/headshot.JPG
```

To replace it:

1. Prepare the new image.
2. Save it with the same filename and extension, or update the image path in `index.html`.
3. Replace the file inside the `assets/` folder.

## Deploying with GitHub Pages

This project is already set up for GitHub Pages.

Current settings:

```text
Repository: NethrajaK/NethrajaK.github.io
Branch: main
Folder: / (root)
```

If GitHub Pages ever needs to be checked again:

1. Open the repository settings.
2. Go to `Pages`.
3. Make sure the source is `Deploy from a branch`.
4. Make sure the branch is `main` and the folder is `/ (root)`.

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

The `.gitignore` file keeps local-only source files out of the published repo:

- `CV Nethraja.pdf`
- `headshot.JPG`
- `.DS_Store`

The website uses the copied files inside `assets/`, so these original files do not need to be pushed to GitHub.

## Why the QR Code Should Point to the Webpage Instead of the CV

Pointing the QR code to the webpage is better than linking directly to the PDF because:

- The webpage presents a stronger professional first impression.
- Recruiters can immediately see contact details, expertise, and profile links.
- The CV can still be viewed or downloaded from the page.
- The page can be updated over time without changing the QR code destination.
- The webpage works as a central profile, while the CV remains one supporting document.
