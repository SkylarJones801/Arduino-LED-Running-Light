# Running Light Project

**Introduction**

The Running Light project is a simple electronic project based on the Arduino Uno that creates dynamic visual effects by sequentially lighting up and turning off LEDs. This project is not only suitable for beginners to learn how to control hardware with Arduino but also helps understand basic programming logic and circuit knowledge. 

In this project, we will use 7 LEDs and write code to control them to light up in sequence, forming a flowing effect. This project can serve as an introductory practice for learning digital electronics and microcontroller programming.

**Materials Needed:**

* 1 x Arduino UNO board
* 7 x LEDs
* 7 x 220Ω resistors (one for each LED to limit the current flowing through the LED)
* 1 x Breadboard (optional, for easy connections)
* Assorted jumper wires (for connecting components)
* ## Online Simulation

Before building the hardware, it's recommended to create an online simulation to identify any potential issues in the circuit or code. 

**Benefits of Online Simulation:**

* Catch errors early in the development process
* Test different configurations without needing physical components
* Save time and resources

**Using PCBX for Online Simulation (Optional):**

This project can be simulated using online PCB simulation tools like PCBX. Joining the PCBX community allows you to simulate your projects for free.

![LED running light](https://github.com/SkylarJones801/Arduino-LED-Running-Light/blob/main/LED%20Running%20Light.gif)

**Connection Steps:**

**Connecting LEDs and Resistors:**

1. **LEDs to Arduino:** Connect the long leg (anode) of each LED to a designated digital pin on the Arduino Uno (pins 3, 4, 5, 6, 7, 8, 9).
2. **Resistors to LEDs:** Connect the short leg (cathode) of each LED to a 220Ω resistor.
3. **Resistors to GND:** Connect the other end of each 220Ω resistor to the GND pin of the Arduino Uno.

**Running Light Effects (Code Implementation):**

The provided code utilizes the `loop()` function to implement various LED display modes:

* **Individual Lighting:** Each LED lights up sequentially, staying on for 100 milliseconds before switching to the next LED.
* **All On:** All LEDs illuminate simultaneously for 1 second.
* **Individual Extinguishing:** Similar to individual lighting, LEDs turn off one by one, staying on for 100 milliseconds each.
* **Individual Blinking:** Each LED blinks independently, turning on for 300 milliseconds three times with a 300-millisecond pause between blinks.

*Note: The specific code implementation for these effects is not provided here. Refer to the provided code source for details.*

**Looping the Effects:**

After completing each mode, the program introduces a 1-second delay before repeating the entire sequence, creating a continuous loop.

**Join the PCBX Community:**

For free online simulation of your project, consider joining the PCBX community: https://www.pcbx.com/forum?mtm_campaign=E&mtm_kwd=git


While the 3D simulation feature is still a work in progress, we would love to hear your suggestions and expectations. It's an open-source community; any sharing and feedback is welcome.Your feedback will help our engineering team enhance the platform and better serve our users.Thank you!
