![image](https://github.com/user-attachments/assets/acfc44c4-259a-4d3e-b3a5-363a1bfa809e)

# 💡 Arduino LED Light Sensor Trigger
This project uses an LDR (light-dependent resistor) to read ambient light levels and control three LEDs connected to an Arduino. When the light intensity falls below a certain threshold, the LEDs turn off, simulating an automatic lighting system.

# 🧰 Components Used
1 × Arduino UNO

3 × LEDs (any color)

3 × 220Ω Resistors (one per LED)

1 × Light Sensor (LDR)

1 × 10kΩ Resistor (for voltage divider)

Breadboard & jumper wires

USB cable (for uploading code)

# 🔌 Circuit Overview
LDR is connected to analog pin A0 using a voltage divider with a 10kΩ resistor.

LEDs are connected to digital pins:

Pin 11

Pin 12

Pin 13
Each LED has a 220Ω resistor in series to limit current.

GND is shared across the LDR, resistor, and LEDs.

# 🧠 Code Functionality
The LDR reads the surrounding light intensity.

The value is mapped inversely to brightness (bright → low number).

If the mapped brightness is greater than 100, all three LEDs turn on.

If it's lower, the LEDs turn off.

The system updates every 50 milliseconds.
