---
title: Cloudflare Tunnel, Zero Trust, and Warp
tags:
  - keyboard
  - QMK
---

## 1. Examining the Standard Office Keyboard

### Pros
- QWERTY is functional and ubiquitous.

### Cons
- Modern computers made keys such as +scroll-lock+, +break+, ++insert, +home+, +delete+, and +end+ more-or-less obsolete. Even when needed, they take your fingers away from the home row and furthermore make the keyboard bigger than it needs to be. 
- Some keys are just poorly designed and thought of:
	- +caps-lock+ is a toggle. It’s the only toggle on the standard keyboard!
	- +shift+ and +control+ are pure modifiers in that they do nothing when single-pressed (the opposite problem of +caps-lock+).
- Whereas the number row also doubles as symbol input; The alphas are just that, only alphas.

!!! question "What am I really missing out on?"

Truth is, not much.

## 2. The Proposed Solution: a QMK Compatible Keyboard

on QMK

At its core, QMK is a firmware for keyboard operations. Its capabilities for advanced customization and configuration sets it apart from anything else readily available. To me, QMK allow for a much more personal interaction with the keyboard, turning a static input device into something more dynamic and adaptive to one's own habits and usage.

Now,

Consider these options as you think about the keyboard you need:
- Do you NEED the numpad or is the number row sufficient?
- Do you NEED the function row?
- Do you NEED dedicated arrow keys or are you okay with using arrow keys as a layer function? Especially consider ditching dedicated arrow keys if you are already used to VIM navgiation. 

Next, consider these choices:

98-key, Tenkeyless, 75%, 65%, and 60%. My preferred layout is 60% and 65% with the former being my favorite for its compactness.


### Buy a QMK Compatible Keyboard

### Adapt Your Existing Keyboard to be QMK Compatible
Hasu’s USB-USB adapter. 
### Build Your Own Custom Keyboard

## 3. The Basic QMK Enhancements

a Brief Interjection on VIA and QMK Configurator

QMK Configurator and VIA are great tools for configuring a basic keymap. Importantly, however, both lack customizations and support for more advanced features of QMK. Hence, all discussions regarding QMK going forward will be based around editing and compiling the keyboard’s QMK source code itself. 

— for a basic starter guide on setting up the QMK build environment, see QMK Firmware’s Docs

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