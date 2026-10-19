# Website

Minimal Jekyll site for GitHub Pages: one full-screen scrolling page built on the
look of the [fullit](https://github.com/fullit/fullit.github.io) theme (MIT), using fullPage.js.

## Editing content

- Site title / tagline: `_config.yml`
- Scroll sections: `_sections/*.md`, one file per section, ordered by `order:`.
  Front matter sets `heading`, `subheading`, and `background` (an image filename
  that must exist in both `assets/img/big/` (landscape) and `assets/img/tablet/` (portrait)).
  The body text becomes the highlighted line under the subheading.

## Local preview

```sh
export PATH=/opt/homebrew/opt/ruby/bin:$PATH   # use Homebrew Ruby, not system Ruby 2.6
bundle install                                  # first time only
bundle exec jekyll serve --livereload
```

Then open http://localhost:4000.

Live site: https://maxonzorro.com (GitHub Pages builds from `main` on every push).
