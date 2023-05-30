---
description: Option to change codec of the &meshcast parameter while screen-sharing
---

# \&mcscreensharecodec

Meshcast Option / Sender-Side Option! ([`&meshcast`](../newly-added-parameters/and-meshcast.md), [`&push`](../source-settings/push.md))

## Aliases

* `&mcsscodec`

## Options

Example: `&mcscreensharecodec=h264`

<table><thead><tr><th width="234">Value</th><th>Description</th></tr></thead><tbody><tr><td><code>h264</code></td><td>h264 codec</td></tr><tr><td><code>vp8</code></td><td>vp8 codec</td></tr><tr><td><code>vp9</code></td><td>vp9 codec</td></tr><tr><td><code>42e01f</code>*</td><td>open h264 codec</td></tr><tr><td>(xxxxxx)*</td><td>h264 profile IDs</td></tr></tbody></table>

\*on beta and alpha

## Details

Adding `&mcsceensharecodec` to the publisher's side together with [`&meshcast`](../newly-added-parameters/and-meshcast.md) gives the option to change the publishing codec while screen-sharing via meshcast.

Example usage: `https://vdo.ninja/?meshcast&mcscreensharecodec=vp8`

There's 4 codec options currently, including the default option:

* The unspecified default, which is software h264.&#x20;
* There's also `h264`, which is what the browser then sets. This could include hardware encoding, but that will not work with Firefox or Safari viewers then.&#x20;
* `vp8` is pretty compatible, so if the default codec doesn't work, you can try that.&#x20;
* `vp9` is also available, which has better compression/quality, but not fully compatible with all devices.&#x20;
* av1 and svc are not yet supported, but that is planned at some point.

## Related

{% content-ref url="../newly-added-parameters/and-meshcast.md" %}
[and-meshcast.md](../newly-added-parameters/and-meshcast.md)
{% endcontent-ref %}

{% content-ref url="and-mcscreensharebitrate.md" %}
[and-mcscreensharebitrate.md](and-mcscreensharebitrate.md)
{% endcontent-ref %}

{% content-ref url="and-meshcastcodec.md" %}
[and-meshcastcodec.md](and-meshcastcodec.md)
{% endcontent-ref %}

{% content-ref url="../advanced-settings/view-parameters/codec.md" %}
[codec.md](../advanced-settings/view-parameters/codec.md)
{% endcontent-ref %}

{% content-ref url="../newly-added-parameters/and-h264profile.md" %}
[and-h264profile.md](../newly-added-parameters/and-h264profile.md)
{% endcontent-ref %}
