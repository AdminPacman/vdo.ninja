---
description: Sets a room ID for the session to join
---

# \&room

General Option! ([`&push`](../source-settings/push.md), [`&scene`](../advanced-settings/view-parameters/scene.md), [`&solo`](../advanced-settings/mixer-scene-parameters/and-solo.md))

## Aliases

* `&roomid`
* `&r`

## Options

Example: `&room=RoomID`

<table><thead><tr><th width="335">Value</th><th>Description</th></tr></thead><tbody><tr><td>(string)</td><td>1 to 49-characters long: aLphaNumEric-characters; case sensitive.</td></tr></tbody></table>

## Details

Rooms broadcast to all participants who have joined.

Rooms are complemented by the [`&director=roomname`](../viewers-settings/director.md) function. Directors can have oversight of a room.

Rooms limit the viewing bitrate that guests of a room can request. OBS does not have these viewing limits though.

Rooms have no forced limit on the number of guests allowed, but practically 10 is about the limit I'd recommend.

Adding [`&showonly=xxx`](../advanced-settings/video-parameters/novideo-1.md) and [`&roombitrate=0`](../advanced-settings/video-bitrate-parameters/roombitrate.md) to the guest's URL can be used to help increase the capacity of rooms to 30 or more.

An alternative to a `&room` is a [_faux-room_](../getting-started/multi-person-chat.md), which can be done with:\
`https://vdo.ninja/?push=aaa&view=bbb,ccc,ddd`

## Additional info

There's a documentation page dedicated to rooms [here](../getting-started/rooms/).

There's also a video below looking at what sort of performance and system load there is when using an unoptimized group room.

{% embed url="https://www.youtube.com/watch?v=VYYG4rZffcM" %}

You can reduce CPU load using the [`&broadcast`](../advanced-settings/view-parameters/broadcast.md) flag, if hosting a larger room.

You can also [transfer guests between group rooms](../getting-started/rooms/transfer-rooms.md), using the transfer function that the director has.

## Related

{% content-ref url="../getting-started/rooms/" %}
[rooms](../getting-started/rooms/)
{% endcontent-ref %}

{% content-ref url="../getting-started/rooms/transfer-rooms.md" %}
[transfer-rooms.md](../getting-started/rooms/transfer-rooms.md)
{% endcontent-ref %}

{% content-ref url="../viewers-settings/director.md" %}
[director.md](../viewers-settings/director.md)
{% endcontent-ref %}
