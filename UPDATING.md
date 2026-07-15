# How to update this website

You can make every change described here directly on GitHub in your browser —
no software to install. Open the file, click the pencil icon (Edit), make your
change, and click **Commit changes**. The site rebuilds and goes live
automatically about two minutes after every commit to `main`.

## Add a new paper

1. Open `data/papers.yaml`.
2. Copy an existing entry (from `publications:` for published work, or
   `working_papers:` for drafts) and edit the fields:

   ```yaml
   - citation_authors: "**Chen, Lingxiao**"   # ** ** bolds your name
     year: 2027
     title: "Paper Title Here"
     venue: "Journal Name"
     volume_pages: "1(1): 1–20"      # optional
     link: "https://doi.org/..."
     keywords: "keyword one, keyword two"   # optional
     abstract: >-
       One-paragraph abstract.       # optional
   ```

3. Commit. The Research page updates itself.

## Move a working paper to publications

Cut its entry from `working_papers:` and paste it under `publications:`,
then add the `citation_authors`, `year`, `venue`, and `link` fields.

## Update your bio (homepage)

Edit `content/_index.md`. Each paragraph is plain text; links are written
as `[link text](https://example.com)`.

## Update the Research page intro

Edit the paragraph in `content/research.md` (below the `---` block).

## Add or change a teaching entry

Edit `data/teaching.yaml`. Each section has a heading (`section:`) and a
list of items. Add a line like:

```yaml
    - text: "Course Name — Undergraduate, Fall 2027"
```

Use `note: "scheduled"` to show an italic *(scheduled)* tag.

## Update your CV

Replace `static/files/cv.pdf` with the new PDF, **keeping the same
filename** (`cv.pdf`). On GitHub: open `static/files/`, click
**Add file → Upload files**, drop in the new `cv.pdf`, and commit — it
overwrites the old one.

## Change your photo

Replace `static/images/photo.jpg` with a new image, keeping the same
filename. A square image works best; it is displayed in a circular frame.

## Change your email, byline, or social links

Edit the `params:` section at the top of `hugo.yaml`.

## Remove the footer credit or the invisible marker

In `hugo.yaml`, set `credit: false` (footer line) or `discovery: false`
(hidden generator metadata) under `params.mysite`.
