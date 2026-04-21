# blog

Personal blog — **Yiğit's Notes** → [ertodebana.github.io/blog](https://ertodebana.github.io/blog/).

Built with [Hugo](https://gohugo.io/) and the [PaperMod](https://github.com/adityatelange/hugo-PaperMod) theme, deployed to GitHub Pages via GitHub Actions. Styled with a red / black / white palette.

## Local development

```bash
git clone --recurse-submodules https://github.com/ertodebana/blog.git
cd blog
hugo server -D
```

Site available at <http://localhost:1313>.

## Writing a post

```bash
hugo new content posts/my-new-post/index.md
```

Add `tags` and `categories` in the front matter so it shows up under [/tags/](https://ertodebana.github.io/blog/tags/) and [/categories/](https://ertodebana.github.io/blog/categories/). Commit and push — GitHub Actions deploys automatically.

## Structure

- `content/` — pages and posts
- `hugo.yaml` — site config
- `assets/css/extended/custom.css` — red/black/white theme overrides
- `themes/PaperMod/` — theme (git submodule, pinned to v8.0)
- `.github/workflows/hugo.yml` — deploy workflow
