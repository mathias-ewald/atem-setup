---
layout: section
---
# How It Works
---
layout: none
---
<SlidevVideo autoplay controls="false" style="width: 100%">
  <source src="/switcher.hd.1080p.mp4" type="video/mp4" />
  <p>
    Your browser does not support videos. You may download it
    <a href="/switcher.hd.1080p.mp4">here</a>.
  </p>
</SlidevVideo>
---
layout: center
---

<v-switch>
  <template #0>

```mermaid {scale: 1.5}
flowchart LR
Cameras -- HDMI --> ATEM -- USB --> Computer -- Webcam --> App
Computer -- Mic --> App
``` 

  </template>
  <template #1>

```mermaid {scale: 1.5}
flowchart LR
Cameras -- HDMI --> ATEM -- USB --> Computer -- Webcam --> App
Computer -- Mic --> App
Mics -- Jack --> ATEM
```

  </template>
</v-switch>

---