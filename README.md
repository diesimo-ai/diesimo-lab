# Diesimo Lab 

![Edge AI Platforms](./resources/images/cover.jpeg)

Welcome to the Open Edge AI Lab.

## Edge AI Models Garden

- Model Garden: [Hugging Face Collections (Coming soon!)](https://huggingface.co/collections/diesimo-ai/edge-ai-67856b736bc168b98abf3ee0)
- Demos: [Hugging Face Spaces (Coming soon!)](#)

In the meantime, find the best model suitable for your application requirements here: [Edge AI Model Zoos](https://github.com/afondiel/Edge-AI-Model-Zoo).


## Hardware Platforms

### (Ultra) Low Performance

![Arduino Nano 33 BLE Sense](./resources/images/arduino-nano/nano.jpeg)

| **Device**                  | Arduino Nano 33 BLE Sense          |
|-----------------------------|------------------------------------|
| **CPU**                     | 1-core nRF52840, @64MHz ARM Cortex-M4 32-bit (FPU)|
| **GPU**                     | None                              |
| **Memory**                  | 1MB Flash, 256KB RAM              |
| **Power Consumption**       | Ultra-low power modes             |
| **Storage**                 | None (onboard Flash)              |
| **Connectivity**            | BLE, NFC                          |
| **Camera/Display Support**  | None                              |
| **Sensors**                 | 9-axis IMU, temp, humidity, pressure, microphone, gesture, light |
| **I/O Pins**                | 14 digital, 8 analog, 12 PWM      |
| **Dimensions**              | 45mm x 18mm                       |
| **Use Case**                | TinyML, IoT, wearables            |

Technical specs: ([Source](https://docs.arduino.cc/hardware/nano-33-ble-sense/)) 

### Lightweight (Entry/Medium) Performance
![Raspberry Pi 3B](./resources/images/pi/pi.jpeg)

| **Device**                  | Raspberry Pi                            |
|-----------------------------|-----------------------------------------|
| **CPU**                     | 4-cores @1.2GHz Broadcom BCM2837 64bit |
| **GPU**                     | None                              |
| **Memory**                  | 1GB RAM                           |
| **Power Consumption**       | 4W (5V, 2.5A ≈ 12.5W, varies by load) |
| **Storage**                 | SD card                           |
| **Connectivity**            | WiFi, BLE, Ethernet, USB          |
| **Camera/Display Support**  | 8MP (up to 3840 x 2160)           |
| **Sensors**                 | None                              |
| **I/O Pins**                | Not specified                     |
| **Dimensions**              | Not specified                     |
| **Use Case**                | Lightweight IoT, smart home, education |

Technical specs: ([Source](https://www.raspberrypi.com/products/raspberry-pi-3-model-b/#Specification)) 

### High Performance Computing/Applications
![NVIDIA Jetson Nano](./resources/images/jetson-nano/jet-nano.jpeg)

| **Device**                  | NVIDIA Jetson Nano                |
|-----------------------------|------------------------------------|
| **CPU**                     | 4-Core ARM Cortex A57 MPCore          |
| **GPU**                     | 128-core Maxwell GPU (472 GFLOPS) |
| **Memory**                  | 4GB 64-bit LPDDR4 RAM                    |
| **Power Consumption**       | 20W (5V, 4A ≈ 3870 mW)            |
| **Storage**                 | MicroSD card (16GB UHS-1 minimum) |
| **Connectivity**            | None specified (Ethernet, USB supported) |
| **Camera/Display Support**  | 8MP (up to 3840 x 2160), Full HD 1080p+ |
| **Sensors**                 | None                              |
| **I/O Pins**                | Not specified                     |
| **Dimensions**              | Not specified                     |
| **Use Case**                | AI applications, neural networks, image processing |

Technical specs: ([Source](https://developer.nvidia.com/embedded/jetson-nano)) 

## Embodied Agents

For real-world data collection and testing. 

### Unmanned Ground Vehicles (UGVs)

(Lego sets) Robotics Platforms 

![ugv](./resources/images/embodied-agents/ugv-0.jpg)

![ugv](./resources/images/embodied-agents/ugv-1.jpg)


### Unmanned Aerial Vehicles (UAVs)

Drone

![uavs](./resources/images/embodied-agents/uavs.jpg)

## Resources

- [Edge AI Engineering (Main)](https://github.com/afondiel/edge-ai-engineering)
- [Edge AI Technical Guide](https://github.com/afondiel/computer-science-notebook/tree/master/core/systems/edge-computing/edge-ai/concepts)
- [Edge AI End-to-End Stack](https://www.qualcomm.com/developer/artificial-intelligence)
- [Edge AI Deployment Stack](https://github.com/afondiel/computer-science-notebook/tree/master/core/systems/edge-computing/edge-ai/concepts/deployment)
- [Edge AI Optimization Stack](https://github.com/afondiel/computer-science-notebook/tree/master/core/systems/edge-computing/edge-ai/concepts/optimization)
- [Edge AI Frameworks](https://github.com/afondiel/computer-science-notebook/tree/master/core/systems/edge-computing/edge-ai/concepts/frameworks)
- [Edge AI Platforms](https://github.com/afondiel/Edge-AI-Platforms)
- [Edge AI Model Zoos](https://github.com/afondiel/Edge-AI-Model-Zoo)
- [Edge AI Model Benchmarking](https://github.com/afondiel/Edge-AI-Model-Zoo/blob/main/model-bench-guide.md)
