---
description: The screen-share of the guest will have the same label as the guest
---

# \&screensharelabel

Sender-Side Option! ([`&push`](../source-settings/push.md))

## Aliases

* `&sslabel`

## Options

Example: `&screensharelabel=SomeLabel`

<table><thead><tr><th width="245">Value</th><th>Description</th></tr></thead><tbody><tr><td>(no value given)</td><td>Uses the existing <a href="../general-settings/label.md"><code>&#x26;label</code></a> value</td></tr><tr><td>(string)</td><td>Sets the label for the screen share</td></tr></tbody></table>

## Details

Without it set, screen shares do not have a label applied to them. With it added to the guest, it will use the existing [`&label`](../general-settings/label.md) value or whatever value has been passed to it. This changes the default behaviour, but it offers more flexibility and is probably the preferred default behaviour for most users.

## Related

{% content-ref url="../general-settings/label.md" %}
[label.md](../general-settings/label.md)
{% endcontent-ref %}

{% content-ref url="../advanced-settings/design-parameters/showlabels.md" %}
[showlabels.md](../advanced-settings/design-parameters/showlabels.md)
{% endcontent-ref %}
