# TeleInfo - ST32WB55

[Version Française / French version](README.FR.md)

This project allows to get the information from the French Linky electric meters (and old meters) via the customer tele-information terminals "TIC" and transmit them in Zigbee. The module is powered by the 150mW dedicated power supply of the Linky.


This repository contains the Kicad sources of the PCB and the sources of the Firmware.

## PCB

The PCB is based on :
* A microcontroller [STM32WB55CCU6](https://www.st.com/en/microcontrollers-microprocessors/stm32wb55cc.html) which takes care of the information retrieval and retransmission in Zigbee
* A diode bridge for the conversion of the AC power supply of the linky into DC.
* A linear regulator LM2937-IMP for the conversion in 3.3V
* One SHA620-A octocoupler for serial link recovery from the TeleInfo
* 2 x 5V power supply pins (5V and GND) for the old counters. With a jumper for the choice between Linky/5V
* 5 pins to flash the microcontroller with a st-link (SWD).







