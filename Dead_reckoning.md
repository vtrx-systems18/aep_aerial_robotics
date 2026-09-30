# Dead Reckoning

Dead reckoning is a method of estimating one's current position based on previous known positions. This is a relative navigation method used by sailors before the arrival of satellites by estimating the current position based on a previously known one, speed, and direction, and time passed. Dead reckoning is called "dead" because it can be deadly if not done correctly.

## How it works

Imagine a robot that starts from a known position and knows how far its wheels have rolled, and the direction it is facing and then will have enough information to determine its position after a certain movement, by updating its position as it moves. The relationship between distance, speed, and time as follows:

`new position = old position + (speed × time × direction)`

## Example

A simple example would involve a robot moving in a straight path and then turning to move in another path. For example, a robot starts at position 0,0, faces east and moves at 2 m/s for a duration of 5 seconds. The robot's speed and time are multiplied to get its position on the x-axis: `25=10`. It then turns north and moves at 1m/s for 4 seconds. This is done by multiplying its speed by the duration of the movement: `14=4`. The robot's position is therefore (10,4), that is, 10 meters east and 4 meters north of its initial position. The new position is calculated by adding the previous one to its new position.

## Where it's used

This method is used in different fields, especially in robotics, where IMUs can be used to measure the robot's movements and rotations, and wheel encoders can be used to determine how far the robot has traveled.

When inside a tunnel, a car's GPS may lose signal and therefore the car's position must be estimated based on its speed and turns.

## Limitations

The main limitation of dead reckoning is cumulative error, or inaccuracies in the estimation of the current position due to errors that occur as the robot moves.

Due to errors in the measurement of the robot's rotation and direction, or wheel slippage, or any other reason small errors may appear as the robot moves. These errors are added to the position as the robot moves forward and therefore accumulate over time. After only a few seconds of errors, the estimated position of the robot can be very different from its real position. This limitation is explained as the errors in the prediction of the robot's position are compounded through the system with every iteration of the loop (every calculation). The longer the robot is dead reckoning, the more inaccurate its position will be.

## Reducing the error

Dead reckoning is usually coupled with other systems in order to reduce these errors. The GPS in phones and cars has the ability to use both information from satellites and the phone's own sensors to estimate the position of the phone. By comparing the position from multiple devices, an average can be calculated in order to reduce error. Another method that reduces error is using a Kalman filter.

## Summary

By summarizing this article on the concept of "dead reckoning", it can be said that dead reckoning is a method of constantly estimating one's position by summing one's movements relative to a fixed point, taking speed and direction into account. Dead reckoning is the integration of velocity with respect to time.

## Sources

1. Wikipedia. "Dead reckoning." https://en.wikipedia.org/wiki/Dead_reckoning (accessed 30 September 2026)

2. Merriam-Webster. "Dead reckoning." https://www.merriam-webster.com/dictionary/Dead%20reckon (accessed 30 September 2026)

3. SBG Systems. "Dead reckoning navigation." https://sbg-systems.com/glossary/dead-reckoning-navigation (accessed 30 September 2026)

4. Daisch Sensor. "What is Dead Reckoning Navigation?" https://daischsensor.com/what-is-dead-reckoning-navigation/ (accessed 30 September 2026)

5. Training-Promotion71. "Dead Reckoning and Interpretation." r/freewill, Reddit. https://www.reddit.com/r/freewill/comments/1kpmvj0/dead_reckoning_and_interpretation/ (accessed 30 September 2026)
