# Introduction
The Motor Control Board (MCB) is a network node used to control a single DC motor.
It will interface on our standardized bus and must implement some common control strategies.

# Encombrement
* lwh: 12x25x6 mm
* No connections (SOLDER ALL THE WIRES) -> hole

# Wanted electrical features
* Debug RGB LED
* Interface to quadrature coder with at least 32 bits + 5V power @ 200 mA
* Interface to potentiometer (not at the same time as encoder).
* 5V voltage arrives on a separate wire.
* Can drive at least the same current and voltage as last year.
* Motor current sense, both signs with RC filter.
* Measure power input voltage with RC filter.
* PAD for CAN termination resistance
* Decoupling cap for all voltages.
* Input voltage : 9.6V-16.8V.
* CAN Interface.
* SWD + traceout pour debug et prog trous métallisés
* Inputs : A/B/I + 1 * (GPIO + 3.3V + GND).
* MCU: STM32F302K8
* Quartz Oscillator
* Chain cards -> big holes for 2 wires.

# Wanted software features
* Current, speed and position control with ramps
* Interface to the CVRA bus.
* preemptive RTOS
* Bootloader
* Programmable en 20 secondes
* Mesurer certaines grandeurs et pouvoir les importer dans Numpy / MATLAB.
* Synchronisation des timestamps.
* Unit tests for everything.
* Self test y compris étage de puissance.

# Application Notes
* Placer les composants à 45 degrés
