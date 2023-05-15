---
description: OpenH264 software encoding will be used
---

# \&h264profile

Viewer-Side Option! ([`&view`](../advanced-settings/view-parameters/view.md), [`&scene`](../advanced-settings/view-parameters/scene.md), [`&room`](../general-settings/room.md))

## Options

Example: `&h264profile=42e01f`

| Value                                        | Description                                                                                                                                    |
| -------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------- |
| (no value given)                             | disables hardware h264 encoding -> OpenH264 software encoding will be used, if H264 is used. This is the same as setting the value to `42e01f` |
| `42e01f`                                     | advanced users can also pass a 6-character h264 profile ID to the parameter to get used instead. This one triggers OpenH264.                   |
| `42001f` \| `420029` \| `42a01e` \| `42a014` | just some examples of other h264 profiles you can try; these often will use the external hardware encoder on Windows systems.                  |
| `0` \| `false` \| `off` \| `default`         | has the h264 profile be left as the default browser default when the sender is an android                                                      |

## Details

`&h264profile` if added to the viewer-side will tweak the h264 profile type.

Open264 software encoding can actually use less CPU than the Windows-selected hardware encoder, and in some cases will suffer from less video glitching. For this reason, it's the default profile ID that gets used when `&h264profile` is added without a value.

Without using `&h264profile`, it's up to the system to decide what profile is used, and whether hardware encoding or software encoding is used. There is no way to force hardware to be used at this time, but you can force software, which may actually use less CPU and will avoid video glitching that hardware encoders sometime have.

Hardware encoders can sometimes cause the video to puke, turn all green, pink, or grey, especially at lower resolutions. It really depends on the hardware and driver being used by the sender, so if you really want to use H264, but it's glitching, adding `&h264profile` and enabling software-encoding can help there.

Advanced users can also pass a 6-character h264 profile ID to the parameter to get used instead. This flag will not force H264 to be used, but rather configures it in case h264 gets used. You can still use [`&codec`](../advanced-settings/view-parameters/codec.md) to set the codec to h264.

Example: `https://vdo.ninja/?view=xxx&h264profile=42e01f&codec=h264&stats`

<div align="left">

<img src="https://lh5.googleusercontent.com/sITY54EgMFJiM2nX7QXOjd645PKQv_xktwsSUg1QVyvdpxJ9hLRuv0iyOQiL4nHw0dDYklKKp8bqh5F3jFh8prq9foPjaEZmv_se_bEwzhECGUDjTYHCJvbaw_eve8Xs3T5_7fxf" alt="">

</div>

## Related

{% content-ref url="../advanced-settings/view-parameters/codec.md" %}
[codec.md](../advanced-settings/view-parameters/codec.md)
{% endcontent-ref %}
