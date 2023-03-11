---
title : "ADS-B Basics"
feed: show
date : 02-10-23
tags: -ADSB
---

## Description
Newly required circa 2020.  Replaces and/or supplements [Mode A/C/S Transponder](notes/aviation/components/Transponder.md).

How airplane systems communicate important data such as position, speed, altitude, and type to ground stations and other aircraft. Aircraft obtain GPS location data from satellites, then broadcast the information (1/s).


![500](notes/aviation/ADSB/images/adsb%20sportys.png)
### Data reported
-   **Register 0,5:** Airborne Altitude, Latitude and Longitude.
-   **Register 0,6:** Surface Movement, Heading, Latitude and Longitude.
-   **Register 0,8:** Aircraft Identification and Category.
-   **Register 0,9:** East-West Speed and North-South Speed or Heading and Airspeed(depending on subtype), Vertical Rate, Geometric Height Difference from Barometric Altitude.

## Where required
![500](notes/aviation/ADSB/images/ADSB%20required%20map.png)


Mandatory in most congested airspaces along with a Mode C [transponder](notes/aviation/components/Transponder.md)
. [FAA Airspace Requirements](https://www.faa.gov/air_traffic/technology/equipadsb/research/airspace#interactiveMap) 

>Any airspace that requires the use of a Transponder, described in 14 CFR 91.215, also requires aircraft to be equipped with a Version 2 ADS-B Out system. This can be either a 1090ES ADS-B system that meets the performance requirements of Technical Standard Order TSO-C166b, or a UAT ADS-B system that meets the performance requirements of TSO-C154c. Please note: The only the systems that meet the performance requirements of TSO-C166b or TSO-154c, or later versions — often referred to as 'Version 2' — comply with 91.225.

>For aircraft operating at and above FL180 (18,000 feet MSL) or to receive ADS-B services outside the United States, you must be equipped with a Mode-S transponder-based ADS-B transmitter. For aircraft operating below 18,000 feet and within the United States ADS-B rule airspace, you must be equipped with either a Mode-S transponder-based ADS-B transmitter or with UAT equipment.

## Technical details
Lots of options in order to transmit/receive ADS-B data. There are two frequencies: 1090MHz and 978MHz. In order to fly in Class A, 1090MHz is required.

Can be picked up with a cheap software defined radio. [[notes/electrical/RF/RTLSDR/RTL-SDR-Basics]] 

## Decoding ADS-B
TBD..


## LInks
https://medium.com/@mehmetcagrikose/mode-a-c-mode-s-and-ads-b-the-alphabet-soup-of-secondary-surveillance-1defcd35b2ab