---
id: awesome-gpt-image-2-121
title: "例 121：建筑空间场景图"
modality: image
tags: ["ui-system", "anime", "sci-fi"]
source:
  repo: "freestylefly/awesome-gpt-image-2"
  url: "https://github.com/freestylefly/awesome-gpt-image-2/blob/main/docs/gallery-part-1.md"
  author: "freestylefly"
  license: unknown
model:
  recommended: "openai/gpt-image-2"
inputs:
  reference_images: 1
preview: "https://raw.githubusercontent.com/freestylefly/awesome-gpt-image-2/main/data/images/case121.jpg"
---

```prompt
{
  "type": "3-panel manga page",
  "style": "anime, highly detailed, cinematic lighting, futuristic corporate",
  "layout": {
    "structure": "1 wide top panel, 2 square bottom panels"
  },
  "panels": [
    {
      "position": "top",
      "shot": "wide landscape",
      "scene": "Futuristic corporate lobby with floor-to-ceiling windows",
      "lighting": "sunrise",
      "background": "City skyline featuring Tokyo Tower",
      "details": "Holographic displays, polished reflective floor, reception desk, lounge chairs"
    },
    {
      "position": "bottom left",
      "shot": "close-up profile",
      "character": "Young woman, dark hair, black business suit",
      "accessories": "Futuristic black earpiece with glowing blue light",
      "speech_bubble": {
        "style": "standard rounded",
        "text": "数字はいいわ"
      }
    },
    {
      "position": "bottom right",
      "shot": "full body, walking away, touching earpiece",
      "character": "Same woman, black suit, black heels, carrying a black tote bag",
      "environment": "Approaching security gates",
      "holographic_sign": "ECHO 42F",
      "speech_bubble": {
        "style": "futuristic angular",
        "text": "おはようございます、ユキさん。本日は記念すべき ──"
      }
    }
  ]
}
```
