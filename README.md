# Movement-of-Robot-Joints
## Aim:  
To move and drive the joints of the robot using python API.

## Equipment’s required:
Visual Components Premium 4.3
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
![image](https://github.com/gpavana/Movement-of-Robot-Joints/assets/118787343/84aaa924-2646-4e7f-a55d-ceda5f6201b0)

### 2. robot.driveJoints(0,0,0,0,0,0)
![image](https://github.com/gpavana/Movement-of-Robot-Joints/assets/118787343/46293726-8d10-4318-9027-76c11d64132c)

### 3. Movement of Joint1
![image](https://github.com/gpavana/Movement-of-Robot-Joints/assets/118787343/3b88805a-04a4-4a49-9192-06e614920a9f)

### 4. Movement of Joint2
![image](https://github.com/gpavana/Movement-of-Robot-Joints/assets/118787343/f898596f-d0da-4048-9a9d-93b2cb8cb721)

### 5. Movement of Joint3
![image](https://github.com/gpavana/Movement-of-Robot-Joints/assets/118787343/9e053e7d-975f-456e-98c0-9287425bd79f)

## Result 
Thus the different robots joints are moved with the help of python list.


