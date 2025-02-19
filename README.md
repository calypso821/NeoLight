

#### NeoLight Ambient Light project

NeoLightFX is a C++ application designed to drive programmable LED strips (WS2811/WS2812) with advanced visual effects. 
It supports both hardware (Raspberry Pi) and simulation (Windows) modes, with a focus on real-time processing of various input sources including video, images, and audio.

## Features

- **Multiple Input Sources**: 
    - video
    - camera capture
    - static images
    - audio

- **Dynamic Effects**: 
  - Rainbow effect
  - Progress/transition effects
  - Fade effects
  - Color correction and conversion
  - Weighted color extraction

- **Hardware Support**:
  - Raspberry Pi 3 integration with rpi_ws281x library
  - LED strip configuration (count, width, height)
  - Hardware and simulation modes

- **Remote Control**:
  - Socket-based client/server architecture (Linux and Windows)
  - IR remote control functionality
  - Command processing interface

- **Performance Optimizations**:
  - Transition processing at 120 FPS
  - Frame processing at 60 FPS
  - Precision timers for accurate timing
  - Threading support

- **Visual Controls**:
  - Brightness adjustment
  - Color intensity modification
  - Greyscale correction
  - Transition speed mapping

## System Architecture

The system is built around several key components:

- **RenderManager**: Controls the main rendering loop
- **InputSourceController**: Manages different input sources
- **FrameProcessor**: Handles frame transition and processing
- **EffectController**: Manages various lighting effects
- **HardwareController/SimulationController**: Hardware abstraction layer
- **Server**: Network interface for remote control

## Build Modes

- **SIMULATE**: For desktop development and testing
- **HARDWARE**: For deployment on Raspberry Pi hardware

## Deployment

The repository includes scripts for:
- Remote deployment
- Building
- Running on target hardware

## Requirements

- C++ compiler with C++11 support
- OpenCV for image/video processing
- CMake build system
- rpi_ws281x library (for hardware mode)

[FriSMS driver](friSMS_driver.md)

![image](images/Neopixel_strip.png)
![image](images/power.png)
![image](images/power_control.png)
![image](images/STM32.png)
![image](images/Rasphberry_PI.png)
![image](images/SPI.png)
![image](images/CaptureCard.png)
![image](images/zakljucekVIN.png)
![image](images/zakljucekOR.png)
