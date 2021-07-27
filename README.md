# ender3-marlin
Install marlin on an ender3 with the Creality New Upgrade Silent Mainboard V4.2.7

## Compile the firmware

0. Install VScode and PlatfromIO
1. Clone the latest version marlin with `git clone https://github.com/MarlinFirmware/Marlin.git`
2. Go into Marlin/ and run `git checkout bugfix-2.0.x` to change th branch
3. Download the `Configuration.h` and the `Configuration_adv.h` from this repository and place them Marlin/Marlin
4. Change the parameter `default_envs` from `mega2560` to `STM32F103RET6_creality` in the `platformio.ini` -file
5. Hit compile
6. You can find your firmware in `Marlin/.pio/build/STM32F103RET6_creality`. The file is called `firmware-XXXXXXX-XXXXX.bin`


## Upload the firmware
Copy your compliled firmware or the binary-file from this repository onto an empty sd-card, plug it into your printer and printer on.

## Links/Sources
* [http://813studios.com/creality-4-2-7-marlin-bltouch-install-notes-ender-3/](http://813studios.com/creality-4-2-7-marlin-bltouch-install-notes-ender-3/)
* [https://github.com/Flawioo/Creality-Ender-3-board-v4.2.7](https://github.com/Flawioo/Creality-Ender-3-board-v4.2.7)
* [Original firmware](https://drive.google.com/drive/folders/1sQ9TnIfssNy42rfK-DcJtLlkd30sUy6V)