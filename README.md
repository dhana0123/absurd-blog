# Absurd Fictional Blog

Plain HTML blog for GitHub Pages. No build step.

## Write a post
1. Copy `posts/_template.html` to `posts/my-post.html`.
2. Edit the title, date and body.
3. Add an `<li>` at the top of the sidebar list in `index.html`, copying the existing one and changing `href`, `data-slug` (file name without `.html`), the title and the date.

## Deploy
1. Create a GitHub repo named `<your-username>.github.io` (public).
2. Push this folder:
   ```
   git init
   git add .
   git commit -m "first post"
   git branch -M main
   git remote add origin https://github.com/<your-username>/<your-username>.github.io.git
   git push -u origin main
   ```
3. In the repo, open Settings > Pages, set Source to "Deploy from a branch", branch `main`, folder `/ (root)`.
4. Your blog goes live at `https://<your-username>.github.io`.

Every later `git push` updates the site.
