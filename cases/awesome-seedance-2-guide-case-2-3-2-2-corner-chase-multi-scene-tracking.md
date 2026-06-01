---
id: awesome-seedance-2-guide-case-2-3-2-2-corner-chase-multi-scene-tracking
title: "Case 2-3-2-2 · Corner Chase + Multi-Scene Tracking"
modality: video
tags: ["ad-series"]
source:
  repo: "EvoLinkAI/awesome-seedance-2-guide"
  url: "https://github.com/EvoLinkAI/awesome-seedance-2-guide/blob/main/use-cases/en/02-camera-movement.md"
  author: "EvoLinkAI"
  license: unknown
model:
  recommended: "bytedance/seedance-2.0-fast"
inputs:
  reference_images: 0
preview: "https://pub-babc88c25d274cfeb8b2ae0cd0816872.r2.dev/assets/2-3-2/2/ref1.jpg"
---

```prompt
Reference the man's image from @image1. He is in the corridor from @image2. Completely reference all camera movement effects and the protagonist's facial expressions from @video1. The camera follows the protagonist running around the corner in @image2, then in the long corridor of @image3, the camera transitions from a rear tracking perspective to an orbit around the protagonist's front. The camera then pans right 90 degrees to shoot the fork in the road from @image4, stops abruptly then pans right 180 degrees, close-up shot of the protagonist's front face. The protagonist is panting heavily. The camera follows the protagonist's perspective orbiting around to observe the surroundings, referencing the rapid left-right orbiting camera movement from @video1 to showcase the scene. Then pull back to @image5, continue tracking the protagonist's side profile running.
```
