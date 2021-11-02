# 
# CNN-for-vibrational-events-in-phase-OTDR

With the help of an OTDR, it is possible to analyze the acoustic effects on a fiber-optic sensor distributed along the length. This allows you to understand in what place the impact took place and to establish the nature of the impact.
This is actively used in tracing gas leaks, monitoring the tightness of an oil pipeline, and in the problem under consideration - an alert system for unauthorized entry into a protected perimeter.

1) The physical principle of operation of sensing using OTDR
The laser module generates pulses with a narrow spectral width, which are sent to the sensor fiber. When an acoustic effect is applied, some of the beams are scattered back, changing their spectral density.
By analyzing the backscattered beams received, it becomes possible to find out the place and strength of the acoustic impact.
Below is a simplified diagram of the warning system.
![otdr_scheme](https://user-images.githubusercontent.com/73990802/139841978-3eed726f-7184-4720-828e-783c1d4a95d1.png)
The number of requests (pulses) is 1000 per second. Therefore, stacking the results of queries, we get a two-dimensional matrix, where the columns mean the distance, and the rows mean the time, the value of an individual element of the matrix reflects the strength of the acoustic impact.
Various acoustic influences have a characteristic acoustic wave distribution, thus possessing unique feaches. This is how we, for example, can classify walking, digging, jumping, etc.
Below is an example of a processed signal describing a human step.
![showing_signal](https://user-images.githubusercontent.com/73990802/139841982-95715c28-5deb-45b5-8372-013362337dbe.jpg)
