# L1-embedded-thermostat

This project builds and runs C++ code on the Raspberry Pi.

---
## Setting Environment Variables

The program needs to know the host and port for the server it connects to.

1. **Create Host**
   ```bash
       export HOST=<server_computer_ip>
    ```

2. **Create Port**
   ```bash
       export HOST=<listening_port_of_server>
    ```

You can check that these were set correctly by running the command:

   ```bash
       echo $HOST $PORT
   ```


## Build and Run with Makefile

The easiest way to create the executable is to use the provided `Makefile`.

1. **Build**
   ```bash
       make
    ```

2. **Run**
   ```bash
       make run
    ```

Or run this command manually:
g++ -std=c++20 -I./include -L../WiringPi src/main.cpp -o main -lwiringPi
./main

