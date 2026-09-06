# CycloidalGearReducer_8to1
A personal project consisting in developing a cycloidal 8 to 1 reducer compatible with a NEMA17 stepper motor with a D-shaft.
This follows directly my previous project of a robotic arm articulated by servo motors after noting the flaws, design and servos limitations (extreme play and backlash, bad repeatability, also not good-looking etc...).

Unlike servos (at least the one I used, DM996 and 9g), steppers don't know where the shaft is oriented, which is why I need a magnetic encoder (AS5600) to track it. Moreover, steppers can't generate a high torque, at least in this context of building a robotic arm, so I need some gear reduction system to multiply the initial torque of 0.4Nm in a compact housing, with no backlash, high precision and shock resistant.

I therefore chose the cycloidal type of reducers with a 8 to 1 reduction ratio, which, if well-designed enough, satisfies all my requirements and would give a torque of 3.2Nm (probably a little less because of friction...).
