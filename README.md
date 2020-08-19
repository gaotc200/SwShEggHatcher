Simple explaination of how to use 

Tested working with
- **MacOS 10.13.6 (17G10021)** + **dfu-programmer 0.6.2** + **avr-gcc 9.2.0** + **Arduino UNO R3**
- **MacOS 10.15.6 (19G2021)** + **dfu-programmer 0.7.2** + **avr-gcc 9.3.0** + **Arduino UNO R3**

How to use
1. Edit file *Joystick.c*. Under `static const command step[]`, keep "Setup controller" section. Edit under "Start"
1. `make`. This will generate *Joystick.hex* as well as a couple *Joystick.\** files
2. Connect Arduino to Mac
3. Bridge the reset pin with the ground on Arduino
4. `./upload Joystick.hex`
5. (Optional) Save a copy of *Joystick.hex*. You could skip the `make` process and upload the hex file next time.
5. `./rmmake`. This will clear the files from previous `make`. 
