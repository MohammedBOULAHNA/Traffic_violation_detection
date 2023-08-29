# Traffic_violation_detection  

## Main problems
- Driver forgets a traffic code (for example: do not follow the red light). 
- Driving on some national network roads which haven’t any road signs. 
- Driver distraction ​to take the proper distance between vehicles. 
- Drivers' lack of respect for traffic regulations.
- Dangerous maneuvers. 
- Speeding.

## Why this project?  
Using this solution, we could help : 
- Saving drivers from paying fines 
- Improving road safety 
- Promote responsible driving that respects the highway code

## Project use case  
- Meeting road safety standards and reducing accident mortality by detecting and alerting the driver in real time about traffic violations. 

## Technical specification  
* Develop a system to detect objects on the road (road signs, traffic lights, etc.).  
* Develop a system capable of recognizing common violations such as speeding, disobeying traffic lights, etc.
* Design a model to estimate the braking distance between two vehicles.
* Integrate violation detection and braking distance prediction functionalities into a user-friendly interface.

## Steps to follow to develop the solution
1. Creation of a model for object detection (traffic signs, traffic lights)
2. Braking distance prediction
3. Development of a user interface for alerts: **Mobile application** 

## Functional Architecture of the system  
![image](https://github.com/MohammedBOULAHNA/Traffic_violation_detection/assets/124175118/980c83cf-629b-414f-8704-831009aa0f13)  
## Physical architecture of the system :  
![image](https://github.com/MohammedBOULAHNA/Traffic_violation_detection/assets/124175118/7193ae3e-fa41-4ac2-9af4-dba91a91e704)

## Technical tools used in the first phase: Developing a model for object detection  
1. YOLO(You Only Look Once) : An object detection model that recognized for {***Real-time detection, Complete object detection framework (detection & localization), Precision and efficiency***}  
![image](https://github.com/MohammedBOULAHNA/Traffic_violation_detection/assets/124175118/55642e6a-e646-4d4c-82e6-f3879f57e4df)  

2. Python: Programming Language used for test  
![image](https://github.com/MohammedBOULAHNA/Traffic_violation_detection/assets/124175118/c7fdd5d9-4aba-4665-beba-7ca2c9d97fdb)  

3. Roboflow: Where we extracted the database for the training  
![image](https://github.com/MohammedBOULAHNA/Traffic_violation_detection/assets/124175118/f1cdcd92-3a6c-4bd9-8417-0e906872fbb1)

## Importing the dataset and training the model for both "Traffic signs and traffic lights datasets"  
* Importing the model  
![image](https://github.com/MohammedBOULAHNA/Traffic_violation_detection/assets/124175118/2acdff68-a649-4b4a-a321-717af6921685)  
* Model training  
![image](https://github.com/MohammedBOULAHNA/Traffic_violation_detection/assets/124175118/adf0d9b8-dd21-4aaf-9576-9b32ad676d1c)
  
## Training results  
***Traffic signs dataset***  
![image](https://github.com/MohammedBOULAHNA/Traffic_violation_detection/assets/124175118/27e46f99-1fa3-4bf0-b6da-3e34e29ec439)

***Traffic lights dataset***  
![image](https://github.com/MohammedBOULAHNA/Traffic_violation_detection/assets/124175118/88525aa9-fd2e-4563-b9bf-c3df927b8824)

## Detection results  
![image](https://github.com/MohammedBOULAHNA/Traffic_violation_detection/assets/124175118/91d5f528-c782-4ad6-8ccc-aba6c5f210cb)

## Converting the model from its default format (pytorch) into TensorflowLite (more compatible with embedded systems)  
![image](https://github.com/MohammedBOULAHNA/Traffic_violation_detection/assets/124175118/4994dfac-cc32-47bc-a2d4-db98056e2312)  

## Deploy the model using a FLASK API  
* Test using videos
![image](https://github.com/MohammedBOULAHNA/Traffic_violation_detection/assets/124175118/f21c4f6f-6eb4-4d99-be80-8e48af0c94a9)
* Test using webcam
![image](https://github.com/MohammedBOULAHNA/Traffic_violation_detection/assets/124175118/a21d1341-0a8a-414d-a417-e9544429f27d)


