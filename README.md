# AtherStatement
Hackathon
# Assumptions:

1) Scooter have 3 axis gyroscope for its balncing as shown in this figure.

![ather2](https://user-images.githubusercontent.com/45059470/152825349-a0a5c85c-f880-41b7-866b-daeeede25978.jpg)
![ather4](https://user-images.githubusercontent.com/45059470/152825438-2d15417c-0320-40cb-98c1-9dd7e152e045.jpg)

2) We are considering following signal lights: Left Indicator(LI), Right Indicator(RI) and Tail Light(TL).

3) On moving handle bars left or right, it rotates around Z-axis.

4) When it is lean on either side (left or right), it rotates around X-axis.

5) When a speed breaker or some pothole come in the way (move up or down), it rotates around Y-axis.

6) After analaying data, we are setting some thresohold value for left and right turn or up and down movement.

7) If it crosses certain threshold, we consider it as a turn and turn ON the lights according to situation.

8) We are setting a certain value relative to threshold value, so if it falls again under that certain value, we are turning OFF the lights according to situation.

9) For turning in left or right direction, we are taking combination of leaning or rotating around X-axis, and rotating around X-axis.

10) When moving move or down, due to speed breaker or pothole, we are considering rotating around Y-axis.

11) Considering received_ts as timestamp data received at server so excluding it from analysis.
