---
title: "Kitchen Alarm System"
image: 
  path: /images/kitchen.png
  thumbnail: /images/kitchen_s.png
  caption: "kitchen alarm photo"
---

This project implements a real-time gas monitoring and alert system using FreeRTOS ported to the STM32F103C8T6 microcontroller. We manually integrated FreeRTOS from source and configured it to run on the STM32 platform, enabling structured multitasking for multiple sensors and peripherals. The system reads from analog gas sensors—MQ2 and MQ9B—to detect smoke, carbon monoxide (CO), and methane (CH₄), along with an additional ADC-based temperature sensor. Each sensor is managed by its own FreeRTOS task, allowing efficient and predictable scheduling of sampling, threshold checks, and actuator responses. A buzzer provides immediate local alerts for hazardous gas levels, and a OLED display (connected via I2C) displays real-time sensor data.

All sensors communicate through STM32's ADC subsystem, and critical alerts are sent remotely via MQTT using an ESP8266 Wi-Fi module. When gas or temperature levels exceed safe limits, the system publishes warning messages to a phone-based IoT application, allowing for timely remote intervention. FreeRTOS ensures deterministic behavior even under load, handling ADC reads, alarm triggering, display updates, and MQTT communication concurrently. This project demonstrates a robust embedded system that combines RTOS task management, analog sensing, I2C interfacing, and cloud connectivity for real-time environmental safety and monitoring.

Github: <a href="https://github.com/Rachelyan666/kitchen_alarm">Kitchen Alarm System</a>

![Smart Dorm IOT](/images/kitchen.png)
