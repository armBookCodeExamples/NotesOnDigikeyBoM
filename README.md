## Buy the whole Bill of Materials (BoM) with one click

You are able to buy all the materials used in the book easily here:
- https://www.digikey.com/en/resources/edu/arm-education-media/embedded-designs-textbook

Most of the parts on that BoM are exactly the same as in the book. However, a few of the parts on DigiKey BoM are not exactly the same as the parts included in the "Bill of Materials" section of the book, but very similar replacements that can be safely used if the following considerations are taken into account:

---

#### [377-2647-ND MB102 breadboard power supply](https://www.digikey.com/en/products/detail/bud-industries/BBP-32701/8602382)

The differences are:
1. The USB connector is A instead of micro B.
2. The selection of 5 V and 3.3 V is with a jumper instead of a switch.
3. There is a selector to choose whether to power it with USB cable or a jack.

---

#### [1597-1182-ND HC-SR501 PIR Sensor Module](https://www.digikey.com/en/products/detail/seeed-technology-co-ltd/101020060/5487425)

Considerations will be soon published here.

---

#### [1597-1647-ND Relay Module](https://www.digikey.com/en/products/detail/seeed-technology-co-ltd/103020132/9369927)

Here it is all the information on the [1597-1647-ND Relay Module](https://wiki.seeedstudio.com/Grove-2-Channel_SPDT_Relay/).  
This module has the following schematic:

<img src="https://github.com/armBookCodeExamples/NotesOnDigikeyBoM/blob/main/1597-1647-ND-Relay-Module.png" width="600">

It has not optocouplers, as the relay module that is used in the book:

<img src="https://github.com/armBookCodeExamples/NotesOnDigikeyBoM/blob/main/Figure7-12.png" width="600">

This could cause noise problems mainly with the solenoid valve.  
At the connection level it is the same as the relay module used in the book.

---

#### [1286-1200-ND SD Card Module](https://www.digikey.com/en/products/detail/digilent-inc/410-380/9445906)

The pinout of the 1286-1200-ND SD Card Module can be seen here: [link](https://mm.digikey.com/Volume0/opasdata/d220001/medias/docus/749/Pmod_MircoSD_RM_Web.pdf)

The correspondence with the module used in the book:

<img src="https://github.com/armBookCodeExamples/NotesOnDigikeyBoM/blob/main/Figure9-3.png" width="600">

Is as follows:

1 -> 12 VCC Power Supply (3.3V)  
2 -> 1 ~CS Chip Select / Data3  
3 -> 2 MOSI MOSI / Command 8  
4 -> 4 SCK Serial Clock  
5 -> 3 MISO MISO / Data0  
6 -> 5 GND Power Supply Ground  

---

#### [1568-1670-ND Moisture sensor](https://www.digikey.com/en/products/detail/sparkfun-electronics/SEN-13637/7400839)

In the book the connections are as decribed here [link](https://arduinopoint.com/soil-moisture-sensor-arduino-project/) while in the 1568-1670-ND Moisture sensor the connections are this way: [link](https://www.geeksforgeeks.org/soil-moisture-measurement-using-arduino-and-soil-moisture-sensor/).
The difference is that the the 1568-1670-ND Moisture sensor directly delivers the analog signal out of the sensor module.
Therefore, the connection would be the same as with the intermediate module we have but directly to the sensor.

---

