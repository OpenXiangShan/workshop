# ADVC 2026 Website

This website uses [Jekyll](https://jekyllrb.com/) and deploys directly through GitHub Pages. The local Gemfile pins the same GitHub Pages build stack so local preview matches the published site more closely.

## Updating content

- Update dates, venue, topics, organizers, and the contact email in `_data/workshop.yml`.
- Update page content in `index.md`, `cfp.md`, `program.md`, and `organizers.md`.
- Update the shared navigation and footer in `_includes/`.
- Update site-wide presentation in `assets/css/site.css`.

## Local preview

Install Ruby and Bundler, then run:

```bash
bundle install
bundle exec jekyll serve
```

The site will be available at `http://localhost:4000`.

## GitHub Pages deployment

1. Update `url` in `_config.yml` to your custom domain and keep `baseurl` empty when using a root-mapped custom domain.
2. Push the repository to GitHub.
3. Add a `CNAME` file at the repository root with your custom domain.
4. In **Settings → Pages**, set **Source** to **Deploy from a branch**, select `main`, and select `/(root)`.

GitHub Pages builds Jekyll automatically after each push to `main`.
