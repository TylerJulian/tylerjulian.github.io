---
title: "Wifi Toaster"
layout: categories
permalink: /toaster/
collection: categories
entries_layout: grid
classes: wide
sitemap: false
date: 2020-11-07T18:38:52+00:00

excerpt: "Wifi toaster is a normal toaster that is controlled over the web using an android app. The wifi toaster was our submission to the 2022 Hacklahoma event. We won best hardware hack and best use of matlab!"
header:
  teaser: /assets/img/beeclick_toast.jpg
---

The wifi toaster was born from laziness. It was from a student's desire to not get up to toast bread. The wifi toaster was our submission to the 2022 Hacklahoma event. We won best hardware hack and best use of matlab! Hacklahoma is a annual hackathon that is hosted at the University of Oklahoma. Jorge Exinia and I chose to make a very 'useful' product that everyone needs in their home. We chose this joke project as an excuse to learn how to connect ESP32 microcontrollers to an android application.

# Functionality

The WiFi toaster is a regular toaster that can be controlled remotely via a web-based Android application. The application enables users to load bread into the toaster and initiate the toasting process from anywhere with an internet connection. The toaster will then notify the user when the toast is ready. The app handles loading the toaster, starting the cooking process, and sending notifications upon completion. All controls can be wirelessly activated from any distance.

To determine the toast's doneness and whether it needs to be toasted again, we employed a MATLAB script that processes pictures of the toast. THe script isolates the toast and determines average color to approximate how toasted it is. 
{% include video id="0jk2vu83qBs" provider="youtube" %}

# How we built it
We began by 3D printing a breadbox that also serves as a hopper. Positioned above the toaster, the breadbox conceals a secret feature—an opening that releases the bread into the toaster upon pressing the button in the Android app. This opening is controlled by a servo and an ESP32 microcontroller.

Additionally, we 3D printed a rack and pinion mechanism responsible for lowering the lever on the toaster to initiate the cooking process. Another servo, also controlled by the ESP32 microcontroller, powers the rack and pinion.

To determine when the toast is finished, we utilized an ultrasonic sensor. When the toast pops out of the toaster, the app displays a notification to inform the user that their toast is ready.

The WiFi toaster operates entirely wirelessly. You can initiate the toasting process and leave the machine untouched until the toast is done. An ESP32 microcontroller connects to a cloud service, which the Android app also connects to, enabling seamless communication between the two devices.

# Challenges we ran into

Throughout the design and construction process of our hack, we encountered two significant challenges. The first hurdle was configuring and programming the ESP32 to establish connections with both the Android app and the cloud service. We dedicated a substantial portion of our time to resolving these connection issues.

The second challenge revolved around time constraints and 3D printing. Typically, when 3D printing components, you have the luxury of iterating through multiple designs. However, given that our prints often took more than six hours, and we had only 24 hours in total to complete the project, we had to ensure our designs were successful on the first attempt or make necessary modifications after printing to achieve functionality. Waiting for prints to finish also posed a challenge, requiring us to utilize our time effectively when impeded by unavailable parts.

# My Contributions to the team
In our team, I took charge of designing and constructing the hardware for the WiFi toaster and helped my teammate debug esp32 code. Additionally, I developed the MATLAB script used to determine the toast's level of doneness.