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

```mermaid {scale: 1.25}
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

```mermaid {scale: 1.25}
flowchart LR
ATEM -- USB --> Computer
ATEM -- Net --> Stream
ATEM -- USB --> SSD
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
layout: two-cols
---
# Function Primitives
Basic functions can be combined

<style>
.footnotes-sep {
    visibility: hidden;
}
</style>

<br/>

## Video
<div class="text-sm">

- Transitions <span style="color: grey">(Cut, Mix, Wipe, Dip, DVE, Stinger<sup>1</sup>)</span>
- Upstream Key <span style="color: grey">(Luma, Chroma, Pattern, DVE)</span>
- Downstream Key <span style="color: grey">(Bugs, Logos, Lower Thirds)</span>
- Media Player <span style="color: grey">(Images, Clips<sup>1</sup>)</span>
- Super Source <sup>2</sup>
- Color Generators

</div>


<br/>

## Audio
<div class="text-sm">

- Equalizer <span style="color: grey">(6 band)</span>
- Dynamics <span style="color: grey">(Expander, Gate, Compressor, Limiter)</span>

</div>

<div style="font-size: 60%; margin-top: 15px;">
[1]: ATEM Constellation or higher<br/>
[2]: ATEM Mini Extreme or higher
</div>

::right::

<div style="display: flex; flex-direction: column; align-items: center; gap: 50px">
    <figure style="width: 50%">
        <img src="/usk.jpg" alt="Trulli">
        <figcaption style="font-size: 50%; text-align: center;">Green screen with Chroma Key</figcaption>
    </figure>
    <figure style="width: 50%">
        <img src="/dsk.jpg" alt="Trulli">
        <figcaption style="font-size: 50%; text-align: center;">Logo with Downstream Key</figcaption>
    </figure>
</div>

---
---
# Transitions
Basic Examples

<div style="width: 100%; display: grid; grid-template-columns: repeat(3,1fr); grid-template-rows: repeat(3,auto); grid-gap:50px 30px;">
   <SlidevVideo autoplay loop><source src="/cut.mp4" type="video/mp4" /></SlidevVideo>
   <SlidevVideo autoplay loop><source src="/mix.mp4" type="video/mp4" /></SlidevVideo>
   <SlidevVideo autoplay loop><source src="/dip.mp4" type="video/mp4" /></SlidevVideo>
   <SlidevVideo autoplay loop><source src="/wipe.mp4" type="video/mp4" /></SlidevVideo>
   <SlidevVideo autoplay loop><source src="/dve.mp4" type="video/mp4" /></SlidevVideo>
</div>
---