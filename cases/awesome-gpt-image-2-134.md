---
id: awesome-gpt-image-2-134
title: "例 134：界面交互设计图"
modality: image
tags: ["ui-system", "ad-series", "card-deck", "unbox", "logo-3d"]
source:
  repo: "freestylefly/awesome-gpt-image-2"
  url: "https://github.com/freestylefly/awesome-gpt-image-2/blob/main/docs/gallery-part-1.md"
  author: "freestylefly"
  license: unknown
model:
  recommended: "openai/gpt-image-2"
inputs:
  reference_images: 1
preview: "https://raw.githubusercontent.com/freestylefly/awesome-gpt-image-2/main/data/images/case134.jpg"
---

```prompt
{
  "type": "skincare e-commerce landing page mockup",
  "brand": "DERMA CALM",
  "color_palette": ["white", "light blue", "dark blue"],
  "layout": {
    "header": {
      "logo": "left-aligned brand name with Japanese subtext",
      "navigation_links": {
        "count": 6,
        "labels": ["ABOUT", "PRODUCT", "FEATURE", "INGREDIENT", "VOICE", "Q&A"]
      },
      "buttons": {
        "count": 2,
        "labels": ["マイページ", "今すぐ購入する"]
      }
    },
    "hero_section": {
      "left_column": {
        "headline": "敏感な肌にも、毎日つづけられる安心ケア。",
        "subtext": "paragraph detailing low irritation, moisturizing, fragrance-free, and alcohol-free benefits",
        "buttons": {
          "count": 2,
          "labels": ["今すぐ購入する", "詳しく見る"]
        }
      },
      "center_column": {
        "product": "white pump bottle with clear cap labeled Moisture Barrier Serum",
        "props": ["dollop of white cream", "circular badge reading 皮膚科医監修"]
      },
      "right_column": {
        "subject": "young East Asian woman with clear glowing skin touching her cheek",
        "background": "blurred laboratory glassware in a bright, clean clinical setting"
      }
    },
    "bottom_features_panel": {
      "left_cards": {
        "count": 3,
        "descriptions": ["95% satisfaction with 5 stars", "shield icon for low irritation formula", "drop icon for skin barrier support"]
      },
      "right_badges": {
        "count": 3,
        "descriptions": ["no fragrance icon", "no alcohol icon", "patch tested icon"]
      },
      "footer": "fine print disclaimers at the bottom"
    }
  }
}
```
