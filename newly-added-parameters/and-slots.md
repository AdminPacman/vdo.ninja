---
description: >-
  Will force the auto-mixer to have that number of slots, even if there are more
  or less videos available to fill them
---

# \&slots

Viewer-Side Option! ([`&view`](../advanced-settings/view-parameters/view.md), [`&scene`](../advanced-settings/view-parameters/scene.md), [`&room`](../general-settings/room.md))

## Options

Example: `&slots=4`

<table><thead><tr><th width="194">Value</th><th>Description</th></tr></thead><tbody><tr><td>(positive integer)</td><td>the number of slots force the auto-mixer to have that number of slots</td></tr></tbody></table>

## Details

You can pass `&slots=N` to a scene link and it will force the auto-mixer to have that number of slots, even if there are more or less videos available to fill them.

Example: `https://vdo.ninja/?room=roomname&scene&slots=4`

![](<../.gitbook/assets/image (114).png>)

I made positioning sticky when using `&slots`, so videos will stick in place now (slot position wise at least), even if another video before it leaves.

If a video is made invisible, it gives up its slot position, which allows a new video to take its spot potentially. When the original video becomes visible again though, the mix-order takes priority. If the mix order is the same, then the connection order takes priority. Dislodged videos are treated like newly joining videos in terms of positioning in the slot.

Screen sharing and highlighting a guest may still break the slotted layout.

If you want more control over position, layout, and all that - consider trying out the [Mixer App](../steves-helper-apps/mixer-app.md) instead, and give some feedback:\
[https://vdo.ninja/alpha/mixer](https://vdo.ninja/alpha/mixer)
