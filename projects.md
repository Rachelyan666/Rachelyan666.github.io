---
layout: home
show_excerpts: false
header: false
title: Projects
---

## Electrical projects

**Ball Balancing PID Platform**

Balancing a ball on a surface is a classic control problem that involves detecting the ball’s position in real time and adjusting the platform’s orientation accordingly. In this project, we built a two-degree-of-freedom ball balancing system using a Raspberry Pi 4, RP2040 microcontroller, servo motors, and a custom platform made from acrylic and 3D-printed parts.

The Pi Camera captures the ball’s position in real time, and the Raspberry Pi uses a computer vision algorithm to track the ball's movement. The position data is then sent to the RP2040 through UART. The microcontroller runs a PID control algorithm that calculates the servo angles needed to tilt the platform and stabilize the ball. The ball’s position is also displayed in real time on a VGA screen as visual feedback. By isolating the x and y directions, we successfully balanced a 1-inch diameter ball on the platform.

Github: <a href="https://ece4760.github.io/Projects/Spring2025/tll68_sy625/index.html">Ball Balancer</a>

![Ball balancer](images/balancer.png)


**Tide Clock**

In general, our system works by sending tidal data from the FRDM-KL46Z board using skills we learned this semester, and then use the arduino to receive and process the data, which finally controlls the LED strip to turn on and off showcasing the tide.

In this project, we accomplished and practices a lot of skills that we learn in this class. For example, in hardware, we practiced wire soldering a lot in the project. Then, in the FRDM-KL46Z code, we accomplished sending data using UART serial communication, as well as the real-time scheduling that we learned by the end of the semester. Finally, in Arduino code, we accomplished receiving data in UART, as well as data decode and other programming skills.

Github: <a href="https://pages.github.coecis.cornell.edu/ece3140-sp2023/jnl77-sy625-xf37/">Tide Clock</a>

![Tideclock](/images/tideclock2.png)


**Embedded Mahjong Player**

Mahjong is a type of Chinese board game where four players are required for a game. Often times, people find it hard to always find four people for the game, often there are only three. Therefore, it became a problem that a fourth player is needed. To solve this problem, our team worked on the embedded mahjong player, so that it can play along as the extra player to help start the game.

Our project first uses the Pi Camera to take photos of Mahjong tiles, and uses the photos to train the computer vision model, and then uses the trained model to identify the tiles. Next, the Mahjong algorithm would determine which tile it should play this round, and send the instruction to the PiTFT and servo to indicate the played tile. Displays and buttons on the PiTFT are also used as round controls. 

Github: <a href="https://github.com/colonel-aureliano/Embedded-Mahjong-Bot">Embedded Mahjong Bot</a>

![Mahjong](/images/mahjong.jpeg)


**Theater Actor Auto Follow Light System** [**In Progress**]

In theater productions, a follow spot is often used to highlight the lead actor on stage. Traditionally, this spotlight is manually controlled, which can be labor-intensive and may not always keep up with fast-moving performances. To solve this problem, our team is developing an automated actor tracking spotlight system that can follow the actor in real-time without human control.

Our project uses a Raspberry Pi and infrared tracking techniques to detect the actor's position on stage. The actor is equipped with an infrared-emitting marker, and sensors or Pi-compatible NoIR cameras are used to detect the IR signal. The position data is then processed to calculate the actor’s location and send commands to a motorized spotlight to pan and tilt accordingly. This system aims to improve spotlight accuracy and reduce manual operation in live theater environments.

![Auto Following Light](/images/follow.png)


**Wetland Flux Chamber** [**In Progress**]
Accurate, long-duration field measurements of methane (CH₄) and carbon dioxide (CO₂) flux are essential for environmental monitoring and climate policy. In this project, we developed a low-power embedded data logger for use in portable flux chambers, enabling autonomous environmental sensing over multi-day deployments.

The system is built around a Raspberry Pi Pico and integrates both a digital SCD30 sensor (for CO₂, temperature, and humidity) and an analog methane sensor via ADC. Sensor data is timestamped using the onboard RTC and logged to a microSD card in CSV format using the FatFs library. To reduce power consumption, the Pico enters a sleep state between logging cycles and wakes on hardware timer alarms. The entire firmware was written in C using protothreads and deployed across 10 field-ready chamber prototypes designed for use in wetlands, agricultural fields, and manure sites.

<br>

## Software Projects

**LTL interpreter**

This project is a interpreter written by Ocaml that transfers a natural language that follows LTL rules into an automata graph.

This is a tool that can translate everyday language into something a machine understands. LTL logic, which is the Linear Temporal Language (LTL) will be transformed into Büchi Automata.

This converter takes in strictly-formatted human language, parses and synthesizes it into a simplified Linear Temporal Logic expression, and converts it into a reliable Büchi automaton that is visualized and verifiable. With the automaton being generated, the user is able to verify if their subsequent tentative actions is executable.

Github: <a href="https://github.com/JLjw8/LTL2Buchi">Interpreter</a>

![interpreter](/images/buchi.png)

**Ultimate Tic-Tac-Toe AI Player**

This project implements an AI agent built to play Ultimate Tic-Tac-Toe, implemented in Python with a AI algorithms and Pygame-based graphical interface.

The project explores classic game AI techniques including Minimax search, Alpha-Beta pruning, and heuristic evaluation functions tailored for the unique rules of Ultimate Tic-Tac-Toe. The AI is capable of playing strategically on both the macro and micro boards, adapting to changing board states and forcing favorable positions. The rules of valid move restrictions and win propagation are fully enforced.

Users can play against the AI in an interactive GUI and toggle between different levels of difficulty. The project also includes testing infrastructure and tools for analyzing AI performance over multiple games.

Github: <a href="https://github.com/Rachelyan666/alien_shooting">AI Ultimate tic-tac-toe player</a>

![AI tic-tac-toe player](/images/uttt.png)
