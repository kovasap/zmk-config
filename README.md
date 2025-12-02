# My ZMK configurations

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

## Lintilla

![My Keymap](https://raw.github.com/kovasap/zmk-config/master/lintilla.svg?sanitize=true)

Generated via https://keymap-drawer.streamlit.app/.
