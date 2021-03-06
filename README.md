# Keyboard localization package for non US-Keyboard Layouts
This is a compatibility package for atom text editor which tries to remap keycodes for your given keyboard layout.

## Whats working
* Prevent default keybindings from being fired
* Keybindings in your foreign keyboard layout
* AltGr-Key (works for me on german layout)
* vim-mode keybindings
* tested on Windows and Linux

## Supported Keyboard Layouts atm
* [German 105-key "QWERTZ"](http://en.wikipedia.org/wiki/File:KB_Germany.svg) (`de_DE`)
* [German Neo-Layout](http://www.neo-layout.org/) (`de_DE-neo`)
* [Spanish](https://www.terena.org/activities/multiling/ml-mua/test/img/kbd_spanish.gif) (`es_ES`) - untested
* [French](https://www.terena.org/activities/multiling/ml-mua/test/img/kbd_french.gif) (`fr_FR`)
* [Belgian French](https://upload.wikimedia.org/wikipedia/commons/9/93/Belgian_keyboard_layout.png) (`fr_BE`)
* [Canadian French](http://i.stack.imgur.com/ryQxs.png) (`fr_CA`)
* [Polish](https://www.terena.org/activities/multiling/ml-mua/test/img/kbd_polish.gif) (`pl_PL`) - untested
* [Danish](http://fontmeme.com/images/danish-keyboard-550x183.png) (`da_DK`) - untested
* [Norwegian](http://upload.wikimedia.org/wikipedia/commons/thumb/c/c9/KB_Norway.svg/2000px-KB_Norway.svg.png) (`nb_NO`) - untested
* [Swedish](http://frontype.com/keyboarding/540px-Computer-keyboard-Sweden.svg.png) (`sv_SE`) - untested
* [Hungarian](https://www.terena.org/activities/multiling/ml-mua/test/img/kbd_hungary.gif) (`hu_HU`) - untested
* [Romanian](http://upload.wikimedia.org/wikipedia/commons/f/f0/Romanian-keyboard-layout.png) (`ro_RO`) - untested
* [Slovenian](http://smotko.si/assets/pics/keyboard.png) (`sl_SL`) - untested
* [Italian](https://www.terena.org/activities/multiling/ml-mua/test/img/kbd_italian.gif) (`it_IT`)
* [Portuguese](https://www.terena.org/activities/multiling/ml-mua/test/img/kbd_portug.gif) (`pt_PT`) - untested


Feel free to send me Issues/PRs so i can add more keymaps.

## Generate your own keymap
You can generate your own localized key-translation-table for your keyboard layout.
Open the generator `keybinding-generator\generate-keybindings.html` included in this package in Chrome(other Browsers may not work) and press all keys(with and without modifiers Shift/Alt) from your keyboard who differ from the US-Layout. Copy the generated JSON-keybindings and create a Json-File.
Then set the package setting `UseKeyboardLayoutFromPath` to your given filename(absolute path).

## Todo
* add more foreign Keyboard-Layouts
* write tests
* ~~add custom path for keymap file~~

## This package tries to fill the gap till the following issues are fixed
* [Chromium Issue 263724: KeyboardEvent does not match the latest specification](https://code.google.com/p/chromium/issues/detail?id=263724)
* [Chromium Issue 300475: Issues with non US keyboard layout keyboard events or editing](https://code.google.com/p/chromium/issues/detail?id=300475)
* [Chromium Issue 168971: Implement 'locale' attribute in KeyboardEvent](https://code.google.com/p/chromium/issues/detail?id=168971)
* [Atom Issue 35: Right ALT not supported (bad for International Keyboards)](https://github.com/atom/atom-keymap/issues/35)
* [Atom Issue 37: Foreign keyboard layouts not working](https://github.com/atom/atom-keymap/issues/37)

## Credits
All thanks go to original author -> [DavidBadura](https://github.com/DavidBadura)
