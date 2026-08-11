# Otto-Bot-Dance-Robot
Arduino-based 4-servo OTTO biped robot with walking, moonwalk, kicking and automatic dance movements.

# OTTO Bot – 4 Servo Biped Dance Robot

A simple Arduino-based OTTO-style biped robot controlled using four servo motors.

The robot uses two leg/foot servos and two hip/side servos to perform walking, running, turning, moonwalk, kicking, swinging, flapping, and predefined dance movements.

The project uses the `Oscillator` library to generate smooth servo movements and supports servo trim calibration using EEPROM.

## Features

* 4-servo biped robot control
* Automatic dance sequence
* Walk and run movements
* Forward and backward movement
* Left and right turns
* Moonwalk left and right
* Kick animations
* Swing and flapping movements
* Servo trim calibration
* Smooth oscillator-based movements
* Neutral servo position at 90°

## Servo Connections

| Servo | Function                     | Arduino Pin |
| ----- | ---------------------------- | ----------- |
| RR    | Right Foot / Right Leg Servo | D5          |
| RL    | Left Foot / Left Leg Servo   | D4          |
| YR    | Right Hip / Side Servo       | D3          |
| YL    | Left Hip / Side Servo        | D2          |

## Libraries

* Servo
* Oscillator
* EEPROM

## Power

Use a stable 5V external power supply for the four servo motors.

Make sure the Arduino GND and servo power-supply GND are connected together.

Avoid powering all four servos directly from the Arduino 5V pin when the robot is operating under load.

## Main Movements Included

`walk()`, `run()`, `backyard()`, `turnLeft()`, `turnRight()`, `moonWalkLeft()`, `moonWalkRight()`, `crusaito()`, `swing()`, `upDown()`, `flapping()`, `kickLeft()`, `kickRight()`, `drunk()`, `goingUp()` and `noGravity()`.

The main `dance()` function combines several of these movements into one continuous OTTO dance routine.
