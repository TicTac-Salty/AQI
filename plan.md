# Overview

I will create an air quality monitor that reports local air quality index, displays the value via LCD screen, and sends values wirelessly to a remote location. 

# Research

## What is the problem?

[Air quality](https://www.wikiwand.com/en/Air_quality_index) in Kathmandu.

## Why is it a problem?

Health:
- Life (animals; includes people!)
- Planet (environment)

## What can I do?

Awareness: Start by monitoring.

## What makes a good design?

- Useful
- Simple (and easy to use)
- Cost effective
- Attractive

Find some examples.

## Resources

### Ideas

- [Air quality monitoring IOT – Arduino & sensors connected to a Raspberry Pi](http://www.open-bigdata.com/arduino-raspberry-air-quality-iot/): *see "Further references / alternatives" at end*
- [Ambient air analyzer.](http://lelabtechno.com/analyseur%20air.html)
- [MEASURE AIR QUALITY YOURSELF](https://luftdaten.info/en/home-en/)
- [How To Measure Particulate Matter With a Raspberry Pi](https://hackernoon.com/how-to-measure-particulate-matter-with-a-raspberry-pi-75faa470ec35)
- [How To Measure Particulate Matter With a Raspberry Pi (Update)](https://openschoolsolutions.org/measure-particulate-matter-with-a-raspberry-pi/)
- [Air quality sensor project](https://www.raspberrypi.org/forums/viewtopic.php?t=209633)

### Learn

- [Getting started with Arduino](https://www.arduino.cc/en/Main/Tutorials)

# Design Objectives

- Measure at least [PM2.5](https://www.wikiwand.com/en/Particulates)
- AQI. *What is AQI? How is it defined? Why is it defined how it is? How to translate sensor data into AQI?*
- Display on LCD at node (both in units of concentration and AQI)
- Should be cost-effective and relatively easy to program.
- Data is uploaded to cloud
- Portable power?
- Allow for easy fixes (consider availability of parts)

# Materials

- Candidate microcontroller kits:
  + [ ] ESP8266
  + [x] Arduino
  + [ ] Raspberry Pi
 - [Testing the Shinyei PPD42NS](http://irq5.io/2013/07/24/testing-the-shinyei-ppd42ns/)
 - [Nova PM sensor SDS011 high precision laser PM2.5 air quality detection sensor module](https://www.aliexpress.com/item/Nova-PM-sensor-SDS011-High-precision-laser-pm2-5-air-quality-detection-sensor-module-Super-dust/32894938003.html?spm=2114.search0104.3.1.1965657fEvSKDg&ws_ab_test=searchweb0_0,searchweb201602_5_10065_10068_10130_10890_10547_319_10546_317_10548_10545_10696_453_10084_454_10083_433_10618_431_10307_537_536_10059_10884_10887_100031_321_322_10103-10890,searchweb201603_45,ppcSwitch_0&algo_expid=629daefa-c2bf-4902-843d-b12fa7ff3ad0-0&algo_pvid=629daefa-c2bf-4902-843d-b12fa7ff3ad0&transAbTest=ae803_3)

# Testing Plan

- Benchmark to handheld monitor
  + Inside
  + Outside
- Sensor data calibration *How to do it? Why to do it? What is truth?*
- Interpreting measurements *How to get usable data (e.g., filtering, processing, etc.)? What to average over what time period to compare to what limits?*

# Programming

I will use the C programming language to program the Arduino.

# Timeline

- October
  + [ ] Get started with Arduino (complete a couple of starter projects) **4 hours**
  + [ ] Research and obtain necessary hardware (e.g., sensors, LCD, fan, enclosure) **4 hours**
- November
  + [ ] Build prototype that can at least plot the signal over time (save to file) **4 hours**
  + [ ] Add LCD screen that displays signal **4 hours**
  + [ ] Convert signal to AQI and display on LCD **4 hours**
- December
  + [ ] Calibrate and test AQI **4 hours**
  + [ ] Connect hardware to internet **4 hours**
  + [ ] Plot file online using data plotter **4 hours**
