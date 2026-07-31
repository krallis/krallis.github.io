# krallis.github.io

Personal academic website of Konstantinos Rallis. Built on [al-folio](https://github.com/alshedivat/al-folio), a Jekyll theme for academic sites.

## Structure

- `_pages/about.md` — home page (bio, profile info)
- `_pages/publications.md` — renders `_bibliography/papers.bib`
- `_pages/cv.md` — renders `_data/cv.yml`
- `_data/socials.yml` — contact/social links, CV PDF path
- `_config.yml` — site-wide settings (name, description, social handles)
- `assets/pdf/CV.pdf` — CV file linked from the nav and CV page

## Local development

```bash
bundle install
bundle exec jekyll serve
```

Site builds at `http://localhost:4000`.

## Deploy

Pushing to `master` triggers `.github/workflows/deploy.yml`, which builds the site and pushes the output to the `gh-pages` branch. In the repo's **Settings → Pages**, set the source to deploy from the `gh-pages` branch.
