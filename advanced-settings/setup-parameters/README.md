---
description: >-
  Stream ID, create a room, password, labels, groups, devices, auto-start,
  welcoming guests, sharing a website/file
---

# Setup Parameters

They are separated in two groups: [general options](./#general-options) (push and view) and [source side](./#source-side-options) (push) options.

## General options

You can add them to both, source ([`&push`](../../source-settings/push.md)) and viewer ([`&view`](../view-parameters/view.md), [`&scene`](../view-parameters/scene.md) or [`&solo`](../mixer-scene-parameters/and-solo.md)) sides.

| Parameter                                                   | Explanation                                                                                                                                                 |
| ----------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [`&push`](../../source-settings/push.md)                    | The stream ID that you are publishing with will be the defined value                                                                                        |
| [`&room`](../../general-settings/room.md)                   | Sets a room ID for the session to join                                                                                                                      |
| [`&password`](../../general-settings/password.md)           | Sets a password to view a stream or to join a room                                                                                                          |
| [`&hash`](../../newly-added-parameters/and-hash.md)         | Checks the password                                                                                                                                         |
| [`&label`](../../general-settings/label.md)                 | Sets a display name label                                                                                                                                   |
| [`&labelsuggestion`](and-labelsuggestion.md)\*              | The same as [`&label`](../../general-settings/label.md), except it asks the user still for a user name                                                      |
| [`&permaid`](and-permaid-alpha.md) (alpha)                  | Will save that stream ID to local storage and reuse it every time `&permaid` is used without a stream ID                                                    |
| [`&group`](../../general-settings/and-group.md)             | Puts guests into sub-groups, so they only see others in the same group                                                                                      |
| [`&groupaudio`](../../general-settings/and-groupaudio.md)   | Tells the system to not filter out audio streams when using [`&group`](../../general-settings/and-group.md)                                                 |
| [`&groupview`](and-groupview-alpha.md) (alpha)              | The same as [`&group`](../../general-settings/and-group.md), except it lets you see those groups without actually needing to join them with your mic/camera |
| [`&datamode`](../../newly-added-parameters/and-datamode.md) | Combines a bunch of flags together; no video, no audio, GUI, etc.                                                                                           |
| [`&audiooutput`](and-audiooutput.md)                        | Like [`&sink`](../view-parameters/and-sink.md), but selects the audio output device                                                                         |
| [`&sink`](../view-parameters/and-sink.md)                   | Outputs the audio to the specified audio output device, rather than the default                                                                             |

\*NEW IN VERSION 22

## Source side options

You have to add them to the source side ([`&push`](../../source-settings/push.md)).

| Parameter                                                           | Explanation                                                                                                                                                                                         |
| ------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [`&audiodevice`](../../source-settings/audiodevice.md)              | Pre-configures the selected audio device                                                                                                                                                            |
| [`&videodevice`](../../source-settings/videodevice.md)              | Pre-configures the selected video device                                                                                                                                                            |
| [`&vdo`](../../newly-added-parameters/and-vdo.md)                   | Like [`&videodevice`](../../source-settings/videodevice.md) for selecting a default video device, but you can still choose to change the camera                                                     |
| [`&device`](../../source-settings/and-device.md)                    | Same as [`&audiodevice`](../../source-settings/audiodevice.md) or [`&videodevice`](../../source-settings/videodevice.md), but applies to both                                                       |
| [`&miconly`](../../source-settings/miconly.md)                      | Share audio-only; no video publishing allowed                                                                                                                                                       |
| [`&miconlyoption`](and-miconlyoption-alpha.md) (alpha)              | A mic only button shows if a guest joining a room                                                                                                                                                   |
| [`&safemode`](../../newly-added-parameters/and-safemode.md)         | Tries to load the camera/audio with as little possible complexity as possible                                                                                                                       |
| [`&autostart`](../../source-settings/and-autostart.md)              | Skips the camera/audio device or screenshare selection                                                                                                                                              |
| [`&easyexit`](../../source-settings/easyexit.md)                    | Won't ask the user to confirm that they wish to exit or leave the page                                                                                                                              |
| [`&webcam`](../../source-settings/and-webcam.md)                    | Disables screen-sharing as an option                                                                                                                                                                |
| [`&webcam2`](../../newly-added-parameters/and-webcam2.md)           | Will show the "Share your Camera" button before asking the user to select camera options                                                                                                            |
| [`&screenshare`](../../source-settings/screenshare.md)              | Disables camera-sharing as an option                                                                                                                                                                |
| [`&screenshare2`](../../newly-added-parameters/and-screenshare2.md) | Will show the "Share your Screen" button before asking the user to select screenshare options                                                                                                       |
| [`&website`](../../source-settings/and-website.md)                  | Only shares a website with viewers                                                                                                                                                                  |
| [`&fileshare`](../../source-settings/and-fileshare.md)              | Allows the user to select a video or audio file as a source for streaming                                                                                                                           |
| [`&intro`](../../source-settings/intro.md)                          | When combined with the either [`&webcam`](../../source-settings/and-webcam.md) or [`&screenshare`](../../source-settings/screenshare.md), this option won't auto-load the camera/mic selection page |
| [`&host`](../../newly-added-parameters/and-host.md)                 | Shows a pop up to invite more guests to the room                                                                                                                                                    |
| [`&tips`](../../general-settings/tips.md)                           | Shows a help-screen on the guest joining                                                                                                                                                            |
| [`&welcome`](../../newly-added-parameters/and-welcome.md)           | Adds a message the guest will see when joining the room                                                                                                                                             |
| [`&welcomeimage`](and-welcomeimage.md)\*                            | Lets you specify an image that appears for a few seconds once a guest joins                                                                                                                         |
| [`&groupmode`](and-groupmode.md)\*                                  | Added to the URL, when not assigned to a group, you don't hear or see anything                                                                                                                      |

\*NEW IN VERSION 22
