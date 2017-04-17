Handwired Atreus50
==================

This firmware is for a Handwired Atreus50 using an Arduino Pro Micro.

## Pinout

The following pins are used:
- Columns 1-13: D4, D7, E6, B4, B5, B6, B2, B3, B1, F7, F6, F5, F4
- Rows 1-4: D3, D2, D1, D0

## QuickStart

###Mac OSX
1. Install AVR, avrdude and DFU-Programmer
```bash
$ brew tap osx-cross/avr
$ brew install avr-libc
$ brew install dfu-programmer
$ brew install avrdude
```

2. Clone this repository
```bash
$ git clone https://github.com/qmk/qmk_firmware
```

3. Navigate to the default Atreus50 keymap
```bash
$ cd qmk_firmware/keyboards/handwired/atreus50/keymaps/default
```

4. Build the firmware and ensure no errors are outputted
```bash
$ make
```

5. Connect your keyboard to your computer over USB

6. Flash your firmware onto your keyboard with `avrdude` 
```bash
$ make avrdude
```
## Compiling and loading the firmware

To build the firmware, run `make`.

To flash the firemware onto the microcontroller, run `make avrdude`, and press the reset button.
