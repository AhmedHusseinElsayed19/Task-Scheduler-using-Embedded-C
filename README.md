1. Develop a task to control the LED, allowing the choice of its color via a parameter, typically an enum. This task should enable the toggling of the green LED at a frequency of 0.5 Hz.

2. Instead of utilizing timer 1, incorporate the scheduler to manage button debouncing. Achieve this by scheduling the "button_checkState" task to run every 5 milliseconds. It's important not to modify the library code for the button.

3. Implement functionality that, upon pressing the joystick button, activates the yellow LED. The LED should deactivate when the joystick button is pressed again or after a 5-second interval, whichever occurs first.

4. Create a stopwatch feature triggered by pressing the rotary button. Utilize the LCD to display the current stopwatch time in seconds and tenths of seconds. No need to implement a stopwatch reset function; the reset button can handle this purpose.

5. Ensure that the taskDescriptors you employ are not local variables, as this could result in undefined behavior when they go out of scope.

6. Avoid the use of busy waiting functions such as "_delay_ms()" for handling multiple-millisecond delays, as they may lead to inefficient code execution.
