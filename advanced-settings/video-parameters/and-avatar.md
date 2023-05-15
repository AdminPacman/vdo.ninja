---
description: Adds the ability to select an image, instead of a video device
---

# \&avatar

Sender-Side Option! ([`&push`](../../source-settings/push.md))\
\* on [https://vdo.ninja/beta/](https://vdo.ninja/beta/) and [https://vdo.ninja/alpha/](https://vdo.ninja/alpha/)

## Options

Example: `&avatar=default`

| Value            | Description                                                            |
| ---------------- | ---------------------------------------------------------------------- |
| (no value given) | adds the ability to select an image, instead of a video device         |
| (encoded URL)    | pre-selects the chosen image as an avatar                              |
| `default`        | will pre-select the default avatar, rather than leaving it un-selected |

## Details

`&avatar` adds the ability to select an image, instead of a video device. The image will trigger when the video is muted or no video device is selected. A default avatar image is provided, but you can select your own from disk. `&avatar=default` will pre-select the default avatar, rather than leaving it un-selected.

![](<../../.gitbook/assets/image (104) (1) (1).png>)

You can toggle it for the guest's invite link in the director's room:\
![](<../../.gitbook/assets/image (118) (1).png>)

You can encode your URL here:\
[https://www.urlencoder.org/](https://www.urlencoder.org/)

### Director

Choosing the default avatar / placeholder image is activated for the director on default

<figure><img src="../../.gitbook/assets/image (6) (3).png" alt=""><figcaption></figcaption></figure>

## Related

{% content-ref url="../newly-added-parameters/and-waitimage.md" %}
[and-waitimage.md](../newly-added-parameters/and-waitimage.md)
{% endcontent-ref %}

{% content-ref url="../design-parameters/and-bgimage.md" %}
[and-bgimage.md](../design-parameters/and-bgimage.md)
{% endcontent-ref %}
