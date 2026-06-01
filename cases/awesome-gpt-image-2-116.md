---
id: awesome-gpt-image-2-116
title: "例 116：主题海报版式设计"
modality: video
tags: ["poster", "ui-system", "ad-series", "anime", "fantasy"]
source:
  repo: "freestylefly/awesome-gpt-image-2"
  url: "https://github.com/freestylefly/awesome-gpt-image-2/blob/main/docs/gallery-part-1.md"
  author: "freestylefly"
  license: unknown
model:
  recommended: "bytedance/seedance-2.0-fast"
inputs:
  reference_images: 0
preview: "https://raw.githubusercontent.com/freestylefly/awesome-gpt-image-2/main/data/images/case116.jpg"
---

```prompt
{
  "type": "2-page manga spread",
  "style": "monochrome anime manga, screentones",
  "theme": "fantasy mage developing a video game",
  "character": "anime girl with blonde hair, tiara, cape, white dress, thigh-highs",
  "layout": {
    "left_page": {
      "panel_count": 11,
      "rows": [
        {"panels": 1, "action": "Determined at dual-monitor desk, speech bubble: '新作ゲーム、絶対完成させる！'"},
        {"panels": 3, "action": "Typing, drawing on tablet, testing with controller"},
        {"panels": 3, "action": "Shocked at ERROR screen, depressed, determined again"},
        {"panels": 4, "action": "Exhausted, sudden realization, furious typing, monitor showing 'Build succeeded!'"}
      ]
    },
    "right_page": {
      "panel_count": 2,
      "panels": [
        {"type": "large splash", "action": "Casting magic from a glowing circle at a code-error monster labeled 'NullReferenceException'. Speech bubble: 'デバッグ魔法!!'"},
        {"type": "bottom banner", "action": "Cheering in front of RPG title screen. Speech bubble: 'やったー！'"}
      ]
    }
  }
}
```
