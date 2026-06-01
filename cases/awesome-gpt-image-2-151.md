---
id: awesome-gpt-image-2-151
title: "例 151：界面交互设计图"
modality: image
tags: ["ui-system", "ad-series", "food"]
source:
  repo: "freestylefly/awesome-gpt-image-2"
  url: "https://github.com/freestylefly/awesome-gpt-image-2/blob/main/docs/gallery-part-1.md"
  author: "freestylefly"
  license: unknown
model:
  recommended: "openai/gpt-image-2"
inputs:
  reference_images: 1
preview: "https://raw.githubusercontent.com/freestylefly/awesome-gpt-image-2/main/data/images/case151.jpg"
---

```prompt
{
  "type": "2x2 advertising banner grid",
  "layout": "4 distinct quadrants, each featuring a different industry advertisement",
  "quadrants": [
    {
      "position": "top-left",
      "industry": "skincare",
      "visuals": "Asian woman touching cheek, floating water droplets, white pump bottle",
      "brand": "BALANCÉE",
      "copy": {
        "headline": "素肌が、目覚める。",
        "subheadline": "透明感あふれる、新しいわたしへ。",
        "features_count": 3,
        "features_labels": ["高保湿", "肌荒れ予防", "美白ケア*"]
      }
    },
    {
      "position": "top-right",
      "industry": "restaurant food",
      "visuals": "close-up of spaghetti bolognese with grated cheese and parsley, dark moody lighting",
      "brand": "Trattoria Luce",
      "copy": {
        "headline": "このパスタ、事件級。",
        "badge": "期間限定",
        "description": "黒毛和牛のボロネーゼ 〜トリュフの香り〜"
      }
    },
    {
      "position": "bottom-left",
      "industry": "travel",
      "visuals": "woman with backpack facing a scenic mountain lake, bright daylight",
      "brand": "NATURE JOURNEY",
      "copy": {
        "headline": "わたしを、解き放つ旅へ。",
        "subheadline": "自然の中で、心が動き出す。",
        "script": "Find your freedom.",
        "banner_details": ["初夏の特別キャンペーン", "6.1 SAT - 6.30 SUN", "最大 20%OFF", "今だけの特別プラン多数！"]
      }
    },
    {
      "position": "bottom-right",
      "industry": "SaaS app",
      "visuals": "smartphone displaying a task management app interface with 4 schedule items",
      "brand": "Taskme",
      "copy": {
        "headline": "タスク管理を、もっとシンプルに、スマートに。",
        "circle_badge": "1日を、デザインしよう。",
        "features_count": 3,
        "features_labels": ["直感的な操作性", "チームで共有可能", "どこでもアクセス"],
        "bottom_banner": "7日間無料トライアル実施中！"
      }
    }
  ]
}
```
