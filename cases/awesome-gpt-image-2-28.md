---
id: awesome-gpt-image-2-28
title: "例 28：写实摄影风格创作"
modality: image
tags: ["headshot", "ui-system", "ad-series"]
source:
  repo: "freestylefly/awesome-gpt-image-2"
  url: "https://github.com/freestylefly/awesome-gpt-image-2/blob/main/docs/gallery-part-1.md"
  author: "freestylefly"
  license: unknown
model:
  recommended: "openai/gpt-image-2"
inputs:
  reference_images: 1
preview: "https://raw.githubusercontent.com/freestylefly/awesome-gpt-image-2/main/data/images/case28.jpg"
---

```prompt
{
  "type": "2x2 portrait grid",
  "subject": "young adult East Asian male with short black hair and a slight smile",
  "style": "photorealistic, high-resolution, professional lighting, consistent facial identity across all panels",
  "layout": {
    "format": "2x2 grid",
    "panel_count": 4,
    "panels": [
      {
        "position": "top-left",
        "description": "Corporate professional wearing a dark navy suit, white shirt, and blue tie against a gray textured background"
      },
      {
        "position": "top-right",
        "description": "Casual attire wearing a dark blue crew neck t-shirt against a blurred outdoor park background"
      },
      {
        "position": "bottom-left",
        "description": "Construction worker wearing a yellow hard hat, navy blue work shirt, and bright orange high-visibility vest against a blurred warehouse background"
      },
      {
        "position": "bottom-right",
        "description": "Medical professional wearing a white lab coat over a light blue collared shirt against a blurred laboratory background"
      }
    ]
  }
}
```
