---
title: "Filippo"
date: 2020-09-12
categories: ["AI Projects"]
tags:
- ADAS
- Jetson Nano
description: "Recently, I have built a prototype of an advanced driver-assistance system (ADAS) using a Jetson Nano computer. In this post, I will introduce my ADAS project on Jetson Nano and the software design of this system."
thumbnail: /posts/adas-jetson-nano-software/camera-calib.png
slug: "/posts/adas-jetson-nano-software/"

discussionId: "/posts/adas-jetson-nano-software/"
math: true
featured: true
toc: true
---

Recently, I have built a prototype of an advanced driver-assistance system (ADAS) using a [Jetson Nano computer](/posts/2020-04-02-thiet-lap-ban-dau-cho-jetson-nano/). In this project, I have successfully deployed **3 deep neural networks**  and some **computer vision algorithms** on a [super cheap hardware of Jetson Nano](https://www.nvidia.com/en-us/autonomous-machines/jetson-store/). I decided to write this post series to share about how this system was designed and implemented. [The first post](/posts/adas-jetson-nano-intro-and-hardware/) is an introduction and the hardware design of my system. Today post will talk about the software design.

The software system provides three main functions: **(i) forward collision warning with forward vehicles and pedestrians, (ii) lane analysis and lane departure warning, (iii) sign detection for maximum speed limit signs and over-speed warning**. These functions will be described in next 3 sections.