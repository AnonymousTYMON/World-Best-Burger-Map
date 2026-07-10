# Contributing to Burger 101

Thanks for wanting to help improve the map! This is a small, single-file static project, so contributing is easy.

## Ways to contribute

- **Fix a pin location** — if a restaurant's marker is in the wrong spot, update its `lat, lng` in the `R` array.
- **Add or update a restaurant** — add a new row to the `R` array (see [README.md](README.md#-data) for the format).
- **Report a bug** — open an issue describing what happened, what you expected, and your browser/OS.
- **Improve the UI/UX** — search, filters, popups, mobile layout, accessibility, etc.

## Making a change

1. Fork the repo and clone your fork.
2. Open `worlds-best-burgers-map.html` directly in your browser, or serve it locally:
   ```bash
   python3 -m http.server 8000
   ```
3. Make your changes. There's no build step — it's vanilla HTML/CSS/JS.
4. Test in both desktop and mobile viewport sizes.
5. Commit with a clear message and open a pull request describing what changed and why.

## Data changes

When editing the `R` array:

- Keep entries in rank order.
- Use the official listing at [worldbestburgers.com](https://www.worldbestburgers.com/our-list) as the source of truth for rank, name, and city.
- Coordinates should point to the neighbourhood/city level; exact street addresses aren't required since every popup links out to Google Maps directions.
- Double-check the Instagram handle field (no `@`, just the handle).

## Code style

- No frameworks, no build tools — keep it a single self-contained HTML file.
- Match the existing formatting and CSS variable naming (`--gold`, `--tomato`, `--cream`, etc.).
- Keep new dependencies to CDN-hosted libraries only, and note them in the README's tech stack table if added.

## Questions

Open an issue and tag it `question` — happy to help.
