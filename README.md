# NYU-W12
Assignment 12.1 Documentation

This assignment was the most difficult to complete.  Not because of the difficulty level but due to the videos did not fully reflect the XR packages installed on the Unity system.  Below I will go through the high level process of creating the environment and XR rig and interactions:

Apart from the standard packages, the following project packages were installed:
•	Unity recorder
•	ProGrids
•	ProBuilder
•	TextMeshPro
•	Oculus XR Plugin
•	XR Plugin Management
•	XR Interaction Toolkit

Environment:
The environment was created using the provided SNAP Prototyping assets.  I followed along with the videos of this week and created a maze environment.  I installed the floor and walls and used the ProGrid for quick grid alignment.
Apart from floor and walls of the maze, I also installed a desk and a cube.  The cube has an XR grab interactable component on it.  I installed a script that would open door when the XR Rig would be within a preset region in the vicinity of door.

VR Setup:
The following Game Objects and components were created as part of the VR scene.

XR Rig:
After installing all the above packages, and particularly the last package “XR Interaction toolkit” – I was able to create  XR Rig, now also known as the XR Origin.  Below is a hierarchy of the XR Origin (Action based):

XR Origin (GameObject)
o	Camera Offset
o	Main Camera
o	LeftHand Controller
o	RightHand Controller

The XR Interaction Manager (That was created automatically) needs an Input Action Manager component.  The Input Action Manager needs to have a reference to the Input Action Map – where all the Headset (Oculus Quest 2) controller mappings are defined.
XR Interaction Manager (GameObject)
o	Input Action Manager

Now for creating the locomotion, teleportation and turn system, the scene needs a Locomotion Game Object with various components onto it.

Locomotion (GameObject)
o	Locomotion system (comes preinstalled)
o	Teleportation provider
o	SnapTurn Provider
o	Continuous Turn provider (use either this or SnapTurn, but not both)
o	Continuous Turn Provider

After some settings, as discussed in video below (YouTube), I was able to get the VR application working. 
URL:   How to Make VR Games in 2022 - Updated Unity VR Tutorial - YouTube

A video of the assignment is given below:
URL:  https://www.dropbox.com/s/fag1y5wnk8kzdkj/Assignment%2012.1%20Create%20a%20Maze.mp4?dl=0

A project repository is placed in the following GitHub link (Public):
URL:  https://github.com/iyounas101/NYU-W12





