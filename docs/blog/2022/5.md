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