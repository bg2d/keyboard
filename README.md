# keyboard

This is the "catan" layout that is used on my dactyl manuform 5x6 keyboard.

To change the layout:
* make sure that you have a clone of qmk firmware
* load catan.json on qmk configurator
* change as you wish
* export the new layout in .json format
* create a keymap from the .json file: ``` qmk json2c -o keymap.c catan.json ```
* replace the original keymap.c from *qmk_firmware/keyboards/handwired/dactyl_manuform/5x6/keymaps* with the new one
* build the new firmware: ``` qmk compile -kb handwired/dactyl_manuform/5x6 -km catan ```
* upload the .hex file on MCUs

