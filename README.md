# Nasseb Marbles Website

A responsive static website for Nasseb Marbles. The site uses only HTML, CSS, and local image assets, so it is ready for GitHub Pages deployment.

## GitHub Pages deployment

1. Create a GitHub repository and push this project folder.
2. Open **Settings → Pages** in the repository.
3. Select **Deploy from a branch**.
4. Choose the `main` branch and the `/` folder.
5. Save the settings and open the generated GitHub Pages URL.

## Image path fix

All image files are stored in the project root and referenced directly, for example `mandir.jpeg` and `gurudwara.jpeg`. This keeps GitHub Pages deployment simple and avoids broken links.

## Local preview

Open `index.html` directly in a browser, or run a local server from the project folder:

```powershell
python -m http.server 8000
```

Then visit `http://localhost:8000`.
