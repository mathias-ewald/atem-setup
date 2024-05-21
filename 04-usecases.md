---
layout: section
---
# Usecases
---
layout: two-cols-header
---
# Speaker w/ Static Background

::left::
## Prereqs
- Camera connected via HDMI
- Image loaded into Media Player

## Config
1. Load image into Media Player
2. Set Media Player as main input source
3. Enable Upstream Key with Camera input

::right::
```mermaid {scale: 1.5}
flowchart LR
Camera -- HDMI --> ATEM
Image -.-> ATEM
```
---
layout: two-cols-header
---
# Speaker w/ Video Background

::left::
## Prereqs
- Camera connected via HDMI
- Video playing on another HDMI input
  - dedicated video player
  - 2nd screen with VLC player

## Config
1. Set video as main input source
2. Enable Upstream Key with Camera input

::right::
```mermaid {scale: 1.5}
flowchart LR
Camera -- HDMI --> ATEM
Video[Video\nPlayer] -- HDMI --> ATEM
```
---
layout: two-cols-header
---
# Screen Sharing

::left::
## Prereqs
- Computer connected to ATEM
- <span style="color: grey;">Optional:</span> Camera connected via HDMI

<br/>

## Config A (USK)
1. Set computer screen as main input source
2. <span style="color: grey;">Optional:</span> Enable Upstream Key with camera

<br/>

## Config B (SSrc)
1. Enable SuperSource as main input
2. Configure box with computer screen
3. <span style="color: grey;">Optional:</span> Configure box with camera input

::right::

```mermaid {scale: 1.5}
flowchart LR
Computer -- HDMI --> ATEM
Camera -- HDMI --> ATEM
```
---
layout: two-cols-header
---
# Green Screen (Virtual Background)

::left::
## Prereqs
- Camera connected to ATEM
- Background via MediaPlayer or HDMI
- Green screen behind the speaker
- Proper lighting

<br/>

## Config
1. Set background as main input source
2. Enable Chroma USK and configure according to your current lighting situation


::right::

```mermaid {scale: 1.5}
flowchart LR
Camera -- HDMI --> ATEM
MP[Media\nPlayer] -.-> ATEM
```
---
layout: two-cols-header
---
# Logo

::left::
## Prereqs
1. Create 1920x1080 image with transparency
2. Place logo in top right corner
3. Save as PNG

<br/>

## Config
- Enable DSK with MediaPlayer as Fill/Key
- Configure DSK for image

::right::

```mermaid {scale: 1.5}
flowchart LR
MP[Media\nPlayer] -.-> ATEM
```
---
layout: two-cols-header
---
# Lower Third

::left::

## Prereqs
- Create 1920x1080 video of lower third
- Play video on one of the HDMI inputs<br/>(ext. video player or 2nd monitor)

<br/>

## Config
1. Enable DSK with video
2. Start video

<br/>

<span class="text-xs" style="line-height: 8px;">
Tip 1: Use image with a blend in effect<br/>
Tip 2: [H2RGraphics](https://h2r.graphics/) 
</span>

::right::

```mermaid {scale: 1.5}
flowchart LR
Camera -- HDMI --> ATEM
Video -- HDMI --> ATEM
```