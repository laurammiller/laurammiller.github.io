---
title: "Transponder"
feed: show
date: "2023-03-11"
tags: #aircraftsystems
---
## Background
Short for "transmitter responder"
Identification of Friend or Foe (IFF)
A basic command/reply response system for identification and classification of aircraft in a controlled airspace

## Piper Archer Installation
Garmin GTX 345 Series installed in [Archer](notes/aviation/club/Archer%20Specs.md)

![300](notes/aviation/components/images/Archer%20Transponder%20OFF.png)


![300](notes/aviation/components/images/Garmin%20GTX345%20Screenshot.png)
### Capabilities
- ADS-B In/Out at 1090MHz
- Mode S extended squitter (ES)
- can stream weather, traffic, etc to connected display or device using "Connext"
## Mode A

A subset of Mode 3 of IFF. Transmits identification only using 4 digits. When asked to "squawk" a code it is transmitted using this mode

### Important squawk codes

-   **1200:** Generally used by aircraft under Visual Flight Rules(VFR)
-   **7700:** Used during emergency
-   **7600**: Used when radio communication fails
-   **7500**: Used during hijacking(unlawful interference) of the aircraft

## Mode C

Contains pressure altitude information in 100ft increments. Both Mode A and Mode C can be activated/deactivated by the pilot using the transponder.

Towers use SSR (Secondary Surveillance Radar) to interrogate aircraft in a moving beam. In this way responses can be plotted on a map.

### Disadvantages
No error checking
Multiple aircraft can reply at the same time

## Mode S

Using the same frequency and transmission properties as Mode C (backwards compatible) but with better error handling and more bandwidth (24bit addresses) and more stored data to query.

Aircraft can be selectively queried based on their mode in an airspace (Mode A/C and Mode S)

![](notes/aviation/components/images/Mode%20S%20Interrogation.png)

### Technical Details
Mode S uses 255 registers, each with 56 bits of data (check this)

#### Reported Data

-   **ELS:** The system must provide automatic aircraft identity reporting, transponder capability report, flight status(airborne/on ground), altitude report.
-   **EHS:** The system provides ELS capability, plus Selected Altitude in Register (4,0), Roll Angle, Track Angle Rate, True Track Angle, Ground Speed in Register (5,0), Magnetic Heading, Indicated Airspeed/Mach No, Vertical Rate in Register (6,0).

![600](notes/aviation/components/images/Mode%20S%20Data.png)

## Next Gen
[ADS-B](notes/aviation/ADSB/ADS-B.md)

## Links
https://medium.com/@mehmetcagrikose/mode-a-c-mode-s-and-ads-b-the-alphabet-soup-of-secondary-surveillance-1defcd35b2ab

