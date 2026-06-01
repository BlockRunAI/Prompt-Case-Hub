# The unified prompt-case format

Every case in this hub is a single markdown file with two parts:

1. **YAML front-matter** — structured metadata (validated against
   [`schema/case.schema.json`](./schema/case.schema.json)).
2. **A prompt body** — the actual prompt(s) in fenced code blocks, so they copy
   cleanly with no markdown rendering in the way.

This is the *one* shape every integrated source is normalized into.

## Front-matter fields

| Field | Required | Type | Description |
|-------|----------|------|-------------|
| `id` | ✅ | string (kebab-case slug) | Stable, unique identifier. Never reused. |
| `title` | ✅ | string | Human-readable name of the case. |
| `modality` | ✅ | enum | One of `image`, `video`, `text`, `audio`. |
| `tags` | ✅ | string[] | Free-form keywords (`portrait`, `cyberpunk`, `headshot`…). |
| `source` | ✅ | object | Provenance — see below. Required for every integrated case. |
| `source.repo` | ✅ | string | `owner/name` of the upstream repository. |
| `source.url` | ✅ | string (URL) | Direct link to the original case / file. |
| `source.author` | ➖ | string | Original author handle, if known. |
| `source.license` | ✅ | string | Upstream license SPDX id, or `unknown`. |
| `model` | ➖ | object | Recommended / tested models. |
| `model.recommended` | ➖ | string | e.g. `openai/gpt-image-1`, `bytedance/seedance-2.0`. |
| `model.tested_on` | ➖ | string[] | Models this prompt is known to work on. |
| `inputs` | ➖ | object | Expected inputs. |
| `inputs.reference_images` | ➖ | integer | How many reference images the prompt expects (0 = text-only). |
| `inputs.aspect_ratio` | ➖ | string | e.g. `1:1`, `16:9`, `9:16`. |
| `preview` | ➖ | string (URL/path) | A sample output image/video for the gallery. |
| `notes` | ➖ | string | Usage tips, caveats, parameter hints. |

The **prompt body** follows the front-matter. Use a fenced block labelled
`prompt` for the main prompt, and optionally `negative` for a negative prompt:

````md
```prompt
<the main prompt text>
```

```negative
<optional negative prompt>
```
````

## Worked example

See [`cases/sample-cinematic-headshot.md`](./cases/sample-cinematic-headshot.md)
for a complete, valid case. Its front-matter:

```yaml
---
id: cinematic-headshot
title: Cinematic studio headshot
modality: image
tags: [portrait, headshot, studio, cinematic]
source:
  repo: jamez-bondos/awesome-gpt4o-images
  url: https://github.com/jamez-bondos/awesome-gpt4o-images
  author: jamez-bondos
  license: unknown
model:
  recommended: openai/gpt-image-1
  tested_on: [openai/gpt-image-1, google/nano-banana-pro]
inputs:
  reference_images: 1
  aspect_ratio: "1:1"
notes: Supply one clear face reference; keep the background prompt minimal.
---
```

## The index

Every case is also registered in [`cases/index.json`](./cases/index.json), a flat
array of catalog entries. This lets a consumer list/filter the whole library
without opening each file. Each entry mirrors the key front-matter fields:

```json
{
  "id": "cinematic-headshot",
  "title": "Cinematic studio headshot",
  "modality": "image",
  "tags": ["portrait", "headshot", "studio", "cinematic"],
  "file": "cases/sample-cinematic-headshot.md",
  "source": "jamez-bondos/awesome-gpt4o-images"
}
```

## Normalization rules

When importing a case from an upstream source:

1. **One case = one file.** Split multi-prompt READMEs into separate files.
2. **Keep the prompt verbatim.** Don't paraphrase upstream prompt text; only fix
   obvious encoding artifacts.
3. **Always attribute.** `source.repo`, `source.url`, and `source.license` are
   mandatory — a case with no provenance is not accepted.
4. **Slugs are forever.** Pick a clear `id`; never reuse or repurpose one.
5. **Validate** against `schema/case.schema.json` before opening a PR.
