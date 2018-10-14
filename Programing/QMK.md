# Leveraging QMK for Programming the Keyboard

## What is QMK?
QMK or Quantum Mechanical Keyboard is firmware based on the TMK keyboard framework and additional features added. It provides support and the ability to customize your own PCB keyboard.

QMK is developed and maintained by Jack Humbert of OLKB with contributions from the community, and of course, [Hasu](https://github.com/tmk). The OLKB product firmwares are maintained by [Jack Humbert](https://github.com/jackhumbert), the Ergodox EZ by [Erez Zukerman](https://github.com/ezuk), the Clueboard by [Zach White](https://github.com/skullydazed), and the Atreus by [Phil Hagelberg](https://github.com/technomancy)

### The TMK keyboard framework
The original or base framework that the QMK framework extends. I find it harder to locate supporting information for this framework. This is another good reason why you will want the QMK framework for your projects.

### What is a PCB Board?
The PCB board or [Printed Circuit Board](https://en.wikipedia.org/wiki/Printed_circuit_board) is a printed board that provides us the ability to fasten to it and also the pathways already etched in to the board.  

### Who Maintains this Framework?
The open source community maintains the QMK firmware and toolbox, etc at [http://docs.qmk.fm](http://docs.qmk.fm)

### Check if your board supports QMK
It is a safe bet that support is available if you built your own keyboard. Just incase you can check on the [QMK firmware supported keyboard page](https://qmk.fm/keyboards/).

## How do I setup my development environment?
### Easiest way to start.
What is the easiest way for you to get started with remapping your keyboard? This is the purpose of this section here.

Get some tools
- **Text Editor**, I recommend ATOM, but you can use notepad or any other tools that you like.
- **QMK Toolbox**, a graphics UI that allows you to map and test your keyboard
- **Keyboard Tester**
- **QMK Configurator**, there is also a tool http://kbfirmware.com/ that one up recommended on their site. There are basic JSON files to upload to start the modification as well. Still created a HEX file.

> Used the kbfirmware builder and I was able to create a new hex mapping and get it uploaded. Very easy tool to begin with for changing your mapping.

#### QMK Toolbox
[Current Release](https://github.com/qmk/qmk_toolbox/releases/tag/0.0.9)
Download qmk_toolbox_install.exe

### QMK Configurator
The web based UI tool allows you to map the keyboard and create a new layout. It supports creating multiple layers abd allows you to save drafts or export the hex file.

1. Map the keys
2. Set the keys on the layers
3. Make sure you have the key to switch layers
4. Name the file in the top right
5. Complie and
6. Download the firmware

### qmk_toolbox
1. Open the toolbox that was installed earlier
2.


## What do the key codes mean
https://docs.qmk.fm/#/keycodes


### Diving a bit deeper
What can I do beyond the basics?
