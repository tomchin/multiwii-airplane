# multiwii-airplane
The purpose of this repository is to improve and add airplane features.  
Although multiwii have airplane mode, from dynamics perspective, airplanes are treated like copters.  
Airplanes have different dynamics than copters.

## TODO List

#### Add _turn coordinator indicator_
Use the accelerometer for computing the coordination angle

#### Fix the weird behavior of the rudder during banked turns
Efficient flight will never use the rudder for flat turns,
a good use of the rudder will be only for coordinate the flight path (mostly during banked turns).

1. first step just fix the behavior during banked turns.
2. limit or completely ignore the use of rudder for yaw stabilization.

#### Fix MAG mode
Avoid side sliding (this increase the stall speed), use only coordinated turns for fixing the heading direction, that mean use mostly ailerons.

#### Add airspeed sensor support
Try to use MPXV7002 as suggested by KaiK here: http://www.multiwii.com/forum/viewtopic.php?f=8&t=2450

#### Add auto-throttle mode
Use airspeed data to to maintain airspeed

#### Fix BARO mode
The throttle alone cannot always maintain altitude, elevator is also needed.

#### Split angle mode
Split ANGLE mode into two different systems:  
auto BANK angle mode - roll stick control the roll angle (like in ANGLE mode)  
auto PITCH angle mode - pitch stick control the pitch angle (like in ANGLE mode)  

### Trainer mode
* Add angle limits
* Add altitude limits
* Add fance
* ...

