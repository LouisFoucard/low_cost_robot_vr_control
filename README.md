# VR controller for low cost robot [arm](https://github.com/AlexanderKoch-Koch/low_cost_robot)

This fork adds a VR controller. Works with any OpenVR compatible controller, tested with Valve Index knuckles.
Quite low latency, I estimate it at under <50ms. This is possible in particular thanks to OpenVR's future position estimation, which here is set to 50ms.
The 6d pose of the controller is obtained through OpenVR API, and the roll angle is used to control the wrist angle.
The 3 joint angles of the base, shoulder and elbow are calculated through inverse kinematics.
The main trigger of the Index controller is mapped to the claw opening.
