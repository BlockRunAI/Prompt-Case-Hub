# Contributing

Thanks for helping integrate and normalize prompt cases. The whole point of this
hub is **one consistent format**, so contributions are mostly about converting an
upstream case into our schema.

## Adding a case

1. **Pick a source** that's listed in [SOURCES.md](./SOURCES.md) (or add it there
   in the same PR).
2. **Create one file per case** under `cases/`, named `id.md` where `id` matches
   the front-matter `id`.
3. **Fill the front-matter** per [FORMAT.md](./FORMAT.md). `source.repo`,
   `source.url`, and `source.license` are mandatory — no provenance, no merge.
4. **Put the prompt in fenced blocks** (` ```prompt ` and optional ` ```negative `).
   Keep the prompt text verbatim from the source.
5. **Register it** in [`cases/index.json`](./cases/index.json).
6. **Validate** the front-matter against
   [`schema/case.schema.json`](./schema/case.schema.json).

## Rules of thumb

- One case = one file. Split multi-prompt pages.
- Don't paraphrase upstream prompt text.
- Slugs (`id`) are permanent — never reuse one.
- If a source's license forbids copying its text, link + index it (metadata only)
  rather than pasting the prompt.

## Validating locally

Any JSON-Schema (draft-07) validator works. Example with `ajv`:

```bash
npx ajv-cli validate -s schema/case.schema.json -d "front-matter.json"
```

(Extract the YAML front-matter to JSON first, or use a front-matter-aware linter.)
