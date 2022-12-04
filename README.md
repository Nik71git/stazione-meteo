# **ESP32 WEATHER STATION**

Welcome to my DIY weather station project based on ESP32, MISOL sensors for wind measurement and rain quantitative, Kemo M152K capacitive sensor for rain detection and DHT22 for temperature and humidity; you can find a lot of similar projects on the web and this is my simple contribution to them.

The goal is to have values in Home Assistant so Esphome is the choice due to [API](https://esphome.io/components/api.html) native integrations vs MQTT (see [here](https://esphome.io/components/api.html#advantages-over-mqtt)), for other hub solutions MQTT is needed; this project works without MQTT and if you need it simple add it to the code referring to this [section](https://esphome.io/components/sensor/mqtt_subscribe.htm) and [MQTT components](https://esphome.io/components/mqtt.html) 

**LIST OF MATERIAL** 

MISOL wind direction sensor  


MISOL anemometer (wind speed)

![anemometer](https://user-images.githubusercontent.com/61212989/205516427-2d414a01-440b-47d0-b5ff-adb7da4adbe0.jpg)
