---
title: "Embedded Mahjong Player"
date: 2024-05-15
categories:
  - Electrical
tags:
  - Embedded
  - Linux
  - ML
  - CV
image: 
  path: /images/mahjong.jpeg
  thumbnail: /images/mahjong_s.jpeg
  caption: "embedded mahjong player photo"
---

Smart AI Mahjong Player on Embedded Operating Systems using CV and robot arm.

Mahjong is a type of Chinese board game where four players are required for a game. Often times, people find it hard to always find four people for the game, often there are only three. Therefore, it became a problem that a fourth player is needed. To solve this problem, our team worked on the embedded mahjong player, so that it can play along as the extra player to help start the game.

Our project first uses the Pi Camera to take photos of Mahjong tiles, and uses the photos to train the computer vision model, and then uses the trained model to identify the tiles. Next, the Mahjong algorithm would determine which tile it should play this round, and send the instruction to the PiTFT and servo to indicate the played tile. Displays and buttons on the PiTFT are also used as round controls. 

Github: <a href="https://github.com/colonel-aureliano/Embedded-Mahjong-Bot">Embedded Mahjong Bot</a>

![Mahjong](/images/mahjong.jpeg)

