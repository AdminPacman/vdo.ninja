---
description: Hides the mouse cursor over videos at a CSS level
---

# \&nocursor

General Option! ([`&push`](../source-settings/push.md), [`&room`](room.md), [`&view`](../advanced-settings/view-parameters/view.md), [`&scene`](../advanced-settings/view-parameters/scene.md))

## Details

This does not hide the mouse cursor for Chrome-based screen capture, as Chrome [does not yet support that](https://developer.mozilla.org/en-US/docs/Web/API/MediaTrackConstraints/cursor#browser\_compatibility). This feature is designed for hiding the mouse when using the [Electron Capture](../steves-helper-apps/electron-capture.md) app, to avoid mousing over the capture area by accident.

Works better in Windows than on macOS, due to OS-level limitations.

If you're looking to hide the cursor while screen-recording, consider using OBS to capture and OBS Virtual Cam as the source into VDO.Ninja. You can also check out: [https://github.com/rdp/screen-capture-recorder-to-video-windows-free](https://github.com/rdp/screen-capture-recorder-to-video-windows-free) as an option to turn a screen into a virtual camera without needing OBS.

## Related

{% content-ref url="../common-errors-and-known-issues/cursor-shows-when-screen-sharing.md" %}
[cursor-shows-when-screen-sharing.md](../common-errors-and-known-issues/cursor-shows-when-screen-sharing.md)
{% endcontent-ref %}

{% content-ref url="../source-settings/cursor.md" %}
[cursor.md](../source-settings/cursor.md)
{% endcontent-ref %}
