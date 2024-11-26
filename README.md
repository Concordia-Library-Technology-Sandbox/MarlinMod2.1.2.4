# Concordia University - Sandbox Division  
## Custom Firmware for 3D Printer  

This repository contains a slightly modified version of **MARLIN 2.1.2**, tailored for the Sandbox Division's custom 3D printer. The changes made are designed to optimize printer performance and adapt the firmware to specific hardware configurations.

The original MARLIN README has been included at "OldREADME.oldmd" for archival purposes and is not a product of Sandbox Division's work.  

---

## What's New?  

### Modifications in `Configuration.h`:  
- **X_HOME_DIR**:  
  - Set to `1` to modify the printer's homing direction.  

- **Extruder Rate Adjustments**:  
  - Three values were tested for the extruder rate: `500`, `94.5`, and `100`.  
  - The current value is set to `100`.  

- **X_DRIVER_TYPE**:  
  - Updated to `DRV8825` to match the stepper driver hardware.  

- **Safe Homing**:  
  - Enabled to ensure the printer homes safely within the build area.

---

## Areas for Improvement  

### 1. Auto-Leveling  
- Implement and fine-tune the auto-leveling feature to improve print consistency and accuracy.  

### 2. Extruder Rate Calibration  
- Determine the ideal extruder rate for consistent material flow.  

### 3. Speed Optimization  
- Experiment with faster rates for the new version of the firmware.  

---

## How to install?

Currently we use Auto Marlin Build, an addon for Visual Studio that automatically sets all the dependacies and pushes the code to the arduino board AtMega2560 for this particular printer (2) simply follow these steps:

1.Reset the printer
2.Connect USB to computer where the code is hosted
3.Build the code and make sure not errors appear at the compily
4.Hit upload to Atmega2560 and it should upload directly


## Notes  
This custom firmware is actively under development and may require additional fine-tuning for specific use cases. Contributions and suggestions from the team are welcome to help refine its functionality.  

For questions or support, contact the **Concordia University - Sandbox Division** development team.  
