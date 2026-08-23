# Yu Zhu Academic CV

Academic personal website for Yu Zhu, built with the
[HugoBlox Academic CV](https://github.com/HugoBlox/hugo-theme-academic-cv)
template and deployed with GitHub Pages.

## Preview

The project-site URL is:

https://zeheru.github.io/yuzhu-academic-cv/

## Local development

The template currently targets Hugo Extended 0.162.0, Node.js 22, and pnpm
10.14.0.

1. Install Hugo Extended, Node.js, pnpm, and Go.
2. Run pnpm install --frozen-lockfile.
3. Run pnpm dev.
4. Open http://localhost:1313/.

For a production build, run pnpm build. Generated files are written to
public/ and are not committed.

The local build includes a small compatibility override for Hugo 0.162 in
layouts/_partials/functions/build_links.html. It initializes Hugo's scratch map
before HugoBlox collects publication and project links.

## Content

- Profile, education, experience, skills, and awards: data/authors/me.yaml
- Homepage: content/_index.md
- Publications: content/publications/
- Projects: content/projects/
- CV source: cv/cv.tex
- Downloadable CV: static/uploads/cv.pdf

To rebuild the PDF CV, run XeLaTeX on cv/cv.tex, copy the resulting PDF to
static/uploads/cv.pdf, and mirror it at static/files/cv.pdf for the legacy URL.
The public PDF intentionally omits the phone number and reference contacts that
were present in the previous version.

Publication records were checked against publisher, arXiv, and CVF metadata
during migration. The original Academic Pages website remains unchanged.
The canonical BibTeX file is publications.bib; the import workflow is manual so
that generated publication pages can be reviewed before they are replaced.

## Deployment

The repository includes the official HugoBlox GitHub Pages build and deploy
workflows. In GitHub, set Settings → Pages → Source to GitHub Actions.

## License

The HugoBlox template is available under the MIT License. Personal content
and publications remain the property of their respective authors and
publishers.
