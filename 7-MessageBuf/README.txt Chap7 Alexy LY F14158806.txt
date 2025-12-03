README.txt Alexy LY F14158806

OS-7 (Chapter_7-MessageBuf) Buffer

This project demonstrates how to use FreeRTOS on the Raspberry Pi Pico to manage multiple concurrent tasks controlling LEDs, decoding counters, handling I/O, and printing system runtime statistics. The behavior is driven by several "Agent" classes (BlinkAgent, CounterAgent, DecoderAgent, IOAgent) and a main supervisory task.

The program sets up several FreeRTOS tasks, each managed by an “Agent” object:

BlinkAgent
Toggles LED at GPIO 0 at a defined interval.

CounterAgent
Drives four LEDs as a binary counter on GPIO 2–5.

DecoderAgent
Reads output from the CounterAgent and decodes the count value.

IOAgent
Handles input/output behavior and drives LED on GPIO 15.

MainTask
Supervises everything, periodically prints runtime stats.


In this case, we want 2 Pico communicating together over UART to display the same value on four LEDs in sync.
-First we connect correctly the GPIO pins to the LEDs and we implement the project file .uf2 into the
2 Raspberry Pi Pico.
-Then to connect succesfully the 2 Raspberry Pi Pico, we use a wire that connects the GPIO Pin 16 from one to the GPIO Pin 17 of the other one.


