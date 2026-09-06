# CycloidalGearReducer_8to1
A personal project consisting in developing a cycloidal 8 to 1 reducer compatible with a NEMA17 stepper motor with a D-shaft.
This follows directly my previous project of a robotic arm articulated by servo motors after noting the flaws, design and servos limitations (extreme play and backlash, bad repeatability, also not good-looking etc...).

Unlike servos (at least the one I used, DM996 and 9g), steppers don't know where the shaft is oriented, which is why I need a magnetic encoder (AS5600) to track it. Moreover, steppers can't generate a high torque, at least in this context of building a robotic arm, so I need some gear reduction system to multiply the initial torque of 0.4Nm in a compact housing, with no backlash, high precision and shock resistant.

I therefore chose the cycloidal type of reducers with a 8 to 1 reduction ratio, which, if well-designed enough, satisfies all my requirements and would give a torque of 3.2Nm (probably less because of friction...).

In this project, I learned how to use Autodesk Fusion CAD because I do not want to use Blender (which I used to build the servo robot arm), the operating principle of a cycloidal drive.

Sources of materials that helped me a lot:
www.youtube.com/watch?v=dv2URKU5YNU //most useful video for me for understanding cycloidal reducers
www.youtube.com/watch?v=stGwlJ-GMCY
youtu.be/OsS9-FzKN6s?si=D96ZwXOTy2uzee3U
www.youtube.com/watch?v=VbAhkESCRFM //what taught me almost everything i needed for using Fusion CAD 
youtu.be/jQ6LQBFZXmU?si=3ZcaHU4sGydaDMxd

Parts list:
26x 693ZZ Bearing                 www.amazon.fr/dp/B0FP4ZW9JP
2x 6702-2RS Bearing               www.amazon.fr/dp/B0GL6KSBSH
2x 6807-2RS                       www.amazon.fr/dp/B09HX12WTC
M3 Screws and Nuts                www.amazon.fr/dp/B0B3MGZ7T2 www.amazon.fr/dp/B0DPWZ53X4
AS5600 Magnetic Encoder           fr.aliexpress.com/item/1005009026945907.html
ESP32-S3 Microcontroller          fr.aliexpress.com/item/1005008845049090.html
TMC2209 V2.0 Stepper Motor Driver fr.aliexpress.com/item/1005010646278731.html
100µF Capacitor
some wires

The most difficult part for me in this project was to think about a step by step assembly process while making it compact and making every parts fit snuggly which led me to do a lot of iterations in certain models, even order an urgent express delivery for new parts, for example I realized very late that I needed much bigger bearings 6807-2RS because I did not think about needing a bigger output shaft with enough space for multiple screws to bear load, this adjustment rendered my gearbox to be too thick for my 20mm M3 screws which led to another express delivery of longer M3 screws etc, a defective caliper etc...

My experience of 3D modelling on Blender I gathered from the first lockdown translated really well to Fusion thanks to the parametric curve maths logic of FUsion made it much easier for me to keep track of all the dimensions otherwise impossible or very frustrating on Blender which uses a polygon mesh logic. This project took me 4 weeks to develop which would have taken months or maybe over year on Blender (the servo robot arm took me over 6 months).

