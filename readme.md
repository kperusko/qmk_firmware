# Quickstart for Sofle RGB with rp2040

## Install & Setup

```
brew install qmk/qmk/qmk
qmk setup
```

## Compilling and Flashing

This will compile the kperusko keyboard mapping for for the sofle rgb keyboard

```
qmk compile -kb sofle -km rgb_kperusko
```

This will flash the keyboard and convert it to support Raspberry PI 2040 version hardware

```
qmk flash -kb sofle -km rgb_kperusko -e CONVERT_TO=promicro_rp2040
```

Note: To put the board in the bootloader mode, quickly press reset button twice.

## Troubleshooting

If the board is not recognized over USB and won't go into bootloader mode a factory reset is needed. Remove the controller from the board and press and hold the bootloader switch while plugging in the USB (bootloader switch is the left one, when the usb is on the top). Board will be recognized as external storage. Drag and drop the Blink.ino.elf.uf2 file (from the root of this repo) and the controller will reset. This only worked on Windows though. 


# Quantum Mechanical Keyboard Firmware

[![Current Version](https://img.shields.io/github/tag/qmk/qmk_firmware.svg)](https://github.com/qmk/qmk_firmware/tags)
[![Discord](https://img.shields.io/discord/440868230475677696.svg)](https://discord.gg/Uq7gcHh)
[![Docs Status](https://img.shields.io/badge/docs-ready-orange.svg)](https://docs.qmk.fm)
[![GitHub contributors](https://img.shields.io/github/contributors/qmk/qmk_firmware.svg)](https://github.com/qmk/qmk_firmware/pulse/monthly)
[![GitHub forks](https://img.shields.io/github/forks/qmk/qmk_firmware.svg?style=social&label=Fork)](https://github.com/qmk/qmk_firmware/)

This is a keyboard firmware based on the [tmk_keyboard firmware](https://github.com/tmk/tmk_keyboard) with some useful features for Atmel AVR and ARM controllers, and more specifically, the [OLKB product line](https://olkb.com), the [ErgoDox EZ](https://ergodox-ez.com) keyboard, and the [Clueboard product line](https://clueboard.co).

## Documentation

-   [See the official documentation on docs.qmk.fm](https://docs.qmk.fm)

The docs are powered by [Docsify](https://docsify.js.org/) and hosted on [GitHub](/docs/). They are also viewable offline; see [Previewing the Documentation](https://docs.qmk.fm/#/contributing?id=previewing-the-documentation) for more details.

You can request changes by making a fork and opening a [pull request](https://github.com/qmk/qmk_firmware/pulls), or by clicking the "Edit this page" link at the bottom of any page.

## Supported Keyboards

-   [Planck](/keyboards/planck/)
-   [Preonic](/keyboards/preonic/)
-   [ErgoDox EZ](/keyboards/ergodox_ez/)
-   [Clueboard](/keyboards/clueboard/)
-   [Cluepad](/keyboards/clueboard/17/)
-   [Atreus](/keyboards/atreus/)

The project also includes community support for [lots of other keyboards](/keyboards/).

## Maintainers

QMK is developed and maintained by Jack Humbert of OLKB with contributions from the community, and of course, [Hasu](https://github.com/tmk). The OLKB product firmwares are maintained by [Jack Humbert](https://github.com/jackhumbert), the Ergodox EZ by [ZSA Technology Labs](https://github.com/zsa), the Clueboard by [Zach White](https://github.com/skullydazed), and the Atreus by [Phil Hagelberg](https://github.com/technomancy).

## Official Website

[qmk.fm](https://qmk.fm) is the official website of QMK, where you can find links to this page, the documentation, and the keyboards supported by QMK.

```

```
