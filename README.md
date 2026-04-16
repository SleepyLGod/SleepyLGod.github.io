# [SleepyLGod.github.io](https://sleepylgod.github.io/)

Personal website for [LU HAODONG](https://sleepylgod.github.io/), built with Jekyll and deployed on GitHub Pages.

```bash
gem install --user-install bundler -v 2.3.26
export PATH="$HOME/.gem/ruby/2.6.0/bin:$PATH"

BUNDLE_PATH=vendor/bundle bundle _2.3.26_ install
BUNDLE_PATH=vendor/bundle bundle _2.3.26_ exec jekyll build
BUNDLE_PATH=vendor/bundle bundle _2.3.26_ exec jekyll serve --config _config.yml,_config.dev.yml
```

The first `bundle install` needs network access to download gems. After that, the site should be available at `http://127.0.0.1:4000/`.
