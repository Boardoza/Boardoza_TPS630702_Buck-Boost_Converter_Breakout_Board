# Boardoza TPS630702 Buck-Boost Converter Breakout Board

The TPS630702 is a high efficiency, low quiescent current buck-boost converter suitable for applications where the input voltage can be higher or lower than the output voltage. Output currents can go as high as 2A in boost mode and in buck mode. The buck-boost converter is based on a fixed frequency, pulse-width modulation (PWM) controller using synchronous rectification to obtain maximum efficiency. At low load currents, the converter enters Power Save Mode to maintain high efficiency over a wide load current range. The converter can be disabled to minimize battery drain. During shutdown, the load is disconnected from the battery.

<!-- ChatGPT: The TPS630702 High-Efficiency Buck-Boost Converter Breakout Board is designed for applications requiring a stable power supply with wide input voltage ranges. This board can efficiently convert input voltages both above and below the desired output, making it ideal for battery-powered devices. It features automatic mode transition, low quiescent current, and robust protection features to ensure reliable performance in portable electronics. -->

### [Click here to purchase!](https://www.ozdisan.com)
|Front Side|Back Side|
|:---:|:---:|
| ![ Front](./assets/TPS630702%20Front.png)| ![ Back](./assets/TPS630702%20Back.png)|

---
## Key Features
- Input Voltage Range : 2.0V to 16V
- Output Voltage Range : 3.3V to 9V
- VSEL simply allows output voltage change
- You Can Select Second Voltage Between 5V, 7.5V, 9V with VSEL When HIGH
- 2A Output Current in Buck Mode
- 2A Output Current in Boost Mode (VIN = 4V ; Vout = 5V)
- Automatic Transition Between Step Down and Boost Mode
- Output Discharge Option
- Load Disconnect During Shutdown
- Input /Output Over Voltage Protection
- Up to 95% Efficiency

<!-- ChatGPT: 
- Wide Input Voltage Range: Supports input voltages from 2.0V to 16V, suitable for various power sources.
- Adjustable Output Voltage: Provides output voltages from 3.3V to 9V, easily adjustable using VSEL.
- Dual Voltage Selection: VSEL pin allows switching between 5V, 7.5V, or 9V output when set to HIGH.
- High Output Current: Delivers up to 2A in both buck and boost modes, providing robust power delivery.
- Automatic Mode Transition: Seamlessly switches between step-down and boost modes based on input voltage.
- Output Discharge and Load Disconnect: Features output discharge and load disconnect during shutdown to minimize battery drain.
- Comprehensive Protection: Includes input/output overvoltage protection for enhanced safety.
- High Efficiency: Achieves up to 95% efficiency, optimizing power usage and reducing heat generation.
- Power Save Mode: Maintains high efficiency over a wide load current range by entering Power Save Mode at low currents.
- Compact and Versatile: Ideal for battery-powered devices and applications requiring stable voltage regulation. -->
---

## Technical Specifications
**Input Voltage:** 2.0V - 16V

**Input Voltage Type:** Molex 2 pin 2.50mm header

**Functions:** Buck-Boost Regulator

**Output Voltage:** 3.3V, 5V, 7.5V, 9V (Selectable)

<!-- 
**Output Current:** 2A (Buck Mode), 2A (Boost Mode)

**Efficiency:** Up to 95% 
-->

**Operating Temperature:** -40°C ~ +150°C

**Board Dimensions:** 40mm x 60mm


---
## Board Pinout
| ( J1 ) Pin Number | Pin Name | Description |
| :---: | :---: | --- |
| 1 | VIN | Voltage Input Pin (2-16V) |
| 2 | GND | Ground |

| ( J2 ) Pin Number | Pin Name | Description |
| :---: | :---: | --- |
| 1 | PG | The PG signal is generated based on the status of the output voltage monitor. The power good circuit operates as long as the converter is enabled and VIN is above the undervoltage lockout threshold. |
| 2 | GND | Ground |

| ( J3 ) Pin Number | Pin Name | Description |
| :---: | :---: | --- |
| 1 | VOUT | Adjustable buck-boost converter output (3.3V - 5V - 7.5V - 9V) |
| 2 | GND | Ground |

| ( JP1 ) Pin Number | Pin Name | Description |
| :---: | :---: | --- |
| 1 | LOW | GND |
| 2 | EN | Regulator enable pin. Default connected to “HIGH”. if You want to disable the regulator, Just jumper it to “LOW”. |
| 3 | HIGH | VIN voltage level |

| ( JP2 ) Pin Number | Pin Name | Description |
| :---: | :---: | --- |
| 1 | LOW | Open drain power good output |
| 2 | PS/SYNC | The PS/SYNC pin has two functions: Switching between forced PWM mode and power save mode. Synchronizing to an external clock applied at pin PS/SYNC. When PS/SYNC is set HIGH, the device operates in power save mode at low output current. The power save mode is disabled when PS/SYNC is set LOW. The device then operates in forced fixed frequency PWM mode independent of the output current.  Default Connected to LOW. |
| 3 | HIGH | VIN voltage level |

| ( JP3 ) Pin Number | Pin Name | Description |
| :---: | :---: | --- |
| 1 | LOW | Open drain power good output |
| 2 | V_SEL | Voltage scaling input. A high level on this pin enables a transistor which pulls pin FB2 to GND. Default connect to “LOW”. It means  output voltage 3.3V. If you want to choose second voltage, just jumper it to “HIGH”, and then jumper it only one pad on “9V - 7.5V - 5V”. |
| 3 | HIGH | VIN voltage level |

| Pin Name | Description |
| :---: | --- |
| 9V | 9V Pad for Second Voltage Selection. Adjusted Resistors for Feedback Pin of Regulator. |
| 7.5V | 7.5V Pad for Second Voltage Selection. Adjusted Resistors for Feedback Pin of Regulator. |
| 5V | 5V Pad for Second Voltage Selection. Adjusted Resistors for Feedback Pin of Regulator. |


---
## Board Dimensions

<img src="./assets/TPS630702 Dimension.png" alt=" Dimension" width="450"/>

---
## Step Files

[Boardoza TPS63070.step](./assets/TPS630702%20Step.step)

---
## Datasheet

[Boardoza TPS63070 Datasheet.pdf](./assets/TPS630702%20Datasheet.pdf)

---
## Version History
- V1.0.0 - Initial Release

---
## Support
- If you have any questions or need support, please contact support@boardoza.com

---
## License

Shield: [![CC BY-SA 4.0][cc-by-sa-shield]][cc-by-sa]

This work is licensed under a [Creative Commons Attribution-ShareAlike 4.0 International License][cc-by-sa].

[![CC BY-SA 4.0][cc-by-sa-image]][cc-by-sa]

[cc-by-sa]: http://creativecommons.org/licenses/by-sa/4.0/
[cc-by-sa-image]: https://licensebuttons.net/l/by-sa/4.0/88x31.png
[cc-by-sa-shield]: https://img.shields.io/badge/License-CC%20BY--SA%204.0-lightgrey.svg
