# Dead Reckoning

Dead reckoning is a way of finding the estimated position of a moving object by using information about where it started. It is a navigation method used to calculate a current position based on a previously known position, speed, direction and elapsed time. Sailors used it long before satellites existed, when all they had was their heading, their speed and a clock.

## How it works

Imagine a robot starting from a known point. If the robot knows how far its wheels have moved and the direction it is facing, it will be able to estimate where it is after moving. It keeps updating its position as it moves.

`new position = old position + (speed × time × direction)`

## Example

A simple example: a robot heads east at 2 m/s for 5 seconds, so it has moved 10 m east. Then it turns north and goes at 1 m/s for 4 seconds. Its estimated position is now 10 m east and 4 m north of where it began. Each step is just added onto the last one.

## Where it is used

It is used in different areas, especially in robotics, cars, ships and aircraft. In robotics, IMUs can be used to measure movements and changes in direction, and wheel encoders can count how far the wheels have turned.

If you drive into a tunnel and the GPS signal is lost, the system can keep guessing your position from your speed and turns.

## Limitations

A common issue with dead reckoning is that it is not always accurate, or at least not completely accurate.

Small mistakes in the sensor readings can add up as the robot continues moving. A wheel might slip a little or the heading might be off by a degree.

After a few seconds this hardly matters, but after a few minutes the estimated position can be far from the real one. Because every new position depends on the old one, the error keeps growing.

## Reducing the error

To reduce this, dead reckoning is often combined with other sources like GPS, cameras or known landmarks, which correct the position every so often. Methods such as the Kalman filter can also mix several sensors together to get a better estimate.

## Summary

In summary, dead reckoning is a process of estimating your position, or keeping track of where you are, by adding small changes in your position over time. It is the integration of velocity with respect to time.

## Sources

1. Wikipedia. "Dead reckoning." https://en.wikipedia.org/wiki/Dead_reckoning (accessed 30 September 2026)
2. Merriam-Webster. "Dead reckoning." https://www.merriam-webster.com/dictionary/Dead%20reckon (accessed 30 September 2026)
3. SBG Systems. "Dead reckoning navigation." https://sbg-systems.com/glossary/dead-reckoning-navigation (accessed 30 September 2026)
4. Daisch Sensor. "What is Dead Reckoning Navigation?" https://daischsensor.com/what-is-dead-reckoning-navigation/ (accessed 30 September 2026)
5. Training-Promotion71. "Dead Reckoning and Interpretation." r/freewill, Reddit. https://www.reddit.com/r/freewill/comments/1kpmvj0/dead_reckoning_and_interpretation/ (accessed 30 September 2026)
