# CycloidalGearReducer_8to1
A personal project consisting in developing a cycloidal 8 to 1 reducer compatible with a NEMA17 stepper motor with a D-shaft.
This follows directly my previous project of a robotic arm articulated by servo motors after noting the flaws, design and servos limitations (extreme play and backlash, bad repeatability, also not good-looking etc...).

Unlike servos (at least the one I used, DM996 and 9g), steppers don't know where the shaft is oriented, which is why I need a magnetic encoder (AS5600) to track it. Moreover, steppers can't generate a high torque, at least in this context of building a robotic arm, so I need some gear reduction system to multiply the initial torque of 0.4Nm in a compact housing, with no backlash, high precision and shock resistant.

I therefore chose the cycloidal type of reducers with a 8 to 1 reduction ratio, which, if well-designed enough, satisfies all my requirements and would give a torque of 3.2Nm (probably a little less because of friction...).

In this project, I learned how to use Autodesk Fusion CAD because I do not want to use Blender (which I used to build the servo robot arm), the operating principle of a cycloidal drive.

Sources of materials that helped me a lot:
https://www.youtube.com/watch?v=dv2URKU5YNU //most useful video for me for understanding cycloidal reducers
https://www.youtube.com/watch?v=stGwlJ-GMCY
https://youtu.be/OsS9-FzKN6s?si=D96ZwXOTy2uzee3U
https://www.youtube.com/watch?v=VbAhkESCRFM //what taught me almost everything i needed for using Fusion CAD 
https://youtu.be/jQ6LQBFZXmU?si=3ZcaHU4sGydaDMxd

Parts list:
26x 693ZZ Bearing www.amazon.fr/dp/B0FP4ZW9JP
2x 6702-2RS Bearing www.amazon.fr/dp/B0GL6KSBSH
2x 6807-2RS www.amazon.fr/dp/B09HX12WTC
M3 Screws and nuts www.amazon.fr/dp/B0B3MGZ7T2 www.amazon.fr/dp/B0DPWZ53X4

The most difficult part for me in this project was to think about a step by step assembly process while making it compact and making every parts fit snuggly which led me to do a lot of iterations in certain models, even order an urgent express delivery for new parts, for example I realized very late that I needed much bigger bearings 6807-2RS because I did not think about needing a bigger output shaft with enough space for multiple screws to bear load.



My experience of 3D modelling on Blender I gathered from the first lockdown translated really well to Fusion, also, the parametric curve maths logic on FUsion made it much easier for me to keep track of all the dimensions otherwise impossible or very frustrating on Blender which uses a polygon mesh logic. This project took me 4 weeks to develop which would have taken months or maybe over year on Blender (the servo robot arm took me 6 months).

