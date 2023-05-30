---
description: Same concept as &view, except does the opposite
---

# \&exclude

Viewer-Side Option! ([`&view`](view.md), [`&scene`](scene.md), [`&room`](../../general-settings/room.md))

## Aliases

* `&ex`

## Options

Example: `&exclude=StreamID1,StreamID2`

<table><thead><tr><th width="200">Value</th><th>Description</th></tr></thead><tbody><tr><td>(string value)</td><td>stream ID to view; can be a comma-separated list of IDs</td></tr></tbody></table>

## Details

Any stream ID listed as a value will **NOT** be played or requested.

Example usage:

`https://vdo.ninja/?room=myroom123&exclude=stream121,sidestream321`

{% hint style="warning" %}
Excluding a stream ID will prevent even a peer connection.\
No video, audio, or chat can be had.
{% endhint %}
