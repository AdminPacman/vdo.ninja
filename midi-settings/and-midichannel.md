---
description: Allows for specifying which midi channel (1 to 16) to listen on
---

# \&midichannel

General Option! ([`&push`](../source-settings/push.md), [`&room`](../general-settings/room.md), [`&view`](../advanced-settings/view-parameters/view.md), [`&scene`](../advanced-settings/view-parameters/scene.md))

## Options

Example: `&midichannel=3`

<table><thead><tr><th width="183">Value</th><th>Description</th></tr></thead><tbody><tr><td>(<code>1</code> to <code>16</code>)</td><td>specifies which midi channel to listen on</td></tr></tbody></table>

## Details

These work in conjunction with [`&midi`](midi.md) to allow for specifying which midi channel (1 to 16) to listen on. If you don't specify anything, it listens to all channels. Previously it was hard-coded to listen to just channel-1, but now it will listen to all channels unless filtered.

## Related

{% content-ref url="midi.md" %}
[midi.md](midi.md)
{% endcontent-ref %}

{% content-ref url="and-mididevice.md" %}
[and-mididevice.md](and-mididevice.md)
{% endcontent-ref %}
