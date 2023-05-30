---
description: Allows for receiving of remote MIDI
---

# \&midiin

General Option! ([`&push`](../source-settings/push.md), [`&room`](../general-settings/room.md), [`&view`](../advanced-settings/view-parameters/view.md), [`&scene`](../advanced-settings/view-parameters/scene.md))

## Aliases

* `&midipull`
* `&mi`

## Options

Example: `&midiin=2`

<table><thead><tr><th width="225">Value</th><th>Description</th></tr></thead><tbody><tr><td><code>0</code></td><td>all midi output devices</td></tr><tr><td>(integer value. eg: 1)</td><td>midi output device index 1</td></tr></tbody></table>

## Details

Allows for receiving of remote MIDI. Device indices starts at 1, where an index of 0 implies "all".

{% hint style="danger" %}
If testing locally, beware of feedback loops, where the MIDI output is fed back into the MIDI input, causing high CPU usage and a lot of MIDI messages. If testing locally, use two MIDI devices and explicitly select the input and output MIDI devices to avoid these feedback loops.
{% endhint %}

## Related

{% content-ref url="midi.md" %}
[midi.md](midi.md)
{% endcontent-ref %}

{% content-ref url="midiout.md" %}
[midiout.md](midiout.md)
{% endcontent-ref %}
