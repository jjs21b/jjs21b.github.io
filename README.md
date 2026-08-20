# Jack Schwartz Portfolio

This folder is a complete static portfolio website prepared for GitHub Pages. It does not require Node.js, React, a build command, or a hosting service.

## Recommended publishing method

1. Create a new public GitHub repository named `jjs21b.github.io`.
2. Upload the contents of this folder to the repository root. Upload `index.html`, `styles.css`, `.nojekyll`, `README.md`, and the `assets` folder directly rather than uploading the containing folder.
3. Open the repository's **Settings** page.
4. Select **Pages** under **Code and automation**.
5. Under **Build and deployment**, select **Deploy from a branch**.
6. Select the `main` branch and the `/(root)` folder, then click **Save**.
7. After GitHub finishes the deployment, the portfolio will be available at `https://jjs21b.github.io/`.

GitHub notes that publishing can take up to 10 minutes after a push.

## Publishing from the command line

Run these commands from inside this unzipped folder after creating the empty `jjs21b.github.io` repository:

```bash
git init
git add .
git commit -m "Publish portfolio"
git branch -M main
git remote add origin https://github.com/jjs21b/jjs21b.github.io.git
git push -u origin main
```

Then configure **Settings > Pages > Deploy from a branch > main > /(root)**.

## Updating the portfolio

Edit `index.html` for project text or links, edit `styles.css` for the design, and replace files in `assets` when images, the résumé, or reports change. Commit and push the changes to `main`; GitHub Pages will publish the update automatically.

## If `jjs21b.github.io` already exists

Use a repository such as `portfolio` instead. The resulting address will be `https://jjs21b.github.io/portfolio/`. Because this package uses relative paths, the site itself will work there, but update the `og:url` and `og:image` values near the top of `index.html` to include `/portfolio/`.

