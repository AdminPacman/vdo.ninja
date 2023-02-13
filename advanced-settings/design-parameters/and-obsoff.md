---
description: Disables the tally light effects
---

# \&obsoff

Viewer-Side Option! ([`&view`](../view-parameters/view.md), [`&scene`](../view-parameters/scene.md), [`&room`](../../general-settings/room.md))

## Aliases

* `&oo`
* `&disableobs`

## Details

Disables the tally light effects; can be applied to both viewer or publisher. Tally lights are represented as a glowing red border around videos. When the light is on, the video is considered "VISIBLE" within OBS Studio. This is based on whether OBS Studio tells VDO.Ninja if a video is active or not.

{% hint style="info" %}
Videos on **first-load** in OBS, even if visible in OBS, **don't glow red**; it requires an **initial visibility change to trigger it**.
{% endhint %}

`&obsoff` can be used to set permissions to fully off (also disables tally light and scene optimizations tho) when added to the OBS browser source link.

## Related

{% content-ref url="../settings-parameters/and-controlobs.md" %}
[and-controlobs.md](../settings-parameters/and-controlobs.md)
{% endcontent-ref %}

{% content-ref url="tallyoff-1.md" %}
[tallyoff-1.md](tallyoff-1.md)
{% endcontent-ref %}
