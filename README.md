# Payload-Electronics
// Welcome to Payload Electronics 2022-2023. This year we are working on the research and developement of a payload that no collegiate team has achieved before. 
The goal is to become the first collegiate team to land something propulsively.
In order to achieve this goal we need to do some work that we don't have experience with.
Luckily for us as the electronics team we have done most everything before in some form. The new parts come in the form of thrust vectoring with servos, as well as
the use of a reaction or fly wheel.

We have several boards we will design to work together.

> ###### Sensor-Board
   We're isolating our sensors to one board, 
       BNO055- Orientation sensor, rotation and acceleration
       BMP180- Barometer, temps, altitude
       Adafruit Ultimate GPS- location bviously
       Camera- It's likely we'll use a camera onboard
>###### Power-Board
   We'll use this simply to mount batteries, and possibly merge this with the Buck-converter board.
   
>###### Buck Converter-Board
   Dependent on the Power board configuration,
     Buck converters are used to step down voltage. 
     Since we'll be using several different voltages throughout the boards, we'll use Buck converters to drop the voltage to each use.
     We will most likely be using a starting voltage of 14 Volts.
        We'll drop to a voltage for the motor, 6V for the servos, 5 Volts for the RasPi, which will supply 3.3 Volts to our sensors.
        
>###### Servo-Board
   This board will be where we house the matrix of wiring and control for our numerous servos.
     We'll have two for thrust vectoring, and another two for actuation of mechanical systems such as flaps and landing legs. 
     because we use PWM (Pulse Width Modulation) to control servose, we'll use a device that allows communication
     with the RasPi in order to create more PWM signals. This is because the RasPi simply doesn't have enough PWM pins to do it on its own.
     We will also supply power and control for the Motor in the flywheel from this board.
     
>###### RasPi Mounting
   We need a board to mount the RasPi inside PLOP, we'll likely stick this with the ignition circuit that starts the rocket motor.
   
        
       


  
