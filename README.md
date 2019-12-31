# Kylra's-Motion-Controller


The preliminary schematics are not tested and can contain errors.


## Motion Controller Diagramm:
An overview of the Board(s).


## TinyK 8L V1.00_Schematic Preliminary_03112019
Hardware Version 1.00

Version 1.00 don't contain the pressure sensor, differential I2C and RS485.
It will be updated.

Specification (V1.10):
Main voltage: 24VDC with over voltage protection
Motor voltage: 4.75V to 46V DC
32bit ARM STM32H743 MCU, 480 MHz
4x TMC5130A motor drivers (2A, 2.5A peak) with fuses, heat sinks, ESD, EME filters
4x TMC4361A closed loop motion controller with ABN/SSI/SPI encoder inputs
4x end switch inputs with input filters (1.6kHz)
1x 5kV isolated USB FS
1x onboard MPRLS0025 pressure sensor over SPI (60 mbar to 2.5 bar | 6 kPa to 250 kPa | 1 psi to 30 psi)
4x PWM outputs, max 24V, voltage selectable per jumper
2x outputs, max 24V, voltage selectable per jumper
2x UARTs, one for user with RS485, other for debug
1x I2C for user
1x SPI for user
6x GPIO, 3.3V
2x probe inputs with input filters (1.6kHz)
4x MAX31725 temperatur sensors, one per motor driver
5x outputs four one spindle (flood coolant, mist coolant (PWM), dir, step, PWM)
ESD protection on all inputs


## PressureSensor4x V1.00_Schematic Preliminary_14112019
Hardware Version 1.00

This Version don't contain Differential I2C and RS485.


## PressureSensor4x dI2C RJ45 V1.00_Schematic Preliminary_01122019
Hardware Version 1.00


## Differential I2C
Its like RS485, but for I2C signals.

Driver is PCA9615.

https://www.nxp.com/docs/en/data-sheet/PCA9615.pdf

Recommended cable is shielded twisted pair like CAT 6A or better.


## Forum:
https://groups.google.com/forum/#!topic/openpnp/rZqqyfjanco
