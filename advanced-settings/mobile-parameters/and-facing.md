---
description: Lets you specify either the front or rear facing camera as the default camera
---

# \&facing

Sender-Side Option! ([`&push`](../../source-settings/push.md))

## Options

Example: `&facing=rear`

<table><thead><tr><th width="305">Value</th><th>Description</th></tr></thead><tbody><tr><td><code>rear</code> | <code>environment</code> | <code>back</code></td><td>rear-facing camera</td></tr><tr><td><code>front</code> | <code>user</code></td><td>front-facing camera</td></tr></tbody></table>

## Details

The `&facing` setting lets you specify either the front or rear facing camera as the default camera. Passing one of `rear`, `environment`, `back`, `front`, and `user` are required to specify whether to select back or front.\
\
Example usage:[`https://vdo.ninja/?webcam&facing=rear`](https://vdo.ninja/?webcam\&facing=rear)\
\
`&facing` takes priority over [`&videodevice`](../../source-settings/videodevice.md), but it will fail to [`&videodevice`](../../source-settings/videodevice.md) or the default behaviour if the rear/front camera can't be selected automatically. If there are multiple rear or front cameras, it will use the first one. [`&videodevice=0`](../../source-settings/videodevice.md) will disable the video outright.

![](<../../.gitbook/assets/image (43).png>)

## Related

{% content-ref url="and-forcelandscape.md" %}
[and-forcelandscape.md](and-forcelandscape.md)
{% endcontent-ref %}

{% content-ref url="and-forceportrait.md" %}
[and-forceportrait.md](and-forceportrait.md)
{% endcontent-ref %}
