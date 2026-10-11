# Ilya Shynkevich · Portfolio

Personal resume site: intro, projects, experience, education, certificates and contact.

Static site with no build step and no dependencies: `index.html`, a favicon and the `img/` folder.

## Updating

- **Projects:** each card is an `<article class="card">` in `index.html`. Its image is set in the `SHOTS` object in the script at the bottom. A list of images becomes a gallery.
- **Live previews:** a card whose image is an `<a class="shot live">` opens that URL when clicked.
- **Certificates:** copy a row in the Certifications section, add the image to `img/`, and register it in `SHOTS` (e.g. `SHOTS["cert-aws"] = "img/cert-aws.jpg";`).
- **Profile picture:** `PHOTO_A` is shown by default and `PHOTO_B` on hover.

## Run locally

Open `index.html` in a browser, or run `python -m http.server 8000` in this folder.

## Deploy

Deployed on Vercel: Application Preset `Other`, no build command, no output directory, no environment variables. Every push to `main` redeploys.
