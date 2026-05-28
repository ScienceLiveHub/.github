# Science Live

**Turn research into stackable, citable knowledge units — signed nanopublications with CiTO-typed citations on an open, decentralised network.**

> Open source · open governance · your nanopubs outlive Science Live.

---

## What is Science Live?

Science Live is a platform and toolset for publishing scientific claims, citations, and replication outcomes as **nanopublications** — small, signed, semantically-typed RDF units that live on a decentralised network independent of any single hosting platform.

Where current scholarly citation infrastructure (DOIs, OpenCitations, WikiCite) excels at **crediting** prior work, Science Live adds the missing piece: a **citable target** on the publishing side so the *intent* of a citation — *extends, uses-method-in, qualifies, confirms, disputes* — becomes machine-actionable rather than buried in PDF prose.

We support three production paths:

- **Extract** · LLM pipelines turning existing PDFs into typed citation nanopubs (complements [GROBID](https://github.com/kermitt2/grobid), [CEC](https://github.com/opencitations/cec), [GRAPHIA](https://www.graphia.org/), and the wider open-citation extraction community)
- **Author** · a [Zotero plugin](https://github.com/ScienceLiveHub/science-live-platform/tree/main/zotero) so the author of a citing work declares intent at write time
- **Annotate** · an expert reader types citations they find in *someone else's* paper — crowd-sourced citation typing, signed and contestable

All three paths converge on the same atomic, signed, addressable nanopub on the open network.

---

## FORRT replication chains — replication as citable data

Science Live's flagship application is **publishing replication studies as citable chains**, following the [FORRT framework](https://forrt.org) ([Röseler et al. 2025](https://doi.org/10.5281/zenodo.16990114)). Each paper-rooted replication produces a six-step chain — **Quote-with-comment → AIDA → FORRT Claim → Replication Study → Replication Outcome → CiTO Citation** — where every step is a separately signed nanopublication with its own URI. An apex **Research Synthesis** nanopub wraps the chain into a single citable target.

The result: a future paper can cite a *specific Outcome*, a *specific Study design*, or the *specific Quote* that anchored the chain — not just the replication paper as a whole. Replication becomes machine-actionable data, and the trust gradient (LLM-extracted → Reader-annotated → Author-validated → FORRT-replicated) becomes explicit and click-resolvable.

The [**`forrt-replication-template`**](https://github.com/ScienceLiveHub/forrt-replication-template) is a self-contained GitHub template that turns this pattern into a working scaffold: clone the template, drop in a paper PDF, and get a Zenodo-archived release plus the full signed nanopublication chain on the open network. Domain-portable via a `DOMAIN.md` swap — currently shipped with a biodiversity + Earth-observation default flavour, adaptable to other computational-reproducibility-based fields.

---

## Core repositories

| Repo | Purpose |
|---|---|
| [**science-live-platform**](https://github.com/ScienceLiveHub/science-live-platform) | Platform monorepo — web app, API, Zotero plugin, viewer/embed components |
| [**forrt-replication-template**](https://github.com/ScienceLiveHub/forrt-replication-template) | Self-contained GitHub template for paper-rooted FORRT replication studies — paper PDF in, Zenodo-archived release + signed nanopublication chain out |
| [**nanopub-view**](https://github.com/ScienceLiveHub/nanopub-view) | JavaScript/React library for rendering nanopublications |
| [**nanopub-create**](https://github.com/ScienceLiveHub/nanopub-create) | JavaScript/React library for creating nanopublications via forms |
| [**nanopub-notebooks**](https://github.com/ScienceLiveHub/nanopub-notebooks) | Jupyter notebooks for programmatic nanopublication creation (Python) |
| [**science-live-pipeline**](https://github.com/ScienceLiveHub/science-live-pipeline) | Backend pipeline for content extraction and nanopublication generation |
| [**ScienceLiveClaims**](https://github.com/ScienceLiveHub/ScienceLiveClaims) · [**templates4sciencelive**](https://github.com/ScienceLiveHub/templates4sciencelive) | Community-discussed nanopublication templates (Quote-with-comment, AIDA, FORRT Claim, Replication Study, Replication Outcome, CiTO Citation, Research Synthesis, …) |
| [**sciencelivehub.github.io**](https://github.com/ScienceLiveHub/sciencelivehub.github.io) | Source for the [sciencelive4all.org](https://sciencelive4all.org) marketing site |
| [**citex2026-stackable-citations**](https://github.com/ScienceLiveHub/citex2026-stackable-citations) | CiTeX 2026 workshop talk — *"Stackable Citation Knowledge: Building on Nanopublications for Climate and Biodiversity Research"* by Anne Fouilloux and Jean Iaquinta. Slidev deck, recorded demo, references. ([live deck](https://sciencelive4all.org/citex2026-stackable-citations/) · [demo video DOI](https://doi.org/10.5281/zenodo.20419561)) |

---

## Try it

- **Platform**: <https://platform.sciencelive4all.org> · open · CC-BY 4.0 · no login required to read
- **Zotero plugin**: install from [`science-live-platform/zotero/`](https://github.com/ScienceLiveHub/science-live-platform/tree/main/zotero) (Zotero 7+)
- **Replication scaffold**: use the [`forrt-replication-template`](https://github.com/ScienceLiveHub/forrt-replication-template) as a GitHub template
- **Marketing + governance**: <https://sciencelive4all.org>

Published nanopubs live in the **decentralised nanopublication network** — content-addressable via Trusty URIs ([Kuhn et al. 2021](https://doi.org/10.7717/peerj-cs.387)), independent of any single platform shutting down.

---

## Governance and collaboration

Science Live is a collaboration between:

- **[VitenHub AS](https://vitenhub.no)** — Norway · coordination, deployment, sustainability
- **[Knowledge Pixels](https://knowledgepixels.com)** — Switzerland · nanopublication network infrastructure (registry, query, resolver)
- **[Prophet Town](https://www.ptown.tech)** — design and engineering

Funded by the **[Astera Institute](https://astera.org)**.

**License**: source code is MIT unless otherwise noted; published nanopublications are CC-BY 4.0.

**Issues, contributions, discussions**: open on the relevant repository's issue tracker. The platform itself is the [`science-live-platform`](https://github.com/ScienceLiveHub/science-live-platform/issues) repo.

---

## Cite Science Live

If you use Science Live in your research or in a publication:

> Fouilloux, A., & Iaquinta, J. (2026). *Stackable Citation Knowledge: Building on Nanopublications for Climate and Biodiversity Research.* CiTeX 2026 — Workshop on Citation Extraction and Parsing, DIPF Leibniz Institute, Frankfurt. <https://doi.org/10.5281/zenodo.20391905>

For the standalone demo video archived separately on Zenodo: <https://doi.org/10.5281/zenodo.20419561>

---

<sub>Updated 2026-05-28.</sub>
