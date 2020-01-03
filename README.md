Testing with
- MacOS 10.13.6 (17G10021)
- dfu-programmer 0.6.2
- avr-gcc 9.2.0
- Arduino UNO R3

1. `make`. This will generate Joystick.hex as well as a couple Joystick.* files
2. Connect Arduino to Mac
3. Bridge the reset pin with the ground on Arduino
4. `./upload Joystick.hex`
5. `./rmmake`. This will clear the files from previous make
