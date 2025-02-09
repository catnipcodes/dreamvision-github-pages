---
title: Dreamvision 98 for macOS
---


### A fantasy console built for graphics experimentation, gamedev and livecoding

Dreamvision 98 is a fantasy console - an emulated computer / game console, but not based on a real machine. You can program your own apps and games as well as playing existing ones.

It has a unique, retrofuturist design - a 1990s fever dream of a future console. It's also almost entirely GPU driven, everything from the CPU to the audio system runs on your computer's graphics processor.

## Important: Dreamvision is in alpha

The current version of Dreamvision is still in active development. It's fully usable and should be very stable, but some features are missing or incomplete (especially the sound system, ability to import images and sounds, disk support, and advanced drawing APIs for sprites and 3D).

In addition, the API might change in future, breaking any code you write now (this will be avoided if possible).

## Hardware specification

- 4096 core CPU
- 64MB RAM
- 960 x 540 resolution 60hz display with HDR
- Shader based graphics with support for multiple color and blending modes
- CD quality stereo sound

## Developing for Dreamvision

It's designed to be powerful while staying easy and fun to program. It's designed as a live coding environment, meaning when you save your code it compiles and updates while still running. This means you can edit your game while its running, and it can be used for live performance too.

Dreamvision apps are written in Metal Shading Language (MSL, C++14 with a few minor differences and its own standard library), and there's an easy to use API for 2D graphics and full in-app help documenting everything.

The code editor has all your favourite features, because when you open a file in Dreamvision it automatically opens the code in the default editor on your system. 

Dreamvision is a highly parallel design, with 4096 CPU cores. This means you can run large simulations, or dedicate a full core to to thousands of enemies for physics and AI in your game. 

Graphics are shader based, meaning you can do fullscreen shader effects and combine that with the 2D drawing API. For example you can draw a circle with the color set to white, or you can set the color per pixel to apply a texture or gradient.

One of Dreamvision's unique features are hardware registers you can poke to switch things like the color mode and hardware blending. This means you can switch between RGB and YUV color modes, and between replace, alpha and additive blending.
