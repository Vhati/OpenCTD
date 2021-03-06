OpenCTD
=======

[Link](https://www.rockethub.com/projects/26388-oceanography-for-everyone-the-openctd): RocketHub Project Description

### Background

Conductivity, temperature, and depth (CTD). With these three measurements, marine scientists can unlock ocean patterns hidden beneath the waves. The ocean is not uniform, it its filled with swirling eddies, temperature boundaries, layers of high and low salinity, changing densities, and many other physical characteristics. To reveal these patterns, oceanographers use a tool called the CTD. A CTD is found on almost every major research vessel. Rare is the scientific expedition--whether it be coastal work in shallow estuaries or journeys to the deepest ocean trenches--that doesn’t begin with the humble CTD cast.

### Overview

The OpenCTD is a low-cost, open-source CTD suitable for both educators and scientists. The platform is built using readily available parts and is powered by an Arduino-based microcontroller. Our goal is to create a device that is accurate enough to be used for scientific research and can be constructed for less than $200. Source codes, circuit diagrams, and building plans will be freely available. The final instrument will be effective to 200 meters depth.   Why 200 meters? For many coastal regions, 200 meters of water depth covers the majority of the ocean that is accessible by small boat. The OpenCTD is targeted to people working in this niche, where entire research projects can be conducted for less than the cost of a commercial CTD. However, the Open CTD is scalable, and anyone with the inclination can adapt our plans to operate in deeper waters.

### Hardware

* An Arduino microcontroller
* MS5803-14BA pressure sensor
* Dallas DS18B20 3-gang temperature probe
* Atlas conductivity circuit with homebrewed probe

### Required Arduino Libraries

I2C library for the MS5803_14BA pressure sensor<br />
https://github.com/millerlp/MS5803_14

Dallas Temperature Control for the DS18B20 thermometer<br />
https://milesburton.com/Dallas_Temperature_Control_Library

OneWire **<br />
http://www.pjrc.com/teensy/td_libs_OneWire.html<br />
http://playground.arduino.cc/Learning/OneWire

SD *<br />
https://www.arduino.cc/en/Reference/SD

SoftwareSerial *<br />
http://www.pjrc.com/teensy/td_libs_SoftwareSerial.html<br />
https://www.arduino.cc/en/Reference/SoftwareSerial

SPI **<br />
https://www.pjrc.com/teensy/td_libs_SPI.html<br />
https://www.arduino.cc/en/Reference/SPI

Wire *<br />
http://www.pjrc.com/teensy/td_libs_Wire.html<br />
https://www.arduino.cc/en/Reference/Wire

\* Included with Arduino.<br />
\** Included with Arduino. A newer version may be available.

### Pinouts

A4 - Pressure Sensor SDA

A5 - Pressure Sensor SCLK

D7 - Temperature Data

D2 - Conductivity RX

D3 - Conductivity TX

### Acknowledgments

This software has been kludged together by Andrew Thaler, based on code from Walt Holm, arduino.cc samples, Atlas scientific, Vhati, and Russell Neches.
