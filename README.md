# Training data

Static site at `https://jxb1st.github.io/training-data-collection/`: one page per dataset (VidChapters-7M, Ego4D and LLaVA-Video-178K) with the released
annotation format, per-dataset statistics, and up to three examples per task type, each with its
annotation as released and a short 480p clip where the videos could be obtained. The companion site is
`https://jxb1st.github.io/benchmark-collection/`.

- `index.html`: overview table and the list of datasets. `<dataset>/index.html`: one page per dataset.
- `<dataset>/clips/`: short excerpts re-encoded at 480p H.264 with a mid-clip poster frame.
- `<dataset>/data/samples.json` and `stats.json`: the examples with their annotation fields, and the
  statistics shown on the page, computed from the released annotation files where available.
- `style.css` is the shared stylesheet of the experiment panel; `collection.css` adds the example cards.

Examples are chosen deterministically from the released annotations with a preference for short
questions and short videos. Where videos are not available (YouTube-only or gated archives, licensed
datasets), the example is annotation only and the page says so. Annotation text is verbatim.
