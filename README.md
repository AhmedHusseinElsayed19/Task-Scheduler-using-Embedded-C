# Task-Scheduler-using-Embedded-C
 Implement a task to toggle an LED and use the parameter to select the color, e.g. by an enum. Use
it to toggle the green led with a frequency of 0.5 Hz.
 Instead of using timer 1, use the scheduler for debouncing the buttons by calling button_checkState
as task every 5 ms. Don’t change the library code for the button.
 When pressing the joystick button, turn on the yellow LED. Turn it off when pressing the joystick
button again or after 5 seconds, whatever comes first.
 Implement a stop watch, which starts and stops when pressing the rotary button. Use the LCD to
show the current stop watch time in seconds and tenths of seconds. You do not need to implement
a reset of the stop watch (you may use the reset button for this purpose).
. Make use of the library created in previous exercises (LCD, LED, and Buttons).
E Make sure, that the taskDescriptors you use are not local variables, which run out of scope after
scheduling – this is a sure means of producing undefined behavior!
E Do not use _delay_ms() (or any other busy waiting) for waiting multiple milliseconds!
