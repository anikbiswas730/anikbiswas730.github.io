# Anik Biswas — Portfolio

A clean, static personal portfolio site. Plain HTML/CSS/JS — no build step, so it hosts directly on GitHub Pages.

## Pages

- `index.html` — Home
- `updates.html` — Updates (a running news/milestones log)
- `experience.html` — Professional experience, research experience, education, awards
- `projects.html` — Selected deep learning and hardware projects
- `publications.html` — Journal articles and conference papers
- `hobbies.html` — Placeholder page (see note below)

Shared styles live in `assets/css/style.css`, and the nav/dropdown behavior in `assets/js/main.js`.

## Before you publish

1. **Hobbies page**: your CV didn't include hobbies, so `hobbies.html` currently has placeholder cards. Open the file and swap in the real content.
2. **ResearchGate link**: the footer's ResearchGate link is a placeholder (`href="#"`) since I couldn't confirm which ResearchGate profile is yours. Replace it in every page's footer once you have the URL — a quick find-and-replace for `href="#" target="_blank" rel="noopener">ResearchGate` will catch all six.
3. **Project links**: the "View on GitHub" links on the Projects page currently point to your GitHub profile (`github.com/anikbiswas730`). Swap each one for the specific repo link once your project repos are public.
4. **Portfolio domain**: if you'd like a custom domain instead of the default `username.github.io` address, add a `CNAME` file at the root once you've got one.

## Hosting on GitHub Pages

1. Create a new repository on GitHub — for a root-level site named `<username>.github.io`, or any name for a project site.
2. Push these files to the repository's default branch (e.g. `main`):
   ```bash
   git init
   git add .
   git commit -m "Initial portfolio site"
   git branch -M main
   git remote add origin https://github.com/<username>/<repo-name>.git
   git push -u origin main
   ```
3. On GitHub, go to the repository's **Settings → Pages**.
4. Under **Build and deployment**, set **Source** to "Deploy from a branch," pick the `main` branch and the `/ (root)` folder, then save.
5. GitHub will publish the site at `https://<username>.github.io/` (if the repo is named `<username>.github.io`) or `https://<username>.github.io/<repo-name>/` otherwise. It can take a minute or two for the first deploy to go live.

## Local preview

Just open `index.html` in a browser, or serve the folder locally:
```bash
python3 -m http.server 8000
```
then visit `http://localhost:8000`.
