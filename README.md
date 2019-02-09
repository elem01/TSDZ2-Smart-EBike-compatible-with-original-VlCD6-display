# TSDZ2-Smart-EBike-compatible-with-original-VLCD6-display
This project is based on the TSDZ2-Smart-EBike repository, but is also compatible with the original VLCD6 display (it should also work with VLCD5 and HX18).
- The walk assist function has been implemented and it works with 5 level of assistance.
- Implemented Java user interface (TDSZ2 Configurator), useful to configure many parameters of program memory and data memory (eeprom) of   the controller.
- The TDSZ2 Configurator run with JRE runtime.... so it must be installed!
- The SDCC compiler must be installed!
- Using TDSZ2 Configurator you can enable the use of both type of display KT-LCD3 and VLCD6 (compatible also VLCD5 and XH18).
- The light-gray fields of the TSDZ2 Configurator are reserved for "expert users".
- Using TDSZ2 Configurator you can save configuration files (.ini) and move them from experimental settings folder to proven settings.
- by clicking the "help" button, a pdf document will open. It contains information regarding the user interface parameters and addresses     related to eeprom memory.
In the firmware M0.16.D of the motor and in the software 0.2.0 of the java configurator some improvements have been implemented:
- The Lights, Street and Power Boost functions can be activated by the lights button (button down for VLCD6) without one function
  excluding the other.
- The Walk Assist Off Delay mode manages a programmable delay for stopped motor, so you can release the Walk Assist button and in case of   need just press the UP button, or the DOWN button, or use the brakes (if enabled).
Walk Assist Off Delay mode works only when Assist Level 1 is set.
- 1 To enable the STREET function (Normal Mode), select Assist Level 1, press and hold the lights key for 2 seconds until the backlight is     lit and E03 is displayed. Press the light button again for another 2 seconds until the backlighting and the E03 code goes off.
    NOTE!! When the E03 code is displayed and the lights button is not pressed again within 5 seconds, the lights will turn on and the         STREET function will be aborted.
- 2 To re-enable the OFFROAD function (Default), refer to point 1, but in this case the displayed code will be E04.
- 3 To enable (E05) or disable (E01) the POWER BOOST function, select Assist Level 2, then refer to point 1.
- 4 To restore the default functions (E02) (OFFROAD enabled, POWER BOST disabled), select Assit Level 0, then refer to step 1 again.
I want to remember that to turn on the lights (if enabled) in the Assit levels 0, 1, 2, you have to press the lights key for 2 seconds, release it and the lights will turn on after 5 seconds ... ignore the codes that will appear on the display, the functions will be aborted automatically. In Assit Levels 3 and 4, the lights will light on immediately after pressing the button for 2 seconds.
This is a Beta release, not all features have been verified, so I leave the user the opportunity to do any tests, this will allow me to receive your impressions.

