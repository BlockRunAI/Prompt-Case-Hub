# Prompt-Case-Hub

A **unified, format-standardized hub** that aggregates prompt *cases* from popular
open-source prompt repositories — image, video, and text — and re-expresses them
under **one consistent case schema**.

Most prompt repos in the wild each invent their own structure: some are flat
`README` tables, some are per-folder markdown, some are JSON, some bury the prompt
inside prose. That makes them hard to consume programmatically and hard to compare.
Prompt-Case-Hub does two things:

1. **Resource integration** — curates and credits high-quality cases from the
   open-source repositories listed below.
2. **Format unification** — normalizes every case into a single
   [case schema](./FORMAT.md) (YAML front-matter + prompt body, plus a JSON index)
   so any tool can load, filter, and render cases the same way.

> Curated by [BlockRun.ai](https://blockrun.ai). This repo holds the **format,
> index, and attribution layer** — original prompt authorship and licensing stay
> with the upstream sources (see [SOURCES.md](./SOURCES.md)).

---

## Integrated sources

At minimum, the hub integrates and credits the following open-source repositories
(full attribution + license notes in [SOURCES.md](./SOURCES.md)):

| Repository | Focus | Notes |
|------------|-------|-------|
| [BlockRunAI/Claude-Code-GPT-IMAGE2-SeeDance-BlockRun](https://github.com/BlockRunAI/Claude-Code-GPT-IMAGE2-SeeDance-BlockRun) | Image / video | The seed library — gpt-image-2 & Seedance one-line cases. |
| [jamez-bondos/awesome-gpt4o-images](https://github.com/jamez-bondos/awesome-gpt4o-images) | Image | Curated GPT-4o / gpt-image-1 image cases with previews. |
| [f/prompts.chat](https://github.com/f/prompts.chat) | Text | f.k.a. *Awesome ChatGPT Prompts* — the classic community collection. |
| [dair-ai/Prompt-Engineering-Guide](https://github.com/dair-ai/Prompt-Engineering-Guide) | Text / method | Techniques and reference patterns. |
| [linexjlin/GPTs](https://github.com/linexjlin/GPTs) | Text | System-prompt collection from public GPTs. |
| [EmbraceAGI/awesome-chatgpt-zh](https://github.com/EmbraceAGI/awesome-chatgpt-zh) | Text (zh) | Chinese prompt guide and curated list. |

This list is intentionally additive — new sources are welcomed via PR as long as
each integrated case carries its `source` attribution (see [FORMAT.md](./FORMAT.md)).

---

## Repository layout

```
.
├── FORMAT.md            # the unified prompt-case schema (the spec)
├── SOURCES.md           # integrated repos: attribution + license notes
├── schema/
│   └── case.schema.json # JSON Schema for validating a case's front-matter
├── cases/
│   ├── index.json       # machine-readable index of all cases
│   └── *.md             # one file per case (front-matter + prompt body)
└── CONTRIBUTING.md      # how to add / normalize a case
```

## Using the cases

Every case is a markdown file with YAML front-matter and a fenced `prompt` body,
plus an entry in [`cases/index.json`](./cases/index.json). To consume them:

- **Browse**: open any file under [`cases/`](./cases/).
- **Programmatic**: read `cases/index.json` for the catalog, then load each
  case file and parse its front-matter against [`schema/case.schema.json`](./schema/case.schema.json).

See [FORMAT.md](./FORMAT.md) for the full field reference and a worked example.

## Status

Bootstrapping. The schema, index format, and attribution layer are in place;
cases are being normalized from the integrated sources. Contributions that add a
correctly-formatted, properly-attributed case are welcome — see
[CONTRIBUTING.md](./CONTRIBUTING.md).

## License

The curation layer (schema, index, docs) is released under the MIT License
(see [LICENSE](./LICENSE)). **Individual prompt cases retain the license and
authorship of their upstream source** — consult [SOURCES.md](./SOURCES.md) before
redistributing any case content.
