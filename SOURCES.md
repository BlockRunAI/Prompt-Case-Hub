# Integrated sources

Prompt-Case-Hub is a **curation + format layer**. It does not claim authorship of
the prompts it normalizes. Every case carries a `source` block (see
[FORMAT.md](./FORMAT.md)) pointing back to one of the repositories below. Before
redistributing any case content, check the upstream license.

## Currently integrated (848 cases)

These are the real upstream repositories the current case set was normalized from,
with the number of cases contributed. The cases reached this hub via the seed
aggregation repo **[BlockRunAI/Claude-Code-GPT-IMAGE2-SeeDance-BlockRun](https://github.com/BlockRunAI/Claude-Code-GPT-IMAGE2-SeeDance-BlockRun)**,
which originally collected them; each case retains attribution to its true origin.

| Cases | Upstream repository | Focus |
|------:|---------------------|-------|
| 352 | [freestylefly/awesome-gpt-image-2](https://github.com/freestylefly/awesome-gpt-image-2) | gpt-image-2 image cases |
| 300 | [EvoLinkAI/awesome-gpt-image-2-prompts](https://github.com/EvoLinkAI/awesome-gpt-image-2-prompts) | gpt-image-2 prompt collection |
| 105 | [YouMind-OpenLab/awesome-seedance-2-prompts](https://github.com/YouMind-OpenLab/awesome-seedance-2-prompts) | Seedance 2 video prompts |
| 63 | [EvoLinkAI/awesome-seedance-2-guide](https://github.com/EvoLinkAI/awesome-seedance-2-guide) | Seedance 2 guide + cases |
| 28 | [ZeroLu/awesome-seedance](https://github.com/ZeroLu/awesome-seedance) | Seedance video prompts |

> Each case's `source.repo` / `source.url` / `source.author` records its specific
> origin. License is recorded as `unknown` where the upstream did not declare one —
> "reproduced with attribution; original license applies."

## Candidate sources (not yet integrated)

Well-known general / text prompt repositories that fit the hub's scope and are
welcome as future imports (link + index only until their cases are normalized and
their licenses confirmed):

- [f/prompts.chat](https://github.com/f/prompts.chat) — f.k.a. *Awesome ChatGPT Prompts*.
- [dair-ai/Prompt-Engineering-Guide](https://github.com/dair-ai/Prompt-Engineering-Guide) — techniques & patterns.
- [linexjlin/GPTs](https://github.com/linexjlin/GPTs) — public GPT system prompts.
- [EmbraceAGI/awesome-chatgpt-zh](https://github.com/EmbraceAGI/awesome-chatgpt-zh) — Chinese prompt guide.

---

## Adding a source

Open a PR that:
1. Adds the repository to this file with URL, focus, and (where known) license.
2. Adds correctly-formatted, attributed cases under `cases/`.
3. Regenerates `cases/index.json`.

A source whose license forbids redistribution can still be **linked and indexed**
(metadata + link only) without copying its prompt text.
