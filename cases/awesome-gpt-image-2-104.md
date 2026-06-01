---
id: awesome-gpt-image-2-104
title: "例 104：界面交互设计图"
modality: video
tags: ["ui-system", "card-deck", "logo-3d"]
source:
  repo: "freestylefly/awesome-gpt-image-2"
  url: "https://github.com/freestylefly/awesome-gpt-image-2/blob/main/docs/gallery-part-1.md"
  author: "freestylefly"
  license: unknown
model:
  recommended: "bytedance/seedance-2.0-fast"
inputs:
  reference_images: 0
preview: "https://raw.githubusercontent.com/freestylefly/awesome-gpt-image-2/main/data/images/case104.jpg"
---

```prompt
{
  "type": "YouTube livestream UI",
  "top_nav": {
    "logo": "YouTube Premium",
    "search": "bilal fraiha",
    "icons": 3
  },
  "player": {
    "subjects": [
      "Sydney Sweeney in white cardigan",
      "bearded man in beige jacket laughing"
    ],
    "bg": "couch, 2 silver play buttons, ram logo 'SARDI'",
    "overlays": {
      "chat": {"pos": "left", "count": 15, "desc": "colored usernames, white text"},
      "goal": {"pos": "top right", "text": "TONIGHT'S GOAL: 0 to 25"},
      "banner": {"pos": "bottom center", "text": "K MOREBILAL"}
    },
    "controls": {"count": 10}
  },
  "details": {
    "title": "FULL STREAM | سيدني سويني مع بلال",
    "channel": "More Bilal No Filter",
    "buttons": 5
  }
}
```
