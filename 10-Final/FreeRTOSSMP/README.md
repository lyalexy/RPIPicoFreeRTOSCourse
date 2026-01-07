This project demonstrates how to run FreeRTOS-based tasks on a Raspberry Pi Pico (RP2040) using the Pico SDK.

The code shows how to create simple agent tasks such as an LED blink agent and a counter agent, and how to run tasks across the RP2040's two cores.

The `src` directory contains the application source. The `lib/FreeRTOS-Kernel` and `port/FreeRTOS-Kernel` directories contain the FreeRTOS kernel and the port configuration used by this project.

Build the project with CMake and Ninja by creating a `build` directory and running CMake configuration followed by a build. For example:

```bash
cmake -S . -B build
cmake --build build
```

Flash or load the resulting firmware using the workspace tasks or the Pico tools configured in the project (for example `picotool` or `openocd`). See the workspace tasks for exact commands.

If you want a line-by-line walkthrough of `src/main.cpp` or any agent implementation, ask and I will open and explain those files.
