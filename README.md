# Movement-of-Robot-Joints
## Aim:  
To move and drive the joints of the robot using python API.

## Equipment’s required:

Visual Components Premium 4.3.

## Procedure:

1. 	In the eCatalog panel, Collections view, browse to Models by Type>Robots>Visual Components and then add a Generic Articulated Robot to the 3D world.
2. 	Click the Modeling tab, and then add a Python Script behaviour. The script editor will open automatically when you add the behaviour.
3. 	In the script editor, add the code and then compile the code.

## Program
```python
from vcScript import *
from vcHelpers.Robot2 import *
def OnRun():
pos = [[1,30],[2,40],[3,90]]
robot = getRobot()
robot.driveJoints (0,0,0,0,0,0)
delay(5)
for i in pos:
robot.Controller.moveJoint (i[0],i[1])
delay (5)






```
## Output
### 1. Generic Articulated Robot
![image](https://github.com/Murali-Krishna0/Movement-of-Robot-Joints/assets/149054535/f057f51b-d4aa-4c83-9715-3b9bf283e945)


### 2. robot.driveJoints(0,0,0,0,0,0)
![image](https://github.com/Murali-Krishna0/Movement-of-Robot-Joints/assets/149054535/d391cd57-4eac-426c-bf80-26f1d5186552)


### 3. Movement of Joint1
![image](https://github.com/Murali-Krishna0/Movement-of-Robot-Joints/assets/149054535/470f571a-ac73-4f31-ad08-9d7f7dad6c00)


### 3. Movement of Joint2
![image](https://github.com/Murali-Krishna0/Movement-of-Robot-Joints/assets/149054535/97e6350a-eaba-42fb-8a52-4f61f7290714)


### 3. Movement of Joint3
![image](https://github.com/Murali-Krishna0/Movement-of-Robot-Joints/assets/149054535/cd276d0b-3eaa-4e29-b17a-b6463467a8bc)


## Result 
Thus the different robots joints are moved with the help of python list.


