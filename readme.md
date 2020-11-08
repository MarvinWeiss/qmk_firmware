# Quantum Mechanical Keyboard Firmware

[![Current Version](https://img.shields.io/github/tag/qmk/qmk_firmware.svg)](https://github.com/qmk/qmk_firmware/tags)
[![Build Status](https://travis-ci.org/qmk/qmk_firmware.svg?branch=master)](https://travis-ci.org/qmk/qmk_firmware)
[![Discord](https://img.shields.io/discord/440868230475677696.svg)](https://discord.gg/Uq7gcHh)
[![Docs Status](https://img.shields.io/badge/docs-ready-orange.svg)](https://docs.qmk.fm)
[![GitHub contributors](https://img.shields.io/github/contributors/qmk/qmk_firmware.svg)](https://github.com/qmk/qmk_firmware/pulse/monthly)
[![GitHub forks](https://img.shields.io/github/forks/qmk/qmk_firmware.svg?style=social&label=Fork)](https://github.com/qmk/qmk_firmware/)

This is a keyboard firmware based on the [tmk\_keyboard firmware](https://github.com/tmk/tmk_keyboard) with some useful features for Atmel AVR and ARM controllers, and more specifically, the [OLKB product line](https://olkb.com), the [ErgoDox EZ](https://ergodox-ez.com) keyboard, and the [Clueboard product line](https://clueboard.co).

## Documentation

* [See the official documentation on docs.qmk.fm](https://docs.qmk.fm)

The docs are powered by [Docsify](https://docsify.js.org/) and hosted on [GitHub](/docs/). They are also viewable offline; see [Previewing the Documentation](https://docs.qmk.fm/#/contributing?id=previewing-the-documentation) for more details.

You can request changes by making a fork and opening a [pull request](https://github.com/qmk/qmk_firmware/pulls), or by clicking the "Edit this page" link at the bottom of any page.

## Supported Keyboards

* [Planck](/keyboards/planck/)
* [Preonic](/keyboards/preonic/)
* [ErgoDox EZ](/keyboards/ergodox_ez/)
* [Clueboard](/keyboards/clueboard/)
* [Cluepad](/keyboards/clueboard/17/)
* [Atreus](/keyboards/atreus/)

The project also includes community support for [lots of other keyboards](/keyboards/).

## Maintainers

QMK is developed and maintained by Jack Humbert of OLKB with contributions from the community, and of course, [Hasu](https://github.com/tmk). The OLKB product firmwares are maintained by [Jack Humbert](https://github.com/jackhumbert), the Ergodox EZ by [ZSA Technology Labs](https://github.com/zsa), the Clueboard by [Zach White](https://github.com/skullydazed), and the Atreus by [Phil Hagelberg](https://github.com/technomancy).

## Official Website

[qmk.fm](https://qmk.fm) is the official website of QMK, where you can find links to this page, the documentation, and the keyboards supported by QMK.

## Custom Layout (German, osx and windows)
I removed the Colemak and Dovark Layouts because I'm fine with the german qwertz layout for now. The quertz layout has the most special signs same as a normal keyboard, only *+'# needet to be placed on the ü and ä key and can be reached by the lower layers 

Qwertz
 ,-----------------------------------------------------------------------------------.
 |   1  |   2  |   3  |   4  |   5  |   6  |   7  |   8  |   9  |   0  |   ß  | Bksp |
 |------+------+------+------+------+------+------+------+------+------+------+------|
 | Esc  |   Q  |   W  |   E  |   R  |   T  |   Z  |   U  |   I  |   O  |   P  |   Ü  |
 |------+------+------+------+------+-------------+------+------+------+------+------|
 |  Tab |   A  |   S  |   D  |   F  |   G  |   H  |   J  |   K  |   L  |   Ö  |   Ä  |
 |------+------+------+------+------+------|------+------+------+------+------+------|
 | Shift|   Y  |   X  |   C  |   V  |   B  |   N  |   M  |   ,  |   .  |   -  |Enter |
 |------+------+------+------+------+------+------+------+------+------+------+------|
 | Ctrl | Alt  | CMD  | CMD  | Lower|    Space    |Raise | Left | Down |  Up  |Right |
 `-----------------------------------------------------------------------------------'
 

 Lower
 ,-----------------------------------------------------------------------------------.
 |   ~  |   !  |   @  |   #  |   $  |   %  |   ^  |   &  |   *  |   (  |   )  | Bksp |
 |------+------+------+------+------+-------------+------+------+------+------+------|
 |   ~  |   !  |   @  |   #  |   $  |   %  |   ^  |   &  |   *  |   (  |   )  | Del  |
 |------+------+------+------+------+-------------+------+------+------+------+------|
 | Del  |  F1  |  F2  |  F3  |  F4  |  F5  |  F6  |   _  |   +  |   {  |   }  |  |   |
 |------+------+------+------+------+------|------+------+------+------+------+------|
 |      |  <>  |  F8  |  F9  |  F10 |  F11 |  F12 |ISO ~ | Pause| BrDn | BrUp | Mute |
 |------+------+------+------+------+------+------+------+------+------+------+------|
 |      |      |      |      |      |             |      | Prev | Vol- | Vol+ | Next |
 `-----------------------------------------------------------------------------------'



Raise
 ,-----------------------------------------------------------------------------------.
 |   `  |   1  |   2  |   3  |   4  |   5  |   6  |   7  |   8  |   9  |   0  | Bksp |
 |------+------+------+------+------+------+------+------+------+------+------+------|
 |   `  |   1  |   2  |   3  |   4  |   5  |   6  |   7  |   8  |   9  |   0  |   +  |
 |------+------+------+------+------+-------------+------+------+------+------+------|
 | Del  |  F1  |  F2  |  F3  |  F4  |  F5  |  F6  |   -  |   =  |   [  |   ]  |   #  |
 |------+------+------+------+------+------|------+------+------+------+------+------|
 |      |  F7  |  F8  |  F9  |  F10 |  F11 |  F12 |ISO # | Pause| BrDn | BrUp | Mute |
 |------+------+------+------+------+------+------+------+------+------+------+------|
 |      |      |      |      |      |             |      | Prev | Vol- | Vol+ | Next |
 `-----------------------------------------------------------------------------------'
 

 Adjust (Lower + Raise)
 ,-----------------------------------------------------------------------------------.
 |  F1  |  F2  |  F3  |  F4  |  F5  |  F6  |  F7  |  F8  |  F9  |  F10 |  F11 |sleep |
 |------+------+------+------+------+------+------+------+------+------+------+------|
 |  F12 | Reset| Debug|      |      |      |      |      |      |      |      |  Del |
 |------+------+------+------+------+-------------+------+------+------+------+------|
 |RGBTog|      |      |Aud on|AudOff|AGnorm|AGswap|QWERTZ|      |      |      |      |
 |------+------+------+------+------+------|------+------+------+------+------+------|
 |      |Voice-|Voice+|Mus on|MusOff|MidiOn|MidOff|      |      |      |      |      |
 |------+------+------+------+------+------+------+------+------+------+------+------|
 |      |      |      |      |      |             |      |      |      |      |      |
 `-----------------------------------------------------------------------------------'
 