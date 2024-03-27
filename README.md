## GoTo Modifier for my Dobsaonian Telescope


The goal of this project is to make a GoTo system for my dobsonian telecope that I got back in the start of 2023. It should be computer controlled and be able to move to a selected target and also automatically track it. To make the GoTo I will primaraly be using an arduino fitted with a cnc shield that controls two NEMA 17 stepper motors witht the help of a rotary encoder. To aid my creation I will be using my schoools lazer vutter and 3d printers.








### Starting Point
The Telescope I bought was a f/5 130mm dobonsian by skywatcher. I bought a dobsonian over a equatorial mount for simplicty reasons as well as for the wooden base and easy to remove hardwear.

<img src="https://usa.all-startelescope.com/cdn/shop/products/S11710_Heritage150_LeftFront_1800x1800_3ac2cdd2-1c1b-43c0-9795-49c9df086e0c-sw_600x600.jpg?v=1645512990" width=50% height=50%>

The telescope moves on two differant mounts, the base (Azimuth); the vertival screw (Altidude). The first step I did was to figure out a way to connect the motor and the axis. The solution was to create two gears that would glue to the bases and allow for the motor to move the gears in any way possible. 

<img src="https://github.com/grahamwa/Go_To_Telescope/assets/88165698/33e6c0f1-e2ff-4fec-838b-c6da134f178a" width=50% height=50%>



### Arduinio Communication Unit

After some trial and error I found that I2C protical for arduino works the best to connect a rotary ecoder to and arduino with a cnc shield. Connecting the two board allowed me to start playing with slave and master programs eventually yielding workable code which uses the second ardunio to gather rotational inputs about the encoder. Currently at a button push it switches motors and turing left yeild a postive turn and right a negative turn. 


For housing I lazer cut I box from thin wood on the cutter, adding holes for cables and fans. 
