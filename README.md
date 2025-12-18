# My ZMK configurations

Currently I use the Lintilla.

## Keymap Learnings

Home row mods lead to too many false presses for me.
In fact, any mod that requires timings of any kind (auto-shift, sticky layer on
the same key that toggles another layer while held) I find quite annoying.

Combos are great, but only when the keys in the combo are all normally
controlled by the same finger.
This means to trigger the combo I need to hit two keys with one finger, or move
fingers to help by pressing keys normally out of their zone of control.
When not following this rule, I get false presses frequently during normal
typing.
Combos where the keys are too far away (e.g. thumb and pinky combos) are a bit
annoying to use.

## Technical Notes

Quickly download firmware after it is built by github actions after a push to
this repo.

```bash
gh run download -R kovasap/zmk-config -n firmware
```

To flash, double tap the small reset button on each half while plugged in with
usb, then copy the firmware files to the "usb drives" your computer should
detect.

## Bluetooth

If you get a persistent "pairing failed" error when trying to pair, clear all bluetooth profiles by holding down each of their keys in turn.
Then switch to your desired profile by tapping the key and try again.

## Lintilla Keymap

![My Keymap](https://raw.github.com/kovasap/zmk-config/master/lintilla.svg?sanitize=true)

Generated via https://keymap-drawer.streamlit.app/.

To draw on command line, run:

```
pipx install keymap-drawer
keymap parse -c 12 -z config/lintilla.keymap > lintilla_keymap.yaml
keymap draw lintilla_keymap.yaml > lintilla.svg
```
