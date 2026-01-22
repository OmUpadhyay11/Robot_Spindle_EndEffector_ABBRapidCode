# Robot_Spindle_EndEffector_ABBRapidCode

## Project Summary:
ABB RAPID code for testing and running a robot-mounted spindle end-effector to cut plywood sheets into predefined parts for BBQ wall manufacturing.
This repository contains the first step of the BBQ wall production process: using an ABB robot + spindle to cut a standard plywood sheet into multiple wall panel components, which are later assembled onto a 2x2 frame.

## Project Details / Tools Used:
- ABB robot RAPID modules (.mod)
- ABB RobotStudio (virtual controller simulation + RAPID debugging)
- Fusion360 CAM post-processing to generate spindle toolpaths
- Fusion360 2D Contour operations executed sequentially for an optimized cutting route
- ABB RAPID programming language
- WorkObject and ToolData are calibrated for the fabrication table setup, and the cutting tool is configured for a 3/8 inch kerf.

## What this code does:
- Cuts a 4 ft x 8 ft plywood sheet into smaller parts based on predefined patterns for efficient high volume manufacturing
- Supports 4 cutting patterns (each pattern has its own RAPID modules)
- Runs multiple contour paths in sequence for efficient routing and reduced cycle time
- Automates spindle control through a digital output (spindle ON before plunge, OFF at end)

## Validation
- Simulated code on ABB RobotStudio, verified functionality and tested on actual IRB 6700 MH3 Robot in facility.
