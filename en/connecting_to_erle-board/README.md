# Connecting to erle-board

As mentioned before,  [APMover2](https://github.com/BeaglePilot/ardupilot/tree/master/APMrover2) works in skid steer mode, that meand that a typical four-wheel vehicles will drive with the wheels mechanically locked in synchronization on each side, and that the left-side drive wheels can be driven independently of the right-side drive wheels.

So when connecting to erle board we will need to connect the two ESC: the right side motors one and the left side motors one; to the output channels one and three.

Following the [Ardurover documentation](http://rover.ardupilot.com/wiki/table-of-contents/), we will find in the [APM setup](http://rover.ardupilot.com/wiki/setup/) section that the channel 1 correspondo to the left side motors and the channel 3 to the right side motors.

To sum up:

|**Channel**|**Motors**|
|-----|-----|
|1|left side|
|3|right side|

So you should connect the ESC following these specifications, that is the right side ESC to the channel 3 and the left side ESC to the channel 1.

Also when connecting to the channe 1 and 3, take **into account the position of the ESC**.
Usually the red wire from the ESC is the +, the black wire the – and the withe wire the pulse(Π) (for more info read the ESC especifications).Be careful to connect them in the proper way to the side connectors (marked in red in the image).

Remember to connect the lipo battery, to prove it, to the ESC (+ and -) ends. You will need a XT60 connector for doing this.

![rover](..img/assembly_img/rover.jpg)

You should, now, **check if all the wheels rotate in the same direction (forwards)**, do this before closing by screwing the top plate.If any of the wheels rotates backward then you should exchange the two wires connected to the motors(So, in our case the red wire goes up and the black goes down now). You don't need to touch the ESC connection, only the motors one.
