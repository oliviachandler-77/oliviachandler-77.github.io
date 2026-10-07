# Olivia Chandler Portfolio

This is a static Jekyll portfolio designed to publish as the GitHub user site
`oliviachandler-77.github.io`.

## Site structure

- `index.md` — home page
- `about.md` — personal introduction, education, and career direction
- `experience.md` — Rue Gilt Groupe internship and Salesforce chronology:
  Sales Intern (summers 2018 and 2019), Sales Development, Business Development,
  Senior Business Development, and Account Executive roles in Small Business,
  Growth Business, and Mid-Market (June 2018–June 2025 overall), with AI
  integration highlights
- `contact.md` — public email contact page
- `_layouts/default.html` — shared document shell
- `_includes/header.html` and `_includes/footer.html` — shared navigation and footer
- `assets/css/style.css` — site styling
- `assets/favicon.svg` — browser favicon
- `_config.yml` — Jekyll and GitHub Pages settings

## Update the content

1. Open the Markdown page you want to edit.
2. Keep the YAML front matter between the opening and closing `---` lines.
3. Add or update work experience using only details Olivia has supplied; do not
   add unverified responsibilities, outcomes, or achievements.
4. Keep content in the Markdown pages and presentation rules in
   `assets/css/style.css`.

The About and experience pages use details from Olivia Chandler's supplied
resume and details she has provided directly. No additional achievements,
employers, clients, metrics, or projects are assumed.

## Publish with GitHub Pages

1. Create or use the repository named `oliviachandler-77.github.io`.
2. Commit this repository to the `main` branch.
3. In GitHub, open **Settings → Pages**.
4. Set the source to **Deploy from a branch**, choose `main`, and choose
   `/(root)`.
5. Save and wait for the Pages build to finish.

The site is already configured as a user site: `baseurl` is empty and links use
Jekyll's `relative_url` filter.

## Preview locally

Install Ruby and Bundler. From the repository root, install the GitHub Pages
dependencies pinned in `Gemfile.lock`:

```sh
bundle install
```

Build the site and fail on invalid front matter or rendering errors:

```sh
bundle exec jekyll build --strict_front_matter
```

The generated static site is written to `_site/`. Run this before publishing
to check all Markdown pages, layouts, and includes. Commit `Gemfile.lock` so
local builds use the same dependency versions.

To preview locally with live reload, run:

```sh
bundle exec jekyll serve --livereload
```

Open the local address printed by Jekyll.

## Lighthouse

After the site is published, open the public URL in Chrome, open DevTools, go
to the **Lighthouse** tab, select **Performance**, **Accessibility**, **Best
Practices**, and **SEO**, then run the audit for both mobile and desktop.

The site avoids external trackers, heavy libraries, and remote font requests to
keep the pages fast and privacy-friendly.