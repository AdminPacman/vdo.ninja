---
description: Remote MIDI control
---

# \&midiremote

General Option! ([`&push`](../source-settings/push.md), [`&room`](../general-settings/room.md), [`&view`](../advanced-settings/view-parameters/view.md), [`&scene`](../advanced-settings/view-parameters/scene.md))

## Aliases

* `&remotemidi`

## Options

Example: `&midiremote=4`

<table><thead><tr><th width="275">Value</th><th>Description</th></tr></thead><tbody><tr><td>(<code>1</code> to <code>4</code>)</td><td>reference <a href="../midi-settings/midi.md"><code>&#x26;midi</code></a>'s values</td></tr></tbody></table>

## Details

This lets you route all MIDI messages from one computer to another computer, with the purpose of remote triggering the VDO.Ninja hotkeys.

```
https://vdo.ninja/beta/?midiremote=4&director=ROOMNAMEHERE
https://vdo.ninja/beta/?room=ROOMNAMEHERE&midiout=1&vd=0&ad=0&push&autostart&label=MIDI_CONTROLLER
```

* `&midiremote={reference &midi's values; 1 to 4}`

See [`&midi`](../midi-settings/midi.md) for a link to the page with more information on available hotkeys.

{% embed url="https://www.youtube.com/watch?v=rnZ8HM9FL4I" %}
How to remote control with MIDI
{% endembed %}

## Related

{% content-ref url="../midi-settings/midi.md" %}
[midi.md](../midi-settings/midi.md)
{% endcontent-ref %}
