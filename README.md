# LM317-Based-Adjustable-Voltage-Regulator-Circuit

### The LM317 device is an adjustable three-terminal positive-voltage linear regulator capable of supplying more than 1.5 A over an output-voltage range of 1.25 V to 37 V. It requires only two external resistors to set the output voltage.
### This is a adjustable voltage regulator circuit from LM317 datasheet shown on the image below.
<img src="designbyTI.JPG" width = "400" height = "300" >
Design Requirements : 

1. R1 and R2 are required to set the output voltage.

2. CADJ is recommended to improve ripple rejection. It prevents amplification of the ripple as the output voltage
is adjusted higher.

3. Ci is recommended, particularly if the regulator is not in close proximity to the power-supply filter capacitors. A
0.1-µF or 1-µF ceramic or tantalum capacitor provides sufficient bypassing for most applications, especially
when adjustment and output capacitors are used.

4. CO improves transient response, but is not needed for stability.

5. Protection diode D2 is recommended if CADJ is used. The diode provides a low-impedance discharge path to
prevent the capacitor from discharging into the output of the regulator.

6. Protection diode D1 is recommended if CO is used. The diode provides a low-impedance discharge path to
prevent the capacitor from discharging into the output of the regulator

Vo is calculated as shown in Equation below. Iadj is typically 50 µA and negligible in most applications.

Vo = Vref (1 + R2 / R1) + (Iadj × R2)

The voltage across the feedback resistor R1 is about 1.25V constant. Due to this reference voltage, a constant current of 100uA flows through the adjust terminal. Due to the 1.25V reference voltage, a current flows through resistor R2.
