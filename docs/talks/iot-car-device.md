# IoT Car Device

### Base Design

Three core components:

* API
* UI
* Data Collector (IoT Device)

API core functionality:

* Receive and store data with a generated timestamp
* Retrieve data by device ID

Hosted on Heroku.

Language: Java
Framework: Spring Boot

UI:

* Framework: React
* Map Library: OpenLayers
* Hosting: Heroku

IoT Device:

* Microcontroller / Single Board Computer: Raspberry Pi
* Sim module: SIM7000
* Carrier: Hologram.io

Gathering Data

* Post data per location point
    * Post data per location point vs post data every 2-3 hours

Challenges:

* Power consumption
    * Not enough power to the SIM7000 makes it unresponsive. PC/Laptop USB power doesn't work.
* Initial response delay
    * Lengthy boot routing for a SIM7000. 15 mins to 3 hours.
* Slow initial connection to network

Futher reading: https://dev.io/alwaysup/make-an-iot-device-for-tracking-vehiciles-1706