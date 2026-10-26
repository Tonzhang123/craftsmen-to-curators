# From Craftsmen to Curators — Paper Analysis Site

An interactive, single-page analysis of the paper:

> **From Craftsmen to Curators: Navigating Cognitive Friction in Generative AI Filmmaking Education**
> T. Zhang, X. Xu, X. Feng, S. Hou, H. Li, and A. Rao.
> *IEEE Transactions on Learning Technologies*, 2026. DOI: [10.1109/TLT.2026.3739765](https://doi.org/10.1109/TLT.2026.3739765)

## What this is
A self-contained, dependency-free HTML website (no build step, no CDN) that visualizes the paper's
key findings: cognitive friction, the "curatorial shift" (craftsmen → curators of probabilities),
the inverted traversal of the Revised Bloom's Taxonomy, and the assessment paradox in GenAI
filmmaking education.

## View locally
Just open `index.html` in any browser — no server required.

## Deploy to GitHub Pages
1. Push this folder to a GitHub repository:
   ```bash
   git remote add origin https://github.com/<your-username>/<repo-name>.git
   git branch -M main
   git push -u origin main
   ```
2. **Make the repository public.** GitHub Pages is only available for *private* repos on paid plans
   (Pro / Team / Enterprise). On the Free plan the repo must be public.
   `Settings → General → Danger Zone → Change repository visibility → Make public`
   (or click the `Private` badge next to the repo name).
3. Enable Pages: `Settings → Pages → Build and deployment → Source: Deploy from a branch →
   Branch: main → Folder: /(root) → Save`.
4. Wait ~1 minute. Your site is live at `https://<your-username>.github.io/<repo-name>/`

> A `.nojekyll` file is included so the site is served exactly as written, with no Jekyll processing.
> Note: a published GitHub Pages site is **public to the internet** even if the repo is private.

## Notes
- The 11 student films are shown as thumbnail cards that open on YouTube — the channel disables
  inline embedding (error 153), so direct `<iframe>` players cannot be used.
- Everything is in a single `index.html`; there is no build step and no external dependency.

## Disclaimer
Independent, non-commercial study visualization. Not affiliated with the authors or IEEE.
All figures and statistics are reproduced from the source manuscript.
