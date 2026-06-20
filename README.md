# rayadastidar.github.io

Personal academic website for Raya Dastidar — astrophysicist researching supernovae,
currently a postdoctoral fellow at INAF (Brera Observatory) and the SOXS team.

## Deploying with GitHub Pages

1. Create a new GitHub repository.
   - For a site at `https://<username>.github.io/`, name the repo exactly `<username>.github.io`.
   - For a project page instead (`https://<username>.github.io/<repo-name>/`), name it anything.
2. Add these two files to the repo root: `index.html` and `style.css`.
3. Commit and push to the `main` branch.
4. In the repo, go to **Settings → Pages**.
5. Under **Build and deployment → Source**, choose **Deploy from a branch**.
6. Under **Branch**, choose `main` and folder `/ (root)`, then **Save**.
7. Wait a minute or two — GitHub will publish the site and show you the live URL at the top of the Pages settings tab.

## Editing content

Everything lives in `index.html` — text, links, and small inline SVG figures (the light curve in
the hero, the schematic diagrams next to each paper). There are no external image files to manage,
so editing is just editing text/markup directly. Visual styling (colors, type, spacing) lives in
`style.css`.

To swap in a real photo or figure instead of an inline SVG, drop the image file into the repo
(e.g. an `assets/` folder) and replace the relevant `<svg>...</svg>` block with an `<img src="assets/yourfile.jpg" alt="...">`.

## Local preview

Any static file server works, e.g. from the repo folder:

```
python3 -m http.server 8000
```

Then open `http://localhost:8000` in a browser.
