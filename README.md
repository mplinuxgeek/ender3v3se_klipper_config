# Klipper Configuration for Ender 3 V3 SE with Nebula Pad Offsets

This is a custom Klipper configuration for the 2022 Creality Ender 3 V3 SE. It combines aspects of the publicly available configurations from `bootuz-dinamon` and `0xD34D`. However, several issues were encountered with those configs, such as incorrect offsets that caused initial purge lines to print off the bed and the bed meshing to be off center. 

To resolve these problems, I extracted and applied the correct X/Y offsets and various other parameters from the Nebula Pad's V3 SE configurations. This ensures that the bed mesh is properly centered and the purge line is correctly placed on the print bed.

## Key Modifications:
- **X/Y Offsets:** Adjusted based on Nebula Pad's configuration for accurate bed meshing and purge line placement.
- **Bed Mesh:** Corrected mesh area to properly cover the entire bed, ensuring precise leveling.
- **Stepper Configurations:** Defined accurate limits and homing settings for X, Y, and Z axes.
- **BLTouch Probe Offsets:** Set `x_offset` and `y_offset` to -24.0 and -20.0, respectively, for proper probe alignment.
- **Endstops:** Adjusted the position of the X, Y, and Z endstops to match the physical setup.
- **Z Offset Note:** This configuration uses a **KE-style ceramic hotend**, which may require different Z offsets. **Make sure to adjust the Z offset to a safe value** before starting any prints. Incorrect Z offset can cause the nozzle to crash into the bed or print too high.
