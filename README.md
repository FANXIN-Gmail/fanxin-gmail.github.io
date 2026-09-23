# Xin Fan — Academic Homepage

An English academic homepage, published at https://fanxin-gmail.github.io/.

This is a static site: no framework, package installation, JavaScript, or build step is required. GitHub Pages publishes the root of the `main` branch; `.nojekyll` disables Jekyll processing.

## Update the homepage

- **Biography and contact links:** edit the `BIO` section in `index.html`.
- **Research summary:** keep a concise PhD introduction with graduate school, laboratory, and supervisor, followed by past research, ongoing interests, and current research. Bold the current research topics. The September 23, 2026 revision removes the master's-degree sentence and earlier non-LLM research from the introduction.
- **Selected Publications:** edit the `PUBLICATIONS` section. This curated list includes first-author, equal-contribution, and collaborative papers. Duplicate an `<article>` block for a new paper, give it unique IDs, preserve the published author order, and bold Xin Fan. Keep `* Equal contribution` and all relevant author markers together.
- **Paper resources:** link to public publisher pages, DOIs, arXiv, or public project repositories. Label an overview/data repository `Project`; use `Code` only for an available implementation. Omit resources that are not public; do not upload unpublished drafts.
- **Publication format:** after each title, show the complete author list, the full conference or journal name (followed by its established acronym when useful), and month/year. Omit page ranges, volume/series numbers, article numbers, conference-track labels, and separate online/proceedings-publication notes. Use conference event months and journal issue months, with RADS-PDD displayed as July 2026 using its first online publication date, as confirmed by the owner on September 8, 2026. Keep `Accepted / To appear` for accepted papers that have not yet been published. These homepage display rules do not remove bibliographic details from source records or figure attributions.
- **Venue metrics:** show a linked CORE rank for conferences using the stated ICORE edition, and a linked Journal Impact Factor (JIF) with its metric year for journals. These are a current venue-metric snapshot, not the metric at each paper’s publication date. Verify both the value and year from the official portal or publisher. Keep any joint-conference qualification visible; never inherit a parent conference’s rank for a regional conference, workshop, or short paper.
- **Photo:** the homepage temporarily uses the owner's social media profile image, `assets/xin-fan-social.jpg` (640 × 457), at its original aspect ratio. To replace it later, update the `img` in the `PHOTO` section, its descriptive alt text, and its actual pixel dimensions. Keep `fetchpriority="high"` for this image.
- **Figures:** store them in `assets/`, add meaningful alt text and intrinsic dimensions, and preserve their aspect ratio. The images link to their full-size versions. Use `publication text-only` for a paper without a figure.
- **Education, experience, and funding:** edit the corresponding sections of `index.html`. Update the footer date after substantive changes.
- **Appearance:** edit `stylesheet.css`; the single-column mobile layout begins at 700px.
- **Footer:** show only the last-updated date. The owner requested removal of the visible layout-inspiration credit on September 7, 2026; keep that provenance in this maintenance document.

Preview locally from this directory:

```sh
python3 -m http.server 8000 --bind 127.0.0.1
```

Open http://127.0.0.1:8000/. Commit and push changes to `main` to publish. Check the GitHub Pages deployment under the repository's Actions tab and Settings → Pages.

## Content and attribution

- The citation display was simplified at the owner's request on September 7, 2026. Event dates and full names were checked against [EMNLP 2026](https://2026.emnlp.org/), [ICONIP 2025](https://iconip2025.apnns.org/), [RecSys 2026](https://recsys.acm.org/recsys26/), the OpenLVLM-MIA CVF citation below, and [SIGIR-AP 2024](https://www.sigir-ap.org/sigir-ap-2024/). RecSys spans September–October 2026. Journal issue months were checked against the publisher: [Neural Networks issue metadata](https://www.sciencedirect.com/science/article/abs/pii/S0893608026008518), [Pattern Recognition, November 2025](https://www.sciencedirect.com/science/article/abs/pii/S0031320325004893), and [Neurocomputing, February 2024](https://www.sciencedirect.com/science/article/abs/pii/S0925231223012638). On September 8, 2026, the owner corrected RADS-PDD's homepage publication date to July 2026: its first online publication was July 16, 2026, as stated in the supplied article and the [PubMed record](https://pubmed.ncbi.nlm.nih.gov/42480164/). The publisher's January 2027 date describes the assigned issue; it is retained only in formal citation metadata. DAD-PDD's 2026 proceedings year remains a separate source fact.

- Profile, education, experience, funding, and bibliographic details were drawn from the owner's confirmed records, with the three collaborative papers' supplied PDFs checked on September 7, 2026. Only homepage content and assets belong in this repository.
- The MTRB-QTA equal-contribution marks for Yuxiang Zhang, Xin Fan, and Junjie Wang were verified against the published paper's first page.
- The GateBoxGCN author list and RecSys 2026 acceptance were checked against the [ZOZO NEXT announcement](https://zozonext.com/news/20260903_zozoresearch). Its public repository contains an implementation and is labeled `Code`. The supplied PDF is an anonymous submission with placeholder publication metadata; it is used only as a figure source, not as evidence of final authorship, DOI, or publication. The two collaborative journal papers' author order, titles, volumes, article numbers, and years were checked against their supplied published PDFs and link to their publisher DOIs: [Pattern Recognition](https://doi.org/10.1016/j.patcog.2025.111829) and [Neurocomputing](https://doi.org/10.1016/j.neucom.2023.127140). All nine selected entries now include figures that link to their full-size versions.
- The layout is independently implemented, inspired by [Tsunehiko Tanaka](https://tsunehiko.github.io/) and [Jon Barron](https://jonbarron.info/).
- `assets/pirbd-pdd.png` is Figure 2 (method overview) extracted from the author's supplied PIRBD-PDD manuscript. The paper is accepted to EMNLP 2026; the manuscript itself is not distributed here. Figure rights remain with the authors.
- `assets/rads-pdd.png` reproduces a figure from [RADS-PDD](https://doi.org/10.1016/j.neunet.2026.109393), © 2026 The Authors, published by Elsevier under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/).
- `assets/dad-pdd.png` reproduces the architecture figure from [DAD-PDD](https://doi.org/10.1007/978-981-95-4091-4_7). Rights remain with the authors and Springer Nature.
- `assets/mtrb-qta.jpg` reproduces the framework figure from [MTRB-QTA](https://doi.org/10.1145/3673791.3698429). Rights remain with the respective copyright holders; see the [public paper](https://arxiv.org/abs/2410.03212).
- `assets/gateboxgcn.png` is Figure 1 (architecture), extracted from page 3 of the owner's supplied GateBoxGCN submission. The manuscript itself is not distributed here. Figure rights remain with the respective copyright holders.
- `assets/synergistic-fusion.png` is Figure 2 (training framework), extracted from page 4 of [Synergistic fusion framework](https://doi.org/10.1016/j.patcog.2025.111829), Pattern Recognition 167 (2025), 111829. © 2025 Elsevier Ltd.; rights remain with the respective copyright holders.
- `assets/sedc-gcn.png` is Figure 2 (overall architecture), extracted from page 5 of [Sampling-based epoch differentiation calibrated graph convolution network for point-of-interest recommendation](https://doi.org/10.1016/j.neucom.2023.127140), Neurocomputing 571 (2024), 127140. © 2023 Elsevier B.V.; rights remain with the respective copyright holders.
- `assets/openlvlm-mia.png` is Figure 1 (LDA+PCA comparison of member/non-member distributions), extracted from page 6 (proceedings p. 2685) of the owner's supplied published OpenLVLM-MIA paper. Its title, author order, WACV 2026 venue, and pp. 2680–2689 were checked against the [CVF proceedings page](https://openaccess.thecvf.com/content/WACV2026/html/Miyamoto_OpenLVLM-MIA_A_Controlled_Benchmark_Revealing_the_Limits_of_Membership_Inference_WACV_2026_paper.html); [DOI 10.1109/WACV61042.2026.00263](https://doi.org/10.1109/WACV61042.2026.00263) appears on the supplied paper's first page. The author name is rendered as published, `Ryoto Miyamoto`. The [public code repository](https://github.com/yamanalab/openlvlm-mia) includes evaluation code and links to the dataset and model. © 2026 IEEE; rights remain with the respective copyright holders.
- `assets/xin-fan-social.jpg` is an unchanged copy of the owner's supplied `X.jpg`, authorized on September 7, 2026 as the temporary homepage profile image. It is a painting used as a social media avatar, not a photographic portrait. No blanket license is granted for third-party images.

- Added PCC-SQL on September 8, 2026. The title, author order (`Miyamoto Ryoto, Xin Fan, Hayato Yamana`), and AACL-IJCNLP 2026 main-conference acceptance were confirmed by the owner and the supplied acceptance screenshot. The homepage follows its existing display format and shows `Accepted / To appear`; the conference name and November 2026 date were checked against the [official conference website](https://2026.aaclnet.org/). No public paper or implementation URL was supplied, so the entry has no paper/code link.
- `assets/pcc-sql.png` is Figure 2 (architecture and token-level masking example), extracted from page 4 of the owner’s supplied PCC-SQL manuscript. It illustrates the state tracker and policy-aware logit masking. The anonymous draft and acceptance screenshot are not distributed in this repository. Figure rights remain with the authors.

## Venue metrics (verified September 23, 2026)

Conference labels use **ICORE 2026**, the current edition of the former CORE rankings. The source edition is stated above Selected Publications; each label links to its official record. A* is a rank, separate from the author asterisks for equal contribution. The [ICORE requirements](https://portal.core.edu.au/conf-changes/serve_file/icore-addition.pdf/) limit a conference rank to main-track full papers.

| Venue | Displayed metric | Official source / qualification |
|---|---|---|
| EMNLP | CORE Rank: A* | [ICORE record 448](https://portal.core.edu.au/conf-ranks/448/) |
| ICONIP | CORE Rank: B | [ICORE record 1152](https://portal.core.edu.au/conf-ranks/1152/); older editions listed A, but 2021, 2023, and 2026 list B |
| AACL-IJCNLP | CORE Rank: B (IJCNLP) | [ICORE IJCNLP record 1317](https://portal.core.edu.au/conf-ranks/1317/). The [official 2026 event](https://2026.aaclnet.org/) is jointly the 5th AACL and 15th IJCNLP. B refers explicitly to the IJCNLP component, not an independent AACL or joint-title rating. An AACL search returned only NAACL, which is a different conference. |
| RecSys | CORE Rank: A | [ICORE record 28](https://portal.core.edu.au/conf-ranks/28/) |
| WACV | CORE Rank: A | [ICORE record 763](https://portal.core.edu.au/conf-ranks/763/); the portal retains the historical name “IEEE Workshop on Applications of Computer Vision” and links to WACV’s DBLP series |
| SIGIR-AP | CORE: Not listed | [ICORE 2026 SIGIR search](https://portal.core.edu.au/conf-ranks/?search=SIGIR&by=all&source=ICORE2026) returns SIGIR and CHIIR, with no SIGIR-AP entry. Do not apply SIGIR’s A* rank to SIGIR-AP. “Not listed” is a search finding, not an assigned ICORE “Unranked” classification. |
| Neural Networks | Impact Factor: 7.2 (2025) | [Publisher Journal Insights](https://www.sciencedirect.com/journal/neural-networks/about/insights) |
| Pattern Recognition | Impact Factor: 9.1 (2025) | [Publisher Journal Insights](https://www.sciencedirect.com/journal/pattern-recognition/about/insights) |
| Neurocomputing | Impact Factor: 6.7 (2025) | [Publisher Journal Insights](https://www.sciencedirect.com/journal/neurocomputing/about/insights) |

All three publisher pages and their Impact Factor information popovers were checked directly in the browser. They identify the metrics as 2025 Journal Citation Reports (Clarivate Analytics, 2026). Thus **2025 is the JIF year**, while 2026 is the release year. Older indexed publisher pages still show 2024 values (6.3, 7.6, and 6.5); the homepage uses the current verified 2025 values consistently. Do not substitute CiteScore, a different metric, for JIF. Metrics describe venues and do not score the individual papers.
