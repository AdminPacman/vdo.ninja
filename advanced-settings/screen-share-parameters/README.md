---
description: Labels, audio filters, type, bitrate, quality etc.
---

# Screen-share Parameters

Screen-share Parameters are separated in [general options](./#general-options), [source side](./#source-side-options) (push) options and [viewer side](./#viewer-side-options) (view) options.

## General options

You can add them to both, source ([`&push`](../../source-settings/push.md)) and viewer ([`&view`](../view-parameters/view.md) or [`&scene`](../view-parameters/scene.md)) sides.

| Parameter                                                                     | Explanation                                                                                                 |
| ----------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------- |
| [`&screensharestereo`](../../newly-added-parameters/and-screensharestereo.md) | Sets the audio mode for screen-shares to stereo and changes default audio settings to improve audio quality |

## Source side options

You can add them to both, source ([`&push`](../../source-settings/push.md)) and viewer ([`&view`](../view-parameters/view.md) or [`&scene`](../view-parameters/scene.md)) sides.

| Parameter                                                                           | Explanation                                                                                                 |
| ----------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------- |
| [`&screenshare`](../../source-settings/screenshare.md)                              | Disables camera-sharing as an option                                                                        |
| [`&screenshare2`](../../newly-added-parameters/and-screenshare2.md)                 | Will show the "Share your Screen" button before asking the user to select screenshare options               |
| [`&screenshareaec`](../../newly-added-parameters/and-screenshareaec.md)             | Turns automatic echo-cancellation filter for screen-shares ON or OFF                                        |
| [`&screenshareautogain`](../../newly-added-parameters/and-screenshareautogain.md)   | Turns audio auto-normalization filter for screen-shares ON or OFF                                           |
| [`&screensharecursor`](../../source-settings/cursor.md)                             | Attempts to show the mouse cursor on screen shares                                                          |
| [`&screensharedenoise`](../../newly-added-parameters/and-screensharedenoise.md)     | Turns audio noise reduction filter for screen-shares ON or OFF                                              |
| [`&screensharefps`](../../source-settings/screensharefps.md)                        | Set a target FPS for your screenshare (secondary stream)                                                    |
| [`&screensharehide`](../../newly-added-parameters/and-screensharehide.md)           | Hides the local screen-share sub-window that appears when screen sharing in a room                          |
| [`&screenshareid`](../../source-settings/screenshareid.md)                          | Pre-sets the screenshare stream id for a screen share if its a secondary stream                             |
| [`&screensharelabel`](../../newly-added-parameters/and-screensharelabel.md)         | The screen-share of the guest will have the same label as the guest                                         |
| [`&screensharequality`](../../source-settings/screensharequality.md)                | Set a custom screenshare quality                                                                            |
| [`&screensharecontenthint`](and-screensharecontenthint.md)\*                        | `=motion` prioritizes screen-share frame rate; `=detail` prioritizes screen-share resolution                |
| [`&screenshareaspectratio`](and-screenshareaspectratio.md)\*                        | Changes the screen-share aspect ratio on the publisher side                                                 |
| [`&screensharestereo`](../../newly-added-parameters/and-screensharestereo.md)       | Sets the audio mode for screen-shares to stereo and changes default audio settings to improve audio quality |
| [`&screensharetype`](../../newly-added-parameters/and-screensharetype.md)           | Defines how webcam and screenshare of a guest in a room interacts which each other                          |
| [`&smallshare`](and-smallshare.md)\*                                                | Makes the screen share behave like a webcam share                                                           |
| [`&screensharevideoonly`](../../newly-added-parameters/and-screensharevideoonly.md) | Lets you disable the option to select audio when screen sharing                                             |
| [`&screensharebutton`](../settings-parameters/and-screensharebutton.md)             | Forces the screen-share button to appear for guests                                                         |
| [`&suppresslocalaudio`](and-suppresslocalaudio.md) (alpha)                          | Will disable local audio playback of a Chrome tab while screen-sharing it                                   |
| [`&prefercurrenttab`](and-prefercurrenttab.md) (alpha)                              | Will have the current tab as the default screen-share source                                                |
| [`&selfbrowsersurface`](and-selfbrowsersurface.md) (alpha)                          | Excludes the current tab as a screen-share source option                                                    |
| [`&systemaudio`](and-systemaudio.md) (alpha)                                        | Excludes the system-audio as an audio source when display sharing                                           |
| [`&displaysurface`](and-displaysurface.md) (alpha)                                  | Will pre-select display-share, rather than tab-share, when screen-sharing                                   |

\*NEW IN VERSION 22

## **Viewer side options**

You have to add them to the viewer side ([`&view`](../view-parameters/view.md) or [`&scene`](../view-parameters/scene.md)).

| Parameter                                                                       | Explanation                                                                  |
| ------------------------------------------------------------------------------- | ---------------------------------------------------------------------------- |
| [`&screensharebitrate`](../../newly-added-parameters/and-screensharebitrate.md) | Lets you manually set the video bitrate for screen-shares                    |
| [`&sharperscreen`](and-sharperscreen.md)\*                                      | Sets [`&scale=100`](../view-parameters/scale.md), but only for screen-shares |
| [`&sspaused`](../../parameters-only-on-beta/and-sspaused.md)                    | Starts any screen-share paused                                               |

\*NEW IN VERSION 22
