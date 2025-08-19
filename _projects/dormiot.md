---
title: "Smart Dorm IOT System"
image: 
  path: /images/dormiot.png
  thumbnail: /images/dormiot_s.png
  caption: "dorm IOT photo"
---

This project is a Wi-Fi-connected smart dorm automation system built using a combination of ESP32 and Raspberry Pi Pico W microcontrollers. 

It integrates multiple subsystems: a AHT20 temperature/humidity sensor-controlled fan (ESP32), a distance-based light control system (Pico W), a PIR montion sensor-controlled signal system of outdoor status and a magnetic door sensor (Pico W) that detects whether the bathroom door is open or closed, indicating occupancy. All sensor data is transmitted over MQTT via Wi-Fi to a centralized broker, allowing for remote monitoring and control. Devices subscribe to control topics and publish real-time status updates, enabling seamless interaction through a custom web-based dashboard with button controls and state indicators.

Sensors are interfaced using the I2C protocol, and PWM is used to drive fan and light switches for precise control. In addition to sensor-actuator loops, the system includes a room status display: a display outside the room signals occupancy or availability based on motion detection and manual override. Together, these components form a cohesive embedded system that demonstrates wireless communication, MQTT messaging, I2C and PWM peripherals, and real-time web integration—designed specifically for convenience, automation, and energy awareness in a college dorm setting.

Github: <a href="https://github.com/Rachelyan666/smart_dorm_iot">Smart Dorm IOT System</a>

![Smart Dorm IOT](/images/dormiot.png)