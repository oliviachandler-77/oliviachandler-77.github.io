# Olivia Chandler — Portfolio

A static Jekyll portfolio for GitHub Pages. The pages are written in Markdown, with shared layout and styling kept separate.

## Update the site

- Edit `index.md`, `about.md`, `experience.md`, and `contact.md` to update page content.
- Replace bracketed notes such as `[Add a personal bio…]` with your own details, or remove them.
- Change navigation or repeated site details in `_includes/`.
- Adjust colors and responsive styles in `assets/css/site.css`.
- Update the GitHub username in `_config.yml`, `robots.txt`, and the GitHub links if it changes.
- The email link is public by design. The résumé phone number is not included.

## Preview and build locally

Install Ruby and Bundler, then run:

```sh
gem install bundler
bundle install
bundle exec jekyll serve
```

Open the local address printed by Jekyll. To create a production build locally:

```sh
bundle exec jekyll build
```

The generated site is written to `_site/`; do not edit generated files directly.

## Publish with GitHub Pages

1. Push this site to the `main` branch of the `oliviachandler-77.github.io` repository.
2. In the repository’s **Settings → Pages**, choose **Deploy from a branch**, select `main`, and select `/(root)`.
3. Save the setting. GitHub Pages builds the Jekyll source automatically; no separate build or output-folder upload is required.

The site is configured as a GitHub user site: `url` is `https://oliviachandler-77.github.io` and `baseurl` is empty.

## Run Lighthouse

After starting the local preview, open it in Chrome. Open Developer Tools → **Lighthouse**, select Performance, Accessibility, Best Practices, and SEO, then run the audit for both mobile and desktop. Check the page at 375px and 1280px viewport widths in responsive design mode.

The layout uses semantic HTML, a keyboard skip link, visible focus styles, responsive spacing, and reduced-motion support. Lighthouse scores should be measured against the built site rather than assumed.
