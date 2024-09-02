New `generic-cartesian` kinematics

**Discourse:**
https://klipper.discourse.group/t/new-generic-cartesian-kinematics-incl-corexyu-corexyuv-generic-idex-and-awd/17510

**Klipper code available**
https://github.com/dmbutyugin/klipper/tree/generic-cartesian

---------------------------------------------------------------

# **Core XYU  - dual carriage** 

**Video demonstration of kinematics including IDEX mode COPY and MIRROR:**  https://www.youtube.com/watch?v=s85qpCWupn4


![CoreXY+U_dual_carriage_frame](https://github.com/user-attachments/assets/361c5da8-9979-4da5-a37e-768a20e0a299)


**Klipper configuration**


```
#--------------------  Motor X ----------------------------------#-
[carriage x] 
....
[stepper x]
kinematics: x+y
....
[tmc2208 stepper x]  
....
#--------------------  Motor Y ----------------------------------#-
[carriage y]
....
[stepper y]
kinematics: x-y
....
[tmc2208 stepper y]   
....
#--------------------  Motor U ----------------------------------#-
[dual_carriage u] 
primary_carriage: x
safe_distance: 35
....
[stepper u]
kinematics: u+y
....
[tmc2208 stepper u]   
....
```

