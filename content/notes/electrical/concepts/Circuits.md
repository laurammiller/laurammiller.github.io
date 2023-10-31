---
title: "Circuits"
feed: show
date: "2023-10-05"
tags: #RTD #transducer #excitation
---

## Measurement circuits
Measuring the output from various [[notes/electrical/sensors/Sensors|Sensors]]

### Transducer Measurement Techniques

##### Excitation In line with Measurement

![[notes/electrical/concepts/images/SimpleTransducerExcitation.png]]

##### Transmitter Connection Types

![[notes/electrical/concepts/images/234CurrentMeasure.png]]

#### 2 Wire Current Excitation
![[notes/electrical/concepts/images/2wireSensor.png]]

#### 2 Wire Measurement

![[notes/electrical/concepts/images/2wireSimple.png]]
#### References
- https://www.analog.com/en/analog-dialogue/articles/transducer-sensor-excitation-and-measurement-techniques.html)
- https://www.ti.com/lit/an/sbaa275a/sbaa275a.pdf?ts=1696412198716
### 4 Wire RTD

The true 4-wire measurement uses the current-potential method. A current of known value (I+) is passed through the sensor along the “current” lead wires. The voltage generated across the sensor is measured using the “potential” lead wires (Vsensor) and the sensor’s resistance is calculated by dividing the measured voltage by the Known current. 
![[notes/electrical/concepts/images/4wireRTD.png]]
![[notes/electrical/concepts/images/4leadMeasure.png]]
![[notes/electrical/concepts/images/4wireKelvin.png]]
In the preceding illustration, two separate pairs of probes are used. Pair 1 and 2 (sometimes referred to as the “source” probes) provides a known quantity of constant current, as in the two-wire setup. In addition, the Kelvin technique employs
a second pair of probes (labeled 3 and 4 above) to sense voltage. This second pair is often called the “sense” probes. The placement of these probes ensures that only the voltage across the load is measured, independent of any resistance contributed by the current (source) probes. Virtually no current passes through the sense probes; the current instead passes through the source probes. This allows for a high level of measurement sensitivity and accuracy when the load under test is of low resistance. The ability to accurately measure low resistances can be critical in applications that involve high current, since even a small change in resistance (for example, due to fluctuating temperature) can have a significant effect on
voltage levels.
#### References
- https://www.aemc.com/userfiles/files/resources/applications/micro-ohmmeter/APP-4WireKelvin.pdf 

## Shunt Calibration

A method for determining the full-scale output of a pressure transducer by electrically simulating a full load. For piezoresistive strain gauge-type pressure transducers.
![[notes/electrical/concepts/images/shuntCalibration.png]]

#### References
- https://www.apgsensors.com/about-us/blog/what-is-shunt-cal-and-how-does-it-work/
- https://studylib.net/doc/5720732/shunt-cal

## Wheatstone Bridge
- A circuit used to measure an unknown resistance by balancing two legs of a bridge circuit
- Can be used to eliminate temperature bias when measuring pressure (voltage) strain gauges such as a [[notes/electrical/sensors/Pressure Transducer|Pressure Transducer]].
- ![[notes/electrical/concepts/images/WheatstoneBridge.png]]
#### References
- https://www.grc.nasa.gov/WWW/k-12/airplane/tunwheat.html
