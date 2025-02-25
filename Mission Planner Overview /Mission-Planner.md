# Mission Planner Overview

Mission Planner is a full-featured ground station application for the ArduPilot open source autopilot project. This page contains information on the background of Mission Planner and the organization of this site.
### What is Mission Planner

![image](https://github.com/user-attachments/assets/67765632-ea07-439c-9b1b-18b7c784d212)

Mission Planner is a ground control station for Plane, Copter and Rover. It is compatible with Windows only. Mission Planner can be used as a configuration utility or as a dynamic control supplement for your autonomous vehicle. Here are just a few things you can do with Mission Planner:

# Plan Tab

## Using Waypoints

### Waypoint Table

- WP Radius: This will be the radius the plane has to fly through before moving on to the next objective

- Loiter Radius: The radius the plane will loiter in if set to loiter

- Default Altitude: This is the distance the plane will fly above the takeoff point. The altitude where the plane is armed is the new reference of zero altitude

- Verify Height: This is used to prevent the plane from flying into a hill inadvertently. So if a waypoint is on have this selected mission planner will increase the ALT setting by the height of the hill

- Add Below: This button will add a waypoint in the table below without placing it on the map

![image](https://github.com/user-attachments/assets/fc19755b-3c63-47f3-a530-16e4d3de9dbc)


## Tips


## Mission Commands 



## Creating a simple quadplane mission plan
1. Open the mission planner plan tab
2. (Optional) Go to the flying field on the map
3. On the map right click on the desired takeoff location and select set home
4. Selcet the way point radius size (default = 90m)
5. Left click on the map to place a waypoint close to the home waypoint then select the command VTOL_TAKEOFF. Make sure the home waypoint is inside the takeoff waypoint's area
 
![image](https://github.com/user-attachments/assets/dbcbab4c-6679-4c99-8533-63917e258389)

7. Continue placing waypoints to design your quadplane's path

![image](https://github.com/user-attachments/assets/afdfea0e-796e-4441-ac83-521b45beee79)

8. To complete your mission plan with a quadplane have your second last waypoint be the command DO_VTOL_TRANSITION and your final waypoint be the command VTOL_LAND for the quadplane to land (The quadplane can land wherever and is not restricted to landing at the home waypoint) ![image](https://github.com/user-attachments/assets/749bcdee-c381-47d2-a1e9-e00c3c10fcf2)
9. To save you mission plan press the Save File button on the right side of the screen select the location you wish to save it. To continue working on a mission plan or to load for simulation use press the Load File button on the right side of the screen (Make sure to manually save your mission plan everytime or it will be lost when closing the mission planner)

# Simulation Tab

The Simulation tab provides a SITL (Software in the Loop) simulation capability. Many typical frame types for each Vehicle type have been created. This allows you to see the expected behavior for vehicles in missions, or with a joystick attached, actually be able to fly/drive the vehicle simulation as if with RC. This allows you to see potential effects of parameter changes on vehicle behavior or explore mission generation, without risking your vehicle first.

## Setup 

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
2. Once the simulation is set up go to the mission planner plan tab
3. Create or load an existing mission plan for the Quadplane to take (follow the steps in [creating a simple mission plan section](#Creating-a-simple-quadplane-mission-plan). ![image](https://github.com/user-attachments/assets/2dce5701-bb59-4aa2-a338-f9da5efa00b2)                                                                                    
4. Press the load file button on the right screen and select the save mission plan from wherever its stored on your computer. To load the mission onto the simulated quadplane by pressing the write then the read button the right side of the screen
5. Open Mission Planner's Data tab
6. If the plane icon isn't over the home waypoint repeat step 4
7. Go to the action tab and from the drop down list left of the Set Mode button select QSTABILIZE then press set mode![Screenshot 2025-01-11 165332](https://github.com/user-attachments/assets/0408a32f-7f5e-42e3-8794-9eba656cbf63)
8. Press the Arm/Disarm button to arm the quadplane and in the HUD it should now say ARMED ![image](https://github.com/user-attachments/assets/adbaf28d-092b-4787-ad32-d4f50daf4cf8)
9. Open the drop down list used in step 7 and select Auto then press the Set Mode button. The mission should start and the as seen in the HUD the altitude should start rising
10. If the waypoints disappear after step 9 go back to the plan tab and press the write button then repeat step 9 again and the quadplane should take off

