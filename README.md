# README.md

# Oscilloscope 

An embedded oscilloscope project designed to interface with a PC for real-time waveform display. Developed using Arduino, MATLAB, and Python for visualization, with responsive hardware and software integration.

## Authors
- **Holden Cooper**  
- **Alexander Reed**  
- **Hugo Paulino Korte**

## Table of Contents
- [Features](#features)
- [System-Level Testing](#system-level-testing)
- [Demo Videos](#demo-videos)
- [Software Implementation](#software-implementation)
- [Hardware Artifacts](#hardware-artifacts)
- [Repository Structure](#repository-structure)

## Features

- **Dual-channel signal capture** (-5 – 5V input range)
- **Trigger functionality** with adjustable level control
- **Scalable voltage and time axes** (manual adjustment + autoset)
- **Pause/Resume waveform** capability for precise measurement
- **Quick shut-off switch** for safety compliance
- **USB-powered operation** (5V @ 300–400 mA)
- **MATLAB + Python GUI** plotting support
- **Responsive user interface** (<20ms reaction time to button input)

## System-Level Testing

System inputs/outputs and requirements were verified through comprehensive testing:

- **Power Interface Validation** - USB power supply verification and stability testing
- **Probe Voltage Handling** - 0–5V range validation with DC offset response testing
- **Display UI/Plot Scaling** - Scaling functionality and trigger level testing
- **Engineering Requirements** - Connectivity, autoset functionality, freeze capability, and fast response verification

## Demo Videos

- [Power & Probe Verification](https://drive.google.com/file/d/1qpPxgj_2ELeq_hVIDmS6AkScGJFoJmDg/view?usp=sharing)
- [Display/Interface Interaction](https://drive.google.com/file/d/10gETVLNk9-uiuTsQ3BNzPl2V_6j1PxNv/view?usp=sharing)
- [Trigger, Scaling & Pause Test](https://drive.google.com/file/d/144kXtIBlEre2H5gJudbySwPas5wJp2iQ/view?usp=sharing)

## Software Implementation

### MATLAB GUI Implementation
- **Real-time plotting** using serial data acquisition
- **Dynamic trigger level** adjustment with visual feedback
- **Autoscaling functionality** for optimal waveform display
- **Responsive logging** system for user interactions

### Python GUI Implementation
- **Tkinter interface** using Matplotlib for plotting
- **Identical functionality** to MATLAB implementation
- **Cross-platform compatibility** with slower performance compared to MATLAB

## Hardware Artifacts

**System Prototype:**

<img width="161" height="210" alt="Oscilloscope Prototype Hardware" src="https://github.com/user-attachments/assets/691cc487-abe5-4199-be97-239549bf357a" />

**PCB Layout and Design:**

<img width="382" height="246" alt="PCB Layout and Schematic Design" src="https://github.com/user-attachments/assets/efe00784-668f-417f-bf13-6776731c8e78" />

**Waveform Display Interface:**

<img width="501" height="270" alt="Real-time Waveform Display" src="https://github.com/user-attachments/assets/9a91f9b3-88c2-4f9a-950d-aa7c4b9e1634" />

## Technical Specifications

### Hardware Requirements
- **Microcontroller:** Arduino-compatible board
- **Power Supply:** USB 5V (300-400mA current draw)
- **Input Channels:** 2 analog inputs (0-5V range)
- **Communication:** Serial interface at 115200 baud
- **Safety Features:** Hardware power disconnect switch

### Software Requirements
- **MATLAB:** R2018b or later with Instrument Control Toolbox
- **Python:** 3.7+ with matplotlib, numpy, pyserial, tkinter
- **Operating System:** Windows, macOS, or Linux support

### Performance Specifications
- **Sample Rate:** Real-time continuous sampling
- **Response Time:** <20ms for user interface interactions
- **Voltage Resolution:** Determined by Arduino ADC (10-bit)
- **Trigger Sensitivity:** Software-configurable threshold

## Testing and Validation

The system has undergone comprehensive validation including:

- **Interface Definition Testing** - All system interfaces verified against specifications
- **Engineering Requirement Verification** - Each requirement tested with documented procedures
- **Performance Benchmarking** - Response time and accuracy measurements
- **Safety Compliance** - Power and signal handling safety verification

All testing procedures and results are documented in the `test_docs/` directory with accompanying video demonstrations.

## Contributing

Contributions to improve functionality, performance, or documentation are welcome. Please ensure all changes maintain compatibility with existing hardware and software implementations.

## License

This project is developed for educational purposes. Please respect institutional guidelines regarding academic work usage and distribution.
