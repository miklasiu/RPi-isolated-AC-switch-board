# RPi isolated AC switch board
 24/110/230V AC triac switch board

The board is intended to be used as a garden watering control be me. Use for whatever you want yourselves. 
There is Python based software being developed thar runs on this hardware.
I used optotriac-trac because it is ~3 times less expenssive than cheapest relay and it should outlast any realy.
Triac introduces ~1.4V drop but it doesn't matter much for 24V and is negligible for 110V and up.

Borard can be made at home as a 1 side. All top-side connections can be made with wires. This is the way I did it.
For the Triac you can use BTA312. I was worried they won't trigger correctly with low voltage/current but they do without a problem.
I used BTA312-600 from WeEn but any low gate current, high voltage triac will likely work.

High side 10nF capacitor needs to be rated to peak-to-peak voltage (RMS_ACV*1.41). I used 500V ones.

I didn't use I2C eeprom at all. It was intended for RPi HAT configuration, but it works without it.

You can omit indicator LEDs and their resistors too.

Generally I put too much stuff here.

Oh there are 8 inputs for whatever use you wish inteded for dry contacts. NO VOLTAGE - just switches/contacts (water level, pressure)
And I2C connector with pinout for 0.91" OLED module. I don't use it too :).

