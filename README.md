# BHA_AI_Strategy

Static executive briefing page for the BHA technology and AI strategy proof of concept.

## Current POC State

- The candidate skills comparison now uses a local static SVG image instead of a live Chart.js canvas.
- The page is still a single HTML file with inline JavaScript for the roadmap and infrastructure toggles.
- The page can be hosted on GitHub Pages and embedded into a modern SharePoint page with the Embed web part.

## Files

- `index.html`: Main briefing page.
- `assets/skills-radar-chart.svg`: Static radar chart used in the candidate profile section.

## Publish To GitHub Pages

1. Push this repository to GitHub.
2. In the GitHub repository, open `Settings` -> `Pages`.
3. Under `Build and deployment`, set `Source` to `Deploy from a branch`.
4. Choose your default branch and `/ (root)`.
5. Save the settings and wait for GitHub Pages to publish the site.
6. Open the published URL and confirm the page renders correctly.

Typical URL format:

```text
https://<github-user>.github.io/<repository-name>/
```

## Embed In SharePoint

1. Edit the modern SharePoint page.
2. Add the `Embed` web part.
3. Paste the GitHub Pages URL for this site.
4. Resize the web part until the full page content is readable.
5. Publish the SharePoint page.

## Notes

- If the tenant blocks external embedding, move the same static files to an approved internal host.
- The remaining external runtime dependency is Tailwind via CDN. If the tenant network policy blocks it, the next hardening step is to replace those classes with local CSS.
