# BenchBot Add-on: Robots for use with Isaac Sim (Omniverse)

This add-on contains robot definition files for using simulated Isaac robots. These robots have been designed to work with Omniverse-powered Isaac Sim, and tested with the current version (2021.2.1)

The following robot definitions are provided:

- carter_omni

## How these were created in Omniverse

1. Start with the example Carter robot from _I can't remember where the one with `Carter_ROS.usd` came from???_
2. Make a copy of that directory
3. Edit ROS specific settings in `Carter_ROS.usd`, and model specific settings in `Robots/Carter/carter_v1.usd` (the default prim in `Carter_ROS.usd` references `Robots/Carter/carter_v1.usd`):
   - frame settings of the ROS components change the frame in the message but not the TF name
   - TF name is changed by renaming the primitives, which must be done in the `carter_v1.usd` file
   - for something to move relative to a prim, it must be nested underneath that prim?
4. Create a \*.zip with a YAML file
