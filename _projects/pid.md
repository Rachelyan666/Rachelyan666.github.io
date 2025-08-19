---
title: "Ball Balancing PID Platform"
categories:
  - Electrical
tags:
  - Embedded
  - PID
  - CV
image: 
  path: /images/balancer.png
  thumbnail: /images/balancer_s.png
  caption: "balancer block diagram"
---

Balancing a ball on a surface is a classic control problem that involves detecting the ball’s position in real time and adjusting the platform’s orientation accordingly. 

In this project, we built a two-degree-of-freedom ball balancing system using a Raspberry Pi 4, RP2040 microcontroller, servo motors, and a custom platform made from acrylic and 3D-printed parts.

The Pi Camera captures the ball’s position in real time, and the Raspberry Pi uses a computer vision algorithm to track the ball's movement. The position data is then sent to the RP2040 through UART. The microcontroller runs a PID control algorithm that calculates the servo angles needed to tilt the platform and stabilize the ball. The ball’s position is also displayed in real time on a VGA screen as visual feedback. By isolating the x and y directions, we successfully balanced a 1-inch diameter ball on the platform.

Github: <a href="https://ece4760.github.io/Projects/Spring2025/tll68_sy625/index.html">Ball Balancer</a>

![Ball balancer](images/balancer.png)