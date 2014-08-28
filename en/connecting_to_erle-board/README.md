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

Remember to connect the lipo battery, to prove it, to the ESC (+ and -) ends. You will need a XT60 connector for doing this.

![rover](..img/assembly_img/rover.jpg)
