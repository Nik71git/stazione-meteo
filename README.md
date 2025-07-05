# **ESP32 WEATHER STATION**

Welcome to my DIY weather station project based on ESP32, MISOL sensors for wind measurement and rain quantitative, Kemo M152K capacitive sensor for rain detection and DHT22 for temperature and humidity; you can find a lot of similar projects on the web and this is my simple contribution to them.

The goal is to have values in Home Assistant so Esphome is the choice due to [API](https://esphome.io/components/api.html) native integrations vs MQTT (see [here](https://esphome.io/components/api.html#advantages-over-mqtt)), for other hub solutions MQTT is needed; this project works without MQTT and if you need it simple add it to the code referring to this [section](https://esphome.io/components/sensor/mqtt_subscribe.htm) and [MQTT components](https://esphome.io/components/mqtt.html) in general. Sorry in advance for my basic level english...

**LIST OF MATERIAL** 

see [Wiki](https://github.com/Nik71git/ESP32-stazione-meteo/wiki) section, wiring is [here](https://user-images.githubusercontent.com/61212989/206810130-b3e16a60-336d-45f4-94cc-58652903698e.jpg) but looking at [code](https://github.com/Nik71git/ESP32-stazione-meteo/blob/master/stazione-meteo.yaml) is quite intuitive.

**SENSOR CALIBRATIONS**

take a look [here](https://github.com/Nik71git/ESP32-weather-station/wiki/hardware-data-sheet) for sensor calibrations, especially the first two PDF.
In my station wind speed has a multiply of 0,04 since it close once per second (that means a complete rotation) at a speed of 2,4 km/h due to datasheet.
Code contains explicative comments but verify your windspeed sensor datasheet for correct calibration.
Same for wind direction and rain gauge, wind direction is the most complex to calibrate since you have to know exactly where is the North that means the starting point for rotations, obviously you need a compass to be more precise as possible, and when you point at north you need 0° which correspond to resistance value from 3100 Ohm to 3200 Ohm (exact value is 3132 Ohm); for this reason probably you need to read **adc_sensor** and **resistance_sensor** so set them to _internal: false_ before toggle them to true. 

## **ASSEMBLY**

* _the complete assembly guide is [here](https://github.com/Nik71git/ESP32-weather-station/files/10198231/sensor.assembly.guide.pdf)_

### _power supply (with fan exhaust):_

power is provided by 12Vdc LVPS (the white one) for rain sensor and ESP32 power converter (the black one) which provide 5Vdc via usb port  

> ![power supply](https://user-images.githubusercontent.com/61212989/206589258-34d5ac9f-9437-4ef9-ab24-4bd76e888d98.jpg)

### _core system:_

> ![assembly](https://user-images.githubusercontent.com/61212989/206589416-a272f8d8-c62b-4f47-a8e5-4606be4ace66.jpg)

### _external hardware:_

> ![stazione-meteorologica_new](https://github.com/user-attachments/assets/6ac7ac4a-36cf-4c16-9ef7-d04747412f80)

### _Home Assistant card:_

![ha card](https://github.com/user-attachments/assets/433e2e16-3b7a-45bc-9064-c9b92c9484a9)

