# ling-xiao-chen.github.io

Personal academic website of **Lingxiao Chen**, PhD Candidate in Sociology at
Emory University — live at <https://ling-xiao-chen.github.io/>.

Built with [Hugo](https://gohugo.io/) and deployed to GitHub Pages by the
workflow in `.github/workflows/deploy.yml` on every push to `main`.

## Structure

| Path | What it is |
|------|------------|
| `content/_index.md` | Homepage bio |
| `content/research.md` | Research page intro |
| `content/teaching.md` | Teaching page shell |
| `content/cv.md` | CV page shell |
| `data/papers.yaml` | Publications and working papers |
| `data/teaching.yaml` | Teaching history |
| `static/files/cv.pdf` | The CV |
| `static/images/photo.jpg` | Profile photo |
| `assets/css/style.css` | All styles |
| `layouts/` | Hugo templates |

## Editing the site

See [UPDATING.md](UPDATING.md) — every routine change (new paper, new CV,
bio edits) is a one-file edit you can make on GitHub in the browser.

## Local preview

```sh
hugo server
```

then open <http://localhost:1313/>.
