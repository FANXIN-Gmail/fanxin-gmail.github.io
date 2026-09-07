# Xin Fan — Academic Homepage

An English academic homepage, published at https://fanxin-gmail.github.io/.

This is a static site: no framework, package installation, JavaScript, or build step is required. GitHub Pages publishes the root of the `main` branch; `.nojekyll` disables Jekyll processing.

## Update the homepage

- **Biography and contact links:** edit the `BIO` section in `index.html`.
- **Selected Publications:** edit the `PUBLICATIONS` section. This curated list includes first-author, equal-contribution, and collaborative papers. Duplicate an `<article>` block for a new paper, give it unique IDs, preserve the published author order, and bold Xin Fan. Keep `* Equal contribution` and all relevant author markers together.
- **Paper resources:** link to public publisher pages, DOIs, arXiv, or public project repositories. Label an overview/data repository `Project`; use `Code` only for an available implementation. Omit resources that are not public; do not upload unpublished drafts.
- **Publication status:** keep acceptance separate from publication. RADS-PDD has a 2027 volume year and July 16, 2026 online publication date; DAD-PDD appeared at ICONIP 2025 and was published in 2026.
- **Photo:** the homepage currently uses a 3:4 placeholder. To add a photo, save it as `assets/xin-fan.jpg` and replace the `portrait-placeholder` div in the `PHOTO` section with `<img src="assets/xin-fan.jpg" alt="Portrait of Xin Fan" width="3000" height="4000" fetchpriority="high">`. Set `width` and `height` to the new image’s actual pixel dimensions; the layout preserves its original proportions.
- **Figures:** store them in `assets/`, add meaningful alt text and intrinsic dimensions, and preserve their aspect ratio. The images link to their full-size versions. Use `publication text-only` for a paper without a figure.
- **Education, experience, and funding:** edit the corresponding sections of `index.html`. Update the footer date after substantive changes.
- **Appearance:** edit `stylesheet.css`; the single-column mobile layout begins at 700px.

Preview locally from this directory:

```sh
python3 -m http.server 8000 --bind 127.0.0.1
```

Open http://127.0.0.1:8000/. Commit and push changes to `main` to publish. Check the GitHub Pages deployment under the repository's Actions tab and Settings → Pages.

## Content and attribution

- Profile, education, experience, funding, and bibliographic details were drawn from the owner's confirmed records, with the three collaborative papers' supplied PDFs checked on September 7, 2026. Only homepage content and assets belong in this repository.
- The MTRB-QTA equal-contribution marks for Yuxiang Zhang, Xin Fan, and Junjie Wang were verified against the published paper's first page.
- The GateBoxGCN author list and RecSys 2026 acceptance were checked against the [ZOZO NEXT announcement](https://zozonext.com/news/20260903_zozoresearch). Its public repository contains an implementation and is labeled `Code`. The supplied PDF is an anonymous submission with placeholder publication metadata; it is used only as a figure source, not as evidence of final authorship, DOI, or publication. The two collaborative journal papers' author order, titles, volumes, article numbers, and years were checked against their supplied published PDFs and link to their publisher DOIs: [Pattern Recognition](https://doi.org/10.1016/j.patcog.2025.111829) and [Neurocomputing](https://doi.org/10.1016/j.neucom.2023.127140). All seven selected entries now include figures that link to their full-size versions.
- The layout is independently implemented, inspired by [Tsunehiko Tanaka](https://tsunehiko.github.io/) and [Jon Barron](https://jonbarron.info/).
- `assets/pirbd-pdd.png` is Figure 2 (method overview) extracted from the author's supplied PIRBD-PDD manuscript. The paper is accepted to EMNLP 2026; the manuscript itself is not distributed here. Figure rights remain with the authors.
- `assets/rads-pdd.png` reproduces a figure from [RADS-PDD](https://doi.org/10.1016/j.neunet.2026.109393), © 2026 The Authors, published by Elsevier under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/).
- `assets/dad-pdd.png` reproduces the architecture figure from [DAD-PDD](https://doi.org/10.1007/978-981-95-4091-4_7). Rights remain with the authors and Springer Nature.
- `assets/mtrb-qta.jpg` reproduces the framework figure from [MTRB-QTA](https://doi.org/10.1145/3673791.3698429). Rights remain with the respective copyright holders; see the [public paper](https://arxiv.org/abs/2410.03212).
- `assets/gateboxgcn.png` is Figure 1 (architecture), extracted from page 3 of the owner's supplied GateBoxGCN submission. The manuscript itself is not distributed here. Figure rights remain with the respective copyright holders.
- `assets/synergistic-fusion.png` is Figure 2 (training framework), extracted from page 4 of [Synergistic fusion framework](https://doi.org/10.1016/j.patcog.2025.111829), Pattern Recognition 167 (2025), 111829. © 2025 Elsevier Ltd.; rights remain with the respective copyright holders.
- `assets/sedc-gcn.png` is Figure 2 (overall architecture), extracted from page 5 of [Sampling-based epoch differentiation calibrated graph convolution network for point-of-interest recommendation](https://doi.org/10.1016/j.neucom.2023.127140), Neurocomputing 571 (2024), 127140. © 2023 Elsevier B.V.; rights remain with the respective copyright holders.
- The portrait is currently omitted from the homepage and deployed assets. No blanket license is granted for third-party figures.
