# USBasp-firmware-update
USBasp firmware update using GUI version of avrdude
Need to download the portable version of the AVRdude GUI from: https://github.com/ZakKemble/AVRDUDESS/releases/

1- Short jumper pin 2 of the USBasp that needs to be updated. This would put the board on Program mode.
![test](https://github.com/user-attachments/assets/0e31207b-250b-4e10-8668-248d51e8aaff)


2- Now join the working USBasp to the one that needs firmware update using the ribbon cable.
![test1](https://github.com/user-attachments/assets/484280e8-ef8a-44df-b84c-e29a10398322)

Plug the working USBasp board to the computer’s usb port

Run the GUI version of avrdude which is : AVRDUDESS-2.17-portable
set the:
Programmer: USBasp ISP and TPI programmer
Port: usb
Baud rate 19200
BitClock: 375 Khz
MCU: ATmega8

Flash: the full path of the .HEX firmware, in this case:
C:\Users\HP\Desktop\avrdude - USBasp\usbasp.2011-05-28\bin\firmware\usbasp.atmega8.2011-05-28.hex

select Read to write the firmware to location
select Write to overwrite the firmware with the new one.

![test21](https://github.com/user-attachments/assets/0bea233e-3521-4b5c-af7b-8fcd9180a74d)

