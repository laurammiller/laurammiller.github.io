---
title : "WeatherStation"
feed: show
date : 02-16-23
---

The train derailment in East Palestine, OH and subsequent lack of communication to local residents had me researching whether there are reliable environmental monitors out there that everyday citizens can use and share for themselves. Luckily, there are some projects out there but not worldwide and not covering every sensor type. 

The sensors I would want are:

- Air particulates (PM 2.5)
- Temperature
- Humidity
- Barometric pressure
- Water quality
- Radiation
( See [Sensors](notes/electrical/sensors/Sensors.md))

*Interesting side note - A little local weather station would be helpful to determine and predict good [flying](notes/aviation/Aviation-Topics) days..*

# Air Quality
- [PurpleAir](https://map.purpleair.com/1/mAQI/a10/p604800/cC0#4.8/42.38/22.15)
- Safecast (Japan)
- [Sensor.Community](https://maps.sensor.community/#7/40.221/-83.662)
	- https://sensor.community/en/sensors/airrohr/
	- https://devices.sensor.community/
- [RibbitNetwork](https://www.ribbitnetwork.org/)

# Radiation
- Safecast
	- An obsolete "pancake geiger" design is found here: https://github.com/Safecast/bGeigieNanoKit/wiki/Parts-List

# DIY Systems
A pretty simple system could be constructed using a microcontroller and an array of sensors. Estimated cost ~ $100 (or much cheaper if skipping the geiger counter test)
## Kits
- [air quality kit](https://howtomechatronics.com/projects/diy-air-quality-monitor-pm2-5-co2-voc-ozone-temp-hum-arduino-meter/)
## Parts
- Particulate Sensors
	- PM2.5 PMS5003
	- SDS011
- Water Particlulate Sensors
	- TDS Probe Sensor
	- Conductivity Sensor (variable, must establish baseline)
- Geiger counter
	- [mightyohm kit](https://mightyohm.com/blog/2012/02/feed-your-geiger-readily-available-radioactive-test-sources/)
	- [Hackaday Photodiode version](https://hackaday.com/2019/02/22/radiation-detector-eschews-tubes-uses-photodiode/)
- RF Meter
	- [Software Defined Radio](notes/electrical/RF/RTLSDR/RTL-SDR.md)
- [Thermocouple](notes/electrical/sensors/Thermocouple.md)
- Humidity
-  [barometric](notes/electrical/sensors/barometric.md) Pressure
- GPS
