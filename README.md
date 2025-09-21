# Oscilloscope (EJ03)

An embedded oscilloscope project designed to interface with a PC for real-time waveform display. Developed using Arduino, MATLAB, and Python for visualization, with responsive hardware and software integration.

## Features

- Dual-channel signal capture (0–5V)
- Trigger functionality with adjustable level
- Scalable voltage and time axes (manual + autoset)
- Pause/Resume waveform for precise measurement
- Quick shut-off switch for safety
- USB-powered (5V @ 300–400 mA)
- MATLAB + Python GUI plotting support
- Responsive UI (<20ms reaction time to button input)

## System-Level Testing

System inputs/outputs and requirements were verified via:

- Power Interface Validation
- Probe Voltage Handling (0–5V, DC offset response)
- Display UI/Plot Scaling and Trigger Tests
- Engineering Requirements (connectivity, autoset, freeze, fast response)

## Demo Videos

- [Power & Probe Verification](https://drive.google.com/file/d/1qpPxgj_2ELeq_hVIDmS6AkScGJFoJmDg/view?usp=sharing)
- [Display/Interface Interaction](https://drive.google.com/file/d/10gETVLNk9-uiuTsQ3BNzPl2V_6j1PxNv/view?usp=sharing)
- [Trigger, Scaling & Pause Test](https://drive.google.com/file/d/144kXtIBlEre2H5gJudbySwPas5wJp2iQ/view?usp=sharing)

## Software Highlights

**MATLAB GUI:**  
- Real-time plotting using serial data
- Dynamic trigger level, autoscaling, and responsive logging

**Python GUI:**  
- Tkinter interface using Matplotlib
- Identical plotting and functionality to MATLAB (slower performance)

## Artifacts

- Arduino Schematic
- PCB Layout + Design
- Pseudocode for state management
- CAD Enclosure Design

## Authors

- Holden Cooper  
- Alexander Reed  
- Hugo Paulino Korte

## Repo Contents

- `matlab/` - MATLAB implementation of GUI
- `python/` - Python implementation (Tkinter)
- `pcb/` - Schematic & layout files
- `cad/` - Enclosure 3D models
- `test_docs/` - System verification documentation
