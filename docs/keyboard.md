Now,

Remove/Ignore PrintScrn, ScrollLock, Pause/Break, Insert, Home, Delete, End, PageUp/PageDown entirely, consider the Leopold FC980C’s layout.

Make CapsLock an addtional modifier (CapsLock when tapped, modifier otherwise). Here, there are two options:

a hyper modifier: combine inputs of common, but impractical modifier combinations such as ++shift+control+lsuper+lalt++.

a layer modifier: momentary switch of keyboard layer when held. This is the preferred behavior.

Keep the Super function when single-pressed, but change its hold function from Super (Win) to the modifier opposite of what’s been chosen above (now preferably the hyper modifier).

Change +lshift+ and +rshift+ into Space Cadet Shift. I chose ( and ) myself as it’s most practical in common writing, coding, and especially markdown.

## 4. Layering and Implementing Common PC Functions

— 1 layer is too little, 3 too many. 2, then, is the sweet spot.

Consider the following common PC actions that do not have a spot on the keyboard:

Volume Adjustment

Pause/Play and Next/Previous

If your chosen layout does not have arrow or function keys, an addition is also perfect for reimplementing them in more convenient spots.

An additional layer is also great for reiterating the key group of PrintScrn, ScrollLock, Pause/Break, Insert, Home, Delete, End, PageUp/PageDown.

## 5. Advanced Functions and Power Implementations

Consider these deeper, highly focused features of QMK:

Leader Key - patterned key sequencing to trigger an action

Tap Dance - trigger an action upon the amount of times pressed

Combos - mutiple keys at once (chording) to trigger an action

Macros - repeatable sequences with one key press

## 6. The Final Core Keymap

References:

The Official QMK Firmware’s Docs

Thomas Baart’s QMK Articles


https://github.com/qmk/qmk_firmware/blob/master/docs/feature_space_cadet.md
https://github.com/qmk/qmk_firmware/blob/master/docs/feature_leader_key.md
https://github.com/samhocevar-forks/qmk-firmware/blob/master/docs/feature_tap_dance.md
https://github.com/qmk/qmk_firmware/blob/master/docs/feature_combo.md
https://github.com/qmk/qmk_firmware/blob/master/docs/feature_macros.md