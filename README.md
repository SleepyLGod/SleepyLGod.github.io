# [SleepyLGod.github.io](https://sleepylgod.github.io/)

Personal website for [LU HAODONG](https://sleepylgod.github.io/), built with Jekyll and deployed on GitHub Pages.

## Local preview

Install Ruby 2.6.10 (recorded in `.ruby-version`) before running these commands. The user gem path below is specific to Ruby 2.6. Check `ruby -v` before installing Bundler.

```bash
gem install --user-install bundler -v 2.3.26
export PATH="$HOME/.gem/ruby/2.6.0/bin:$PATH"

BUNDLE_PATH=vendor/bundle bundle _2.3.26_ install
BUNDLE_PATH=vendor/bundle bundle _2.3.26_ exec jekyll build
BUNDLE_PATH=vendor/bundle bundle _2.3.26_ exec jekyll serve --config _config.yml,_config.dev.yml
```

The first `bundle install` needs network access to download gems. After that, the site should be available at `http://127.0.0.1:4000/`.

## JavaScript assets

With Node.js and npm installed, run `npm ci --ignore-scripts`, then `npm run build:js`. Commit both source changes and the generated `assets/js/main.min.js`. Jekyll and GitHub Pages serve that bundle directly; they do not run the JavaScript build. `package-lock.json` pins the build dependencies. Use `npm run watch:js` while editing JavaScript.

## Content and archives

The homepage is `_pages/about.md`. Public CV files are `_pages/cv_md_export.html` and `res/cv-pdf.pdf`; profile images live in `images/`. Preserve public asset paths when reorganizing source files.

`_archive/` is excluded from the site build but retained in Git. It contains historical CVs, template pages, sample content, example comments, and upstream documentation. Keep personal documents and photographs intact. The root `LICENSE` records upstream licensing.

## Restore a collection

Teaching, talks, portfolio, and publications are declared in `_config.yml` with `output: false`. Their shared layouts, includes, and styles remain available.

1. Create real entries in `_teaching/`, `_talks/`, `_portfolio/`, or `_publications/`. Examples live in `_archive/sample-teaching/`, `_archive/sample-portfolio/`, `_archive/sample-publications/`, and `_talks/`. Review sample entries before enabling output.
2. Set the selected collection's `output` to `true`.
3. For teaching or portfolio, move the corresponding listing page from `_archive/pages/` to `_pages/`. For talks or publications, replace the existing redirect page with a listing using `layout: archive`, its existing permalink, and a loop over `site.talks` or `site.publications` including `archive-single.html` for each `post`. Remove `redirect_to` and `sitemap: false` when publishing the listing.
4. Add the listing to `_data/navigation.yml` if desired. Build and check the list, detail links, and sitemap before publishing.

The current collection defaults and rendering templates are retained. `_archive/upstream/` contains the original theme guides for optional features.
