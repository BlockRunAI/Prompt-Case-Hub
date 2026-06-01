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
notes: Supply one clear face reference; keep the background prompt minimal so the lighting reads as studio rather than busy.
---

A professional cinematic studio headshot demonstrating the unified case format.
The prompt itself lives in the fenced block below so it copies cleanly.

```prompt
A cinematic studio headshot of the person in the reference image. Soft key light
from the upper left, gentle rim light separating the subject from a deep charcoal
seamless backdrop. Shallow depth of field, 85mm portrait look, crisp catchlights
in the eyes, natural skin texture, neutral color grade with a subtle teal-shadow
warm-highlight balance. Centered composition, head-and-shoulders framing.
```

```negative
harsh on-camera flash, blown highlights, plastic skin, distorted facial features,
busy background, text, watermark
```
