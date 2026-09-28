# tharcisse.github.io

Tharcisse's personal website, built with Jekyll and published through GitHub Pages.

## Local preview

Use Ruby 3.3.5 (see `.ruby-version`) and Bundler 4.0.16:

```sh
gem install bundler -v 4.0.16
bundle install
bundle exec jekyll serve
```

Open <http://localhost:4000>. To check a production build, run `bundle exec jekyll build --trace`.

## Deploy to GitHub Pages

1. Push this repository to `tharcissentirandekura/tharcisse.github.io` on `main` or `master`.
2. In the repository's **Settings → Pages → Build and deployment**, choose **GitHub Actions**.
3. The **Deploy Jekyll site to Pages** workflow builds and deploys the site. It can also be run manually from **Actions**.

The site URL is <https://tharcissentirandekura.github.io/tharcisse.github.io/>. The daily workflow uses the same deployment workflow and requires no personal access token.

## Content

- `_config.yml`: name, tagline, profile link, and site URL.
- `about/index.md` and `research/index.md`: biography and research content.
- `_layouts/home.html`: homepage introduction; preserve its markup and styles when editing copy.
- `news.md`: homepage updates.
- `_posts/`: new posts, with `category: life`, `notebook`, or `projects`.
- `assets/profile.svg`: provisional initial avatar; replace with a personal image when available.

The inherited author's posts remain in their original folders but are excluded from the published site. Their publications, account integrations, and verification files are not presented as Tharcisse's work.

## Attribution

Adapted from [Lj V. Miranda's website](https://github.com/ljvmiranda921/ljvmiranda921.github.io). The original design and source content are credited to Lester James V. Miranda under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/). This adaptation changes personal content and deployment configuration while preserving the layout.
