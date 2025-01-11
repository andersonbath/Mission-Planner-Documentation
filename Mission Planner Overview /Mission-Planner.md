### Mission Planner Overview

Mission Planner is a full-featured ground station application for the ArduPilot open source autopilot project. This page contains information on the background of Mission Planner and the organization of this site.
### What is Mission Planner

![image](https://github.com/user-attachments/assets/67765632-ea07-439c-9b1b-18b7c784d212)

Mission Planner is a ground control station for Plane, Copter and Rover. It is compatible with Windows only. Mission Planner can be used as a configuration utility or as a dynamic control supplement for your autonomous vehicle. Here are just a few things you can do with Mission Planner:

## Creating a simple mission plan

###
# Simulation Page

The Simulation tab provides a SITL (Software in the Loop) simulation capability. Many typical frame types for each Vehicle type have been created. This allows you to see the expected behavior for vehicles in missions, or with a joystick attached, actually be able to fly/drive the vehicle simulation as if with RC. This allows you to see potential effects of parameter changes on vehicle behavior or explore mission generation, without risking your vehicle first.

# Setup 

- Select the simulation page
- Advanced users only:
  - (Optional) Select the applicable model
  - (Optional) To wipe any previous changes made in the config page that are causing simulation errors select the check box labeled wipe
  ![image](https://github.com/user-attachments/assets/7650590a-3863-49d8-b0f4-d1fd7e5b319f)
  ![image](https://github.com/user-attachments/assets/f2c9776c-eb35-4a9f-be37-340213158935)
- Select the applicable the firmware to run in the simlation
![image](https://github.com/user-attachments/assets/60f5533d-89c1-42a2-838e-4f216b7affec)
- Select which version you want to use between Latest and Stable (you should be fine with either) 
![image](https://github.com/user-attachments/assets/e74dbd32-caf8-41d6-bc27-69fce410b481)

After completeing all the setup steps the firmware will start downloading and launch the simluation. 

## Setting Up a Quadplane Simulation
1. Follow the [setup section](#Setup) and make sure the model is set to quadplane
2. Once the simulation is set up go to the mission planner plan page
3. Create or load an existing mission plan for the Quadplane to take (follow the steps in [creating a simple mission plan section](#Creating-a-simple-mission-plan). Press the load file button on the right screen and select the save mission plan from wherever its stored on your computer ![image](https://github.com/user-attachments/assets/3df651d0-07a4-4c3f-9ac4-69f42f0101d7)                                                                                    
4. Load the mission onto the simulated quadplane by pressing the write then the read button the right side of the screen !

