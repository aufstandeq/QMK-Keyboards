# Programming your Mechanical Keyboard
## Introduction
This section is focused on programming your mechanical keyboard. You have either purchased a keyboard that supports custom programming or you have successfully constructed your own keyboard and this is the next logical step.

QMK stands for Quantum Mechanical Keyboard and it is the framework that we are leveraging to program the firmware on the keyboard. QMK was developed and is maintained by **Jack Humbert** of OLKB with contributions from the community, and of course, [**Hasu**](https://github.com/tmk). The OLKB product firmwares are maintained by [**Jack Humbert**](https://github.com/jackhumbert), the Ergodox EZ by [**Erez Zukerman**](https://github.com/ezuk), the Clueboard by [**Zach White**](https://github.com/skullydazed), and the Atreus by [**Phil Hagelberg**](https://github.com/technomancy).

The QMK framework is an extension of the TMK keyboard framework originally written by [**Hasu**](https://github.com/tmk). QMK was started by [**Jack Humbert**](https://github.com/jackhumbert) and has not grown in to a community project. It is the default firmware for all OLKB boards, the clueboard line, and the Ergodox EZ. It supports most AVR and ARM chips.

The open source community maintains the QMK firmware and toolbox, etc at [http://docs.qmk.fm](http://docs.qmk.fm)

## The Printed Circuit Board
The PCB is discussed in the hardware section, but what is important now is the microprocessor. We want to know the number on the chip. The number is required when we want to flash the new firmware to the keyboard.

> Add image from my boards

You can also check online to make sure your board supports QMK firmware. [QMK firmware supported keyboard page](https://qmk.fm/keyboards/).

## How do I setup my development environment?
### Easiest way to start.
What is the easiest way for you to get started with remapping your keyboard? This is the purpose of this section here.

The development environment, per se, is a tool to create the HEX file, a tool to flash the keyboard, and a tool to test that the mapping worked.

# Map our Keyboards
Create the keyboard mapping for each level you would like

I tested two tools for mapping my new keyboard.

1. [Keyboard Firmware Builder](http://kbfirmware.com/)
2. [QMK Configurator](https://config.qmk.fm/#/1upkeyboards/1up60hse/LAYOUT_60_ansi)

## Keyboard Firmware Builder
I found this one to be really simple and worked each time.

1. Open the [**Keyboard Firmware Builder**](http://kbfirmware.com/)
2. I used the Underglow PCB board from [**1 UP**](http://1upkeyboards.com) which in the webpage provides a [**default KBFirmware layout file**](https://1upkeyboards.com/1up_rgb_custom_pcb_standard_map.json)
3. Download the file and in the tool select **Upload** and select the default file.
  - This file will now work on QMK Configurator
4. Click on the **PINS** table below the keyboard. This is where we want to validate the microprocessor.
  - E.G. my board is the ATmega32U4
5. Click **KEYMAP**. This is where you can change the keys and laters.
  - See the section on programming keys below
  - The QMK site provides a full list of [keycodes](https://docs.qmk.fm/#/keycodes) are available online as well
6. Skip to the **SETTINGS** tab and in the first field - Layout Name - change the name of the file. Use a logical naming convention.
7. Save the configuration file
8. Click on the **COMPILE** tab and download the HEX file.

***END***

## QMK Configurator
The configuration tool is another way to build the same HEX file that we need to update the firmware.

1. Open the [QMK Configurator](https://config.qmk.fm/#/1upkeyboards/1up60hse/LAYOUT_60_ansi) website

***END***

# Flash the Firmware on the Keyboards
Now upload the keyboard mapping to the keyboard


# Test the new firmware
Finally test the keyboard and make sure everything is working.
