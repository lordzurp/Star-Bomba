# Star Bomba
## la bombe des étoiles

 
### Central board to Power and Control telescope stuff

PI Hat compatible, ATmega328 Powered board


##### Power Management
The board power the Rpi directly, and has 2 DC-jack outputs to accessories

IRS-Q12 Modules from Murata provides high-efficiency conversion from wide input voltage range
* 5V 10A
* 12V 4.5A

Linear regulator AMS1117 is used to provide 3.3V for the boards components


#### RTC Unit
Based on DS3231 chip



#### Dew heater

* 5V or 12V selectable output
* 2x 2A dew heaters, MOSFET PWM driver for power dimming
* DHT22 module for ambiant T° and Rh
* DS18B20 for heater T°
* controlled by the µC, can be read and set from the Rpi


#### Rpi shutdown

can send power_off signal to Rpi thru the GPIO_4


#### OLED Display

* power ON with short press on switch, auto power-off screen after 30s
* Display misc infos :
	* Power_IN voltage, current, power and power consumption infos
	* Dew heaters status

#### Thanks to
* Dragonlost for his NAFA-BOX hardware project
* Charles LEMAIRE for his TeenAstro project