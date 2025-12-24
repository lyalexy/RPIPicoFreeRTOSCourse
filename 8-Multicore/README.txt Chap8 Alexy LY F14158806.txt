README.txt Alexy LY F14158806

OS-8 (Chapter_8-Multicore) SMP 

This project Demonstrates FreeRTOS on the Raspberry Pi Pico (RP2040) using both cores (SMP-style multicore example) to run simple agent tasks (LED blink, counters, etc...).

Agents are implemented as FreeRTOS tasks (each agent wraps a task loop).
For example, BlinkAgent toggles a GPIO at intervals; CounterAgent increments and may communicate via queues/semaphores.

The RP2040 has two cores: code may start a secondary core and assign tasks or use inter-core synchronization primitives (mutexes/queues) provided by FreeRTOS/Pico SDK.

I made no modifications to the code and just ran it.
