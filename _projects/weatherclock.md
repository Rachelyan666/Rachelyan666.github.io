---
title: "Weather Clock Project"
date: 2025-08-12
categories:
  - Electrical
tags:
  - Embedded
  - Networks
image: 
  path: /images/weather_clock.png
  thumbnail: /images/weather_clock_s.png
  caption: "weather clock photo"
---

This project is a Wi-Fi-connected weather and temperature display system built using an STM32F103 microcontroller, a ESP32-C2 wifi board, and an ST7735 LCD. 

The ESP32-C2 connects to the internet, retrieves live weather and time data from OpenWeatherMap, and sends a compact summary—location, weather condition, temperature, and timestamp—via UART communication with the AT commands to the STM32. The STM32 parses the data and renders it on the LCD with accompanying weather icons and digital clock output.

The system also features an onboard NTC thermistor for ambient temperature sensing via ADC, and an MPU6050 accelerometer connected over I2C to detect device orientation. Based on tilt, the screen automatically rotates its contents for better viewing. This project integrates wireless communication, USART communication, I2C sensor interfacing, ADC measurement, DMA for accelerated data transfer and SPI-based graphical output in a compact, responsive embedded system.


Github: <a href="https://github.com/Rachelyan666/weather_clock">Weather Clock</a>

![Weather Clock](/images/weather_clock.png)

