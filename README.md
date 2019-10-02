# Contiki Programming

Task 0 (10 marks): After having successfully installed Contiki on your system, change the code of the hello-world.c application to print your name and surname.
Useful resources: https://github.com/contiki-ng/contiki-ng/wiki

Task 1 (10 marks): Extend the hello-world.c app to do the following:
a) Once the mote is booted, the red LED is turned on for 2 seconds
b) Then, the red LED is turned off and the blue one is turned on for 4 seconds
c) Then, both are lit for 1 second and then turned off
d) Steps (a) to (c) are repeated indefinitely and corresponding messages are printed on the
terminal (e.g. red LED: ON)
Useful files: ‘contiki/core/dev/leds.h’ and ‘contiki/core/sys/etimer.h’
Other: https://github.com/contiki-ng/contiki-ng/wiki/Documentation:-Timers

Task 2 (15 marks): Extend the hello-world.c app to make use of the user-button. In particular, every time the button is pressed and for as long as the button is pressed, the green LED is lit. The green LED is turned off once the button is released.

Task 3 (20 marks): You are asked to develop a simple ‘ping-pong’ game on Contiki to be played with two RE-MOTES. In particular, once the motes are booted, a token is generated - you need to come up with a token generation mechanism such that eventually only one token exists between the two motes. The mote currently holding the token has its LED lit. Once the user button is pressed, then the token is transmitted to the other mote and the LEDs are turned off and on correspondingly. The process is continued indefinitely allowing the motes to exchange the token each time the user button of the token-holder is pressed.
