# Nethraja Kandula Personal Webpage

This project is a simple one-page professional portfolio built with plain HTML, CSS, and vanilla JavaScript. It is designed to work well from a QR code on a conference business card and to provide a stable webpage URL for recruiters and collaborators.

## Project Structure

```text
Webpage/
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

1. Create a GitHub repository and upload this folder.
2. Commit and push the files to the default branch, usually `main`.
3. In the repository settings, open `Pages`.
4. Set the source to deploy from the default branch root.
5. Save the setting and wait for GitHub Pages to publish the site.
6. Use the published webpage URL in the QR code on the business card.

The URL will typically look like:

```text
https://your-username.github.io/repository-name/
```

## Why the QR Code Should Point to the Webpage Instead of the CV

Pointing the QR code to the webpage is better than linking directly to the PDF because:

- The webpage presents a stronger professional first impression.
- Recruiters can immediately see contact details, expertise, and profile links.
- The CV can still be viewed or downloaded from the page.
- The page can be updated over time without changing the QR code destination.
- The webpage works as a central profile, while the CV remains one supporting document.
