---
title : "ADS-B Resources"
feed: show
date : 02-08023
tags:
---
Some nice resources I've found in my searches. Make sure to check [[notes/electrical/RF/RTLSDR/Setting-up-a-new-RTL-SDR-Device]]

## dump1090
#dump1090 #rtlsdr #adsb #python 
	https://github.com/antirez/dump1090
	<iframe src="https://github.com/antirez/dump1090">
	</iframe>
	
![dump1090](notes/images/Running%20dump1090.bat.png)
Uses rtlsdr.dll, decodes messages into View1090.exe

When I installed and tested this, I had to reroute to port 8081 in dump1090.bat. I am not sure why, yet.


## pyModeS
Use this for decoding #adsb messages in #python 
	https://github.com/junzis/pyModeS
	`pip install pyModeS`

## Background
- [[notes/software/python/Python-Resources]]
- [[notes/electrical/RF/RTLSDR/LabVIEW-RTL-SDR-Resources]]
