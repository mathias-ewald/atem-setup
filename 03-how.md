---
layout: section
---
# How It Works
---
layout: none
---
<SlidevVideo autoplay style="width: 100%">
  <source src="/switcher.hd.1080p.mp4" type="video/mp4" />
  <p>
    Your browser does not support videos. You may download it
    <a href="/switcher.hd.1080p.mp4">here</a>.
  </p>
</SlidevVideo>

---
layout: default
---
# Big Picture

<div style="height: 100%; display: flex; flex-direction: row; justify-content: center; align-items: center">

```mermaid {scale: 1.5}
flowchart LR
Inputs[Input Sources] --> ATEM --> Output[Content Output]
```

</div>

---
layout: two-cols-header
---
# Input Sources
Takes inputs for processing

::left::

## Video, e.g.
- Camera
- Computer
- Tablet

## Audio, e.g.
- Microphone
- Audio Interface

<br/>
<br/>

::right::

```mermaid {scale: 1.5}
flowchart LR
Video -- HDMI --> ATEM
Audio -- Jack --> ATEM
```

---
layout: two-cols-header
layoutClass: gap-16
---

# Content Output
Mixes inputs into a single output

::left::

```mermaid {scale: 1.5}
flowchart LR
ATEM -- USB --> Computer
ATEM -- Net --> Stream((Stream\nTarget))
```

::right::

## Webcam, e.g.
- Zoom
- Google Meet
- Teams

## Streaming, e.g.
- YouTube
- LinkedIn
---