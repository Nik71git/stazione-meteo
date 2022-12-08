# **ESP32 WEATHER STATION**

Welcome to my DIY weather station project based on ESP32, MISOL sensors for wind measurement and rain quantitative, Kemo M152K capacitive sensor for rain detection and DHT22 for temperature and humidity; you can find a lot of similar projects on the web and this is my simple contribution to them.

The goal is to have values in Home Assistant so Esphome is the choice due to [API](https://esphome.io/components/api.html) native integrations vs MQTT (see [here](https://esphome.io/components/api.html#advantages-over-mqtt)), for other hub solutions MQTT is needed; this project works without MQTT and if you need it simple add it to the code referring to this [section](https://esphome.io/components/sensor/mqtt_subscribe.htm) and [MQTT components](https://esphome.io/components/mqtt.html) in general. Sorry in advance for my basic level english...

**LIST OF MATERIAL** 

see [Wiki](https://github.com/Nik71git/ESP32-stazione-meteo/wiki) section, wiring will follow but looking at [code](https://github.com/Nik71git/ESP32-stazione-meteo/blob/master/stazione-meteo.yaml) is quite intuitive

## **ASSEMBLY**

### _power supply (with fan exhaust):_

> ![power supply](https://user-images.githubusercontent.com/61212989/206589258-34d5ac9f-9437-4ef9-ab24-4bd76e888d98.jpg)

### _core system:_

> ![assembly](https://user-images.githubusercontent.com/61212989/206589416-a272f8d8-c62b-4f47-a8e5-4606be4ace66.jpg)

### _external hardware:_

> ![assembly](https://user-images.githubusercontent.com/61212989/205520572-8e8b52ff-2852-4d28-9d31-e012adb5b7f9.png)
