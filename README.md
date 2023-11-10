# RASC-AL-GULLS-RX
This is the receiving end of the RASC-AL Project. Will focus on the PWM of an LED for initial prototyping

Laser Sensor Prototyping Stages: 
1 - PWM out to an LED, 50% brightness.
2 - PWM out to an LED, step brightness up and down in intervals of 10% with some user input like a keyboard stroke
3 - PWM out, change brightness in steps with respect to a timer, ie. "timer has run for 70sec, time to change PWM duty cycle from X% to X+Y%" (hypothetical)
4 - ADC in, store value & do continual average. if ADC in is .5V higher than continuous average, stop the average and start a timer. compare current ADC value to held average, if it dips back down to that value +- a little wiggle room, reset the timer.
5 - tie it all together, PWM level shifts to three discrete values for timer NO HIT, <70s, and >70s as per system description
