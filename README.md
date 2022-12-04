# **ESP32 WEATHER STATION**

Welcome to my DIY weather station project based on ESP32, MISOL sensors for wind measurement and rain quantitative, Kemo M152K capacitive sensor for rain detection and DHT22 for temperature and humidity; you can find a lot of similar projects on the web and this is my simple contribution to them.

The goal is to have values in Home Assistant so Esphome is the choice due to [API](https://esphome.io/components/api.html) native integrations vs MQTT (see [here](https://esphome.io/components/api.html#advantages-over-mqtt)), for other hub solutions MQTT is needed; this project works without MQTT and if you need it simple add it to the code referring to this [section](https://esphome.io/components/sensor/mqtt_subscribe.htm) and [MQTT components](https://esphome.io/components/mqtt.html) in general. Sorry in advance for my basic level english...

**LIST OF MATERIAL** 

MISOL wind direction sensor

![wind_direction](https://user-images.githubusercontent.com/61212989/205518097-71500970-abfb-4297-8a95-0e9fd8b5e6c8.jpg)

MISOL anemometer (wind speed)

![anemometer](https://user-images.githubusercontent.com/61212989/205518109-f59e09a2-8f26-41a0-a054-587ec792ebb5.jpg)
