# mzyy1001.github.io

Personal homepage for **Hongrui Chen** (Imperial College London).

Lives at: <https://mzyy1001.github.io>

## What this is

A minimal static site — HTML, CSS, and manuscript preview assets:

| File | What it does |
|---|---|
| `index.html` | All page content (about, research interests, projects, contact). |
| `style.css`  | Layout + typography. Mobile-friendly and supports light/dark mode via `prefers-color-scheme`. |
| `README.md`  | This file. |
| `assets/` | Paper figures (MPI framework from the manuscript’s Figure 1). |

No build step, no Jekyll, no JavaScript framework. GitHub Pages serves the
files as-is.

## Editing

To change content (e.g. add a project, update the bio): open `index.html`,
edit the relevant `<section>` block, save, commit, push. The live site
updates within a minute or two.

To change layout/colors: edit `style.css`. The CSS variables at the top of
the file (`--accent`, `--max-width`, etc.) cover the most common tweaks
without hunting through rules.

## Local preview

Any static file server works. From this directory:

```bash
python3 -m http.server 8000
# then open http://localhost:8000
```

## Enabling GitHub Pages (one-time)

After this repo (`mzyy1001/mzyy1001.github.io`) exists on GitHub:

1. Push to the `main` branch.
2. Go to **Settings → Pages**.
3. Under *Source*, choose **Deploy from a branch**, branch **main**, folder **/ (root)**, then **Save**.
4. Wait ~1 minute. The site will be live at `https://mzyy1001.github.io`.

For a user/organization page named `<username>.github.io`, GitHub Pages
serves automatically from the default branch — no `gh-pages` branch
needed.
