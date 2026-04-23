# Electro-Mechanical Propeller Vehicle (Breadboard Chassis)

An open-source hardware (OSHW) project demonstrating a parallel-circuit electro-mechanical vehicle. This design uniquely utilizes a standard breadboard not just as a prototyping area, but as the primary structural chassis of the vehicle.

## System Architecture
The vehicle operates on a purely analog, parallel DC circuit. The power delivery is gated by a main tactile switch, which then branches into three parallel nodes:
1.  **Propulsion Node:** A mini DC motor driving a propeller for aerodynamic thrust.
2.  **Illumination Node 1:** A current-limited red LED acting as the right headlamp.
3.  **Illumination Node 2:** A current-limited red LED acting as the left headlamp.

By utilizing a parallel configuration, the system ensures that the voltage drop across the motor does not dim the LEDs (which operate independently on their own branches with series resistors).

## BOM (Bill of Materials)
To replicate this build, the following electro-mechanical components are required:
* **Chassis:** 1x Half-size Breadboard (400 tie-points)
* **Power Source:** 1x 3V Battery Holder (2x AA Batteries)
* **Actuator:** 1x Mini DC Motor (3V-6V rated) with attached Propeller
* **Control:** 1x Push-Button / Slide Switch
* **Indicators:** 2x 5mm Red LEDs
* **Protection:** 2x Current Limiting Resistors (e.g., 100Ω - 330Ω)
* **Mobility:** 4x Plastic Wheels with axles
* **Wiring:** Standard solid-core jumper wires

## Circuit Schematic
![Circuit Schematic](./docs/car_schematic.png)

## Power Analysis & Physical Dynamics
The 3V DC source provides sufficient torque for the motor to generate aerodynamic thrust. The inclusion of resistors on the LED branches prevents thermal runaway and diode burnout, showcasing fundamental load-balancing in a mixed-component circuit. The breadboard provides a rigid yet modular foundation, allowing for rapid iteration of the center of gravity and weight distribution.

## Academic Context
Developed by Naz | TOBB ETU - Electrical and Electronics Engineering. 
This project serves as a foundational study in mechatronics, circuit topology, and open-source hardware documentation.
