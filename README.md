# 2-Way Traffic Light System Using IC 4017, 555 Timer, and Diodes

## Project Overview

This project demonstrates a **2-way traffic light control system** using a 4017 Decade Counter, 555 Timer IC, and diodes. The circuit simulates a traffic light sequence for a 2-way intersection with two sets of red, yellow, and green LEDs. Each set changes automatically based on a timed sequence, making this an effective model for traffic light operation.
<p align="center">
    <img src="https://github.com/thynavy/Auto_Traffic_Light_circuit/blob/main/4017.png" />
    <br />
    <strong>Figure 1: The 2-way traffic light control system</strong>
</p>
<p align="center">
    <img src="https://github.com/thynavy/2-way_traffic_light_control_system/blob/main/LED.jpg" />
    <br />
    <strong>Figure 2: Traffic Light LED</strong>
</p>

## Features

- **Automated Traffic Light Sequence:** Operates two sets of traffic lights (each with red, yellow, and green LEDs) in a timed sequence, simulating real-world traffic control.
- **Diode Isolation:** Diodes are used to control the LED flow and prevent reverse currents, ensuring stable operation and extending the lifespan of the LEDs.
- **Adjustable Timing:** A potentiometer allows for fine-tuning of the 555 timer's clock speed, which controls the timing of each LED, enabling customizable light intervals.
- **Efficient Design:** Built with minimal components around two popular ICs—the 4017 and the 555 timer—plus diodes, making it a beginner-friendly yet reliable project.

## Components Used

- **IC 4017 Decade Counter:** Cycles through 10 output pins (Q0 to Q9) with each clock pulse, enabling controlled LED sequencing for the traffic lights.
- **IC 555 Timer:** Configured in astable mode to generate a continuous clock pulse that drives the 4017 counter. The clock pulse timing determines the LED switching rate.
- **Diodes:** Diodes are included to manage the current flow between LEDs and outputs of the 4017, isolating each LED to avoid interference or backfeeding between the outputs.
- **LEDs:** Two sets of red, yellow, and green LEDs represent the two traffic lights, each controlled by specific 4017 output pins.
- **Resistors and Capacitors:** Used for LED current limiting and for setting the timing interval on the 555 timer.

## How It Works

1. Clock Generation with the 555 Timer: The 555 timer provides a steady clock pulse to the 4017. The pulse frequency can be adjusted with a potentiometer, allowing for customized traffic light intervals.
2. LED Sequence Control with the 4017 Decade Counter: Clock pulses advance the 4017 through its output pins (Q0 to Q9), each of which lights up a specific LED in sequence.
3. Diode Isolation:
   - Diodes are placed on certain output pins of the 4017 to prevent backfeeding, ensuring each LED only receives current from its intended output pin.
   - This prevents one traffic light’s signal from affecting the other, ensuring that each set of LEDs operates independently without cross-interference.
4. Traffic Light Logic:
   - The first traffic light is controlled by outputs Q0, Q1, and Q2, which turn on the red, yellow, and green LEDs in sequence.
   - The second traffic light is managed by outputs Q3, Q4, and Q5, with its own red, yellow, and green LEDs.
   - After Q5, the 4017 resets to Q0, creating a continuous cycle.

This circuit serves as an excellent demonstration of timing control, current management using diodes, and sequencing for traffic applications. It’s a practical project for anyone learning about digital logic, timing circuits, and diode use for current isolation.


