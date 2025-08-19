---
title: "Wetland Flux Chamber"
image: 
  path: /images/flux.png
  thumbnail: /images/flux_s.png
  caption: "Flux chamber block diagram"
---

Accurate, long-duration field measurements of methane (CH₄) and carbon dioxide (CO₂) flux are essential for environmental monitoring and climate policy. 

In this project, we developed a low-power embedded data logger for use in portable flux chambers, enabling autonomous environmental sensing over multi-day deployments. The system is built around a Raspberry Pi Pico and integrates both a digital SCD30 sensor (for CO₂, temperature, and humidity) and an analog methane sensor via ADC. Sensor data is timestamped using the onboard RTC and logged to a microSD card in CSV format using the FatFs library. To conserve power, the Pico enters a sleep state between logging cycles and wakes on hardware timer alarms. All firmware was written in C using protothreads and tested across 10 field-ready chamber prototypes for deployment in wetlands, agricultural fields, and manure management sites.

To support long-term stability and field reliability, we designed a custom PCB that consolidates the entire electronics system—power management, sensors, storage, and interface connections—into a compact, robust layout. We implemented watchdog timers and error recovery routines to ensure the logger could autonomously recover from temporary faults such as I2C hangs or sensor communication errors. These improvements significantly enhanced system uptime, allowing multi-day logging without interruption. The final system reflects a complete embedded solution, combining environmental sensing, ultra-low power operation, resilient firmware, and hardware integration suitable for real-world environmental research.

Github: <a href="https://cornellfluxchamber.github.io/">Cornell Flux Chamber</a>

![Wetland Flux Chamber](/images/flux.png)