
# **Non-Inverting Op-Amp Preamp for Electret Microphone**

## **Overview**
This project demonstrates a **non-inverting operational amplifier (op-amp) preamp circuit** designed for use with an **electret microphone**. The circuit uses the **LM358 op-amp** and operates on a **single-supply voltage** (5V). It is ideal for amplifying low-level audio signals for further processing or interfacing with audio systems (amplifiers).

![Circuit Schematic](/mic_preamp_schematic.png)

---

## **Features**
- Single-supply operation (5V).
- Also works with other op-amps like TL072
- Designed for electret microphones with an internal FET.
- Adjustable gain for signal amplification.
- Capacitive coupling to block DC offset.
- Simple and beginner-friendly design.

---

## **Circuit Description**
1. **Electret Microphone Biasing**:
   - A bias resistor provides power to the microphone's internal FET.
   - Coupling capacitor allows the AC audio signal to pass while blocking DC.

2. **Op-Amp Configuration**:
   - Non-inverting input (+) is fed with the microphone signal.
   - A voltage divider creates a virtual ground at mid-supply (2.5V) for single-supply operation.
   - Feedback resistor and input resistor sets the gain.

3. **Output Coupling**:
   - A capacitor is used at the output to remove any DC offset.

---

## **Bill of Materials (BOM)**
| **Component**       | **Value**       | **Quantity** |
|---------------------|-----------------|--------------|
| Op-Amp              | LM358 or TL072          | 1            |
| Bias Resistor       | 2.2kΩ            | 1            |
| Feedback Resistor   | 220kΩ           | 2            |
| Input Resistor      | 6.8kΩ            | 1            |
| Load Resistor (Optional) | 10kΩ       | 1            |
| Coupling Capacitor (Input) | 1µF       | 1            |
| Coupling Capacitor (Output) | 1µF     | 1            |
| Voltage Divider Resistors | 10kΩ       | 2            |
| Electret Microphone | 1             | 1            |
| Power Supply        | +5V DC           | 1            |

---

## **Circuit Schematic**
![Circuit Schematic](/mic_preamp_schematic.png)

---

## **Electret Mic Schematic**
![Electret Mic Schematic](/electret_mic_schematic.png)

---

## **How to Use**
1. **Assemble the Circuit**:
   - Connect the components as per the schematic.
   - Ensure correct polarity for capacitors.

2. **Power Up**:
   - Use a regulated 5V DC supply.

3. **Test the Circuit**:
   - Connect the output to an oscilloscope or audio amplifier to observe the amplified signal.

---

## **Calculations**
- **Gain**:  
 Voltage gain Av = 1 + (Rf / Rin),
Av = 1 + (R4 / R6) = 65.7 Gain

- **Input Coupling Capacitor (Cutoff Frequency) a.k.a High pass filter**:  
 Cutoff Frequency: Cutoff frequency (fc) in Hz: fc = 1/(2πRC), R7 = 10K, C1 = 1uf
fc = 15.92 Hz

---

## **Applications**
- Audio preamplifiers.
- Signal conditioning for microphones.
- Voice recognition systems.
- DIY audio projects.

---

## **License**
Non-Inverting Mic Preamp of Opamp by Mubarak Basha is marked with CC0 1.0

CC0: This work has been marked as dedicated to the public domain.

[View the full license details here](https://creativecommons.org/publicdomain/zero/1.0/)


---

## **Acknowledgments**
- Circuit designed by **Mubarak Basha**.
- Schematic created using **Figma**.

---

## **Contact**
For questions or feedback, feel free to reach out:
- **Email**: dev947824@gmail.com
- **Website**: [Mubarak Native](https://mubaraknative.github.io/contact.html)
