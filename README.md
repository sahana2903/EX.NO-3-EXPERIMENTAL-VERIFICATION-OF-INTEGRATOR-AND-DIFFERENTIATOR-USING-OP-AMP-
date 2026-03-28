## EX.NO: 3  EXPERIMENTAL VERIFICATION OF INTEGRATOR AND DIFFERENTIATOR USING OP-AMP 
            
## DATE:31.1.2026

## 3A INTEGRATOR

## AIM
To design and test the performance of integrator and differentiator circuits using Op-amp

---

## APPARATUS REQUIRED

| S.No | Name of the Apparatus | Range | Quantity |
|------|------------------------|--------|-----------|
| 1 | Function Generator | 3 MHz | 1 |
| 2 | DSO | 30 MHz | 1 |
| 3 | Dual RPS | (0 – 30) V | 1 |
| 4 | Op-Amp | µA741 | 1 |
| 5 | Bread Board | — | 1 |
| 6 | Resistors | 1K,10K,100K  | 2 |
| 7 | capacitors | 0.1µF,0.01µF | 1 |
| 8 | Connecting wires and probes | As required | — |

---

## THEORY
INTEGRATOR
A circuit in which the output voltage waveform is the integral of the input voltage waveform is the integrator. Such a circuit is obtained by using a basic inverting amplifier configuration if the feedback resistor Rf is replaced by a capacitor Cf . The expression for the output voltage is given as,
Vo = - (1/Rf C1 ) ∫ Vi dt

Here the negative sign indicates that the output voltage is 180 0 out of phase with the input signal. Normally between fa and fb the circuit acts as an integrator. Generally, the value of fa < fb . The input signal will be integrated properly if the Time period T of the signal is larger than or equal to Rf Cf . That is,
T ≥ Rf Cf

The integrator is most commonly used in analog computers and ADC and signal-wave shaping circuits.
 
## CIRCUIT DIAGRAM

 ![WhatsApp Image 2026-03-27 at 8 45 48 PM](https://github.com/user-attachments/assets/82757c00-a408-446e-8f84-95c188834768)


## MODEL GRAPH

![WhatsApp Image 2026-03-27 at 8 46 44 PM](https://github.com/user-attachments/assets/c6f4c050-6e60-47bf-b84e-32655f73ced9)

## DESIGN

To obtain the output of an Integrator circuit with component values R1Cf = 0.1ms , Rf = 10 R1 and Cf = 0.01 µF and also if 1 V peak square wave at 1000Hz is applied as input.
We know the frequency at which the gain is 0 dB, fb = 1 / (2π R1 Cf) Therefore fb = 	 Since fb = 10 fa , and also the gain limiting frequency fa = 1 / (2π Rf Cf)


## PROCEDURE

1.	Connections are given as per the circuit diagram
2. + Vcc and - Vcc supply is given to the power supply terminal of the Op-Amp IC.
3.	By adjusting the amplitude and frequency knobs of the function generator, appropriate input voltage is applied to the inverting input terminal of the Op- Amp.
4.	The output voltage is obtained in the CRO and the input and output voltage waveforms are plotted in a graph sheet.

![WhatsApp Image 2026-03-27 at 10 18 37 PM](https://github.com/user-attachments/assets/0d03b32b-ae4c-490c-ba50-55efe0b9bd9e)

## TABULATION

![WhatsApp Image 2026-03-27 at 8 50 46 PM](https://github.com/user-attachments/assets/69208ec7-0309-400a-a5e5-005cbd730dd0)

---
## CALCULATION

![WhatsApp Image 2026-03-27 at 8 47 23 PM](https://github.com/user-attachments/assets/4d9f33bc-2bee-4187-a4f3-518ccef5e357)

## OUT PUT WAVEFORM AND DISCUSSION 

![WhatsApp Image 2026-03-27 at 8 49 51 PM](https://github.com/user-attachments/assets/7cefd11d-63b1-463d-af5d-5526a92a954d)

---
## DATE:7.2.2026
## 3B DIFFERENTIATOR
---

## AIM
To design and test the performance of integrator and differentiator circuits using Op-amp

---

## APPARATUS REQUIRED

| S.No | Name of the Apparatus | Range | Quantity |
|------|------------------------|--------|-----------|
| 1 | Function Generator | 3 MHz | 1 |
| 2 | DSO | 30 MHz | 1 |
| 3 | Dual RPS | (0 – 30) V | 1 |
| 4 | Op-Amp | µA741 | 1 |
| 5 | Bread Board | — | 1 |
| 6 | Resistors | 1K,10K,100K  | 2 |
| 7 | capacitors | 0.1µF,0.01µF | 1 |
| 8 | Connecting wires and probes | As required | — |

---

## THEORY
DIFFEERENTIATOR:
The differentiator circuit performs the mathematical operation of differentiation; that is, the output waveform is the derivative of the input waveform. The differentiator may be constructed from a basic inverting amplifier if an input resistor R1 is replaced by a capacitor C1 . The expression for the output voltage is given as,
Vo = - Rf C1 ( dVi /dt )

Here the negative sign indicates that the output voltage is 180 0 out of phase with the input signal. A resistor Rcomp = Rf is normally connected to the non-inverting input terminal of the op-amp to compensate for the input bias current. A workable differentiator can be designed by implementing the following steps:
1.	Select fa equal to the highest frequency of the input signal to be differentiated. Then, assuming a value of C1 < 1 µF, calculate the value of Rf.
2.	Choose fb = 20 fa and calculate the values of R1 and Cf so that R1C1 = Rf Cf.

The differentiator is most commonly used in wave shaping circuits to detect high frequency components in an input signal and also as a rate–of–change detector in FM modulators.

## CIRCUIT DIAGRAM

![WhatsApp Image 2026-03-27 at 8 25 27 PM](https://github.com/user-attachments/assets/975b85f2-2e75-4d1e-b841-b505d1089bdc)


## MODEL GRAPH

(i)	 SINE WAVE INPUT
 
 ![WhatsApp Image 2026-03-27 at 8 26 13 PM](https://github.com/user-attachments/assets/48e1212e-e8db-4c75-a544-49a18763d542)


(ii) SQUARE WAVE INPUT

![WhatsApp Image 2026-03-27 at 8 27 47 PM](https://github.com/user-attachments/assets/ec881bcf-afa5-470f-95f8-31506c9bdd70)


---

## DESIGN

Design an op-amp differentiator that will differentiate an input signal with fmax = 100HZ Select fa = fmax = 100 HZ = 1 / 2πRFC1
Let C1 = 0.1μF
Then RF = 1 / 2π(102)(10-7)
= 15.9KΩ
Now choose fb = 10fa = 1 / 2πR1C1 Therefore, R1 = 1 / 2π(103)(10-7)
= 1.59KΩ Since RFCF = R1C1
We get, CF = (1.59*103*10-7) / 15.9*103
= 0.01μF
![WhatsApp Image 2026-03-27 at 10 21 19 PM](https://github.com/user-attachments/assets/e95040f7-cf3d-4ac3-ad57-1ddfbac6af20)

![WhatsApp Image 2026-03-27 at 10 25 09 PM](https://github.com/user-attachments/assets/c11086cc-07e3-4de1-aeef-eddf2e058908)

## PROCEDURE

1.	Connections are given as per the circuit diagram
2. + Vcc and - Vcc supply is given to the power supply terminal of the Op-Amp IC.
3.	By adjusting the amplitude and frequency knobs of the function generator, appropriate input voltage is applied to the inverting input terminal of the Op- Amp.
4.	The output voltage is obtained in the CRO and the input and output voltage waveforms are plotted in a graph sheet.

## TABULATION
![WhatsApp Image 2026-03-27 at 8 29 53 PM](https://github.com/user-attachments/assets/882d23d1-1b61-4c84-99bf-251ba82defd7)

## CALCULATION
![WhatsApp Image 2026-03-27 at 8 51 38 PM](https://github.com/user-attachments/assets/9de93e36-c5e7-40ac-85bd-331bce6b2957)

## OUT PUT WAVEFORM AND DISCUSSION 
![WhatsApp Image 2026-03-27 at 8 31 38 PM](https://github.com/user-attachments/assets/d78da06f-1703-4e29-9c75-85ddc9139d49)
![WhatsApp Image 2026-03-27 at 8 52 03 PM](https://github.com/user-attachments/assets/f58b68c8-fa98-4422-be52-fff7777383e7)
 
 ## RESULT:
Thus an Integrator and Differentiator using op-amp are designed and their performance was successfully tested using op-amp IC 741.
 



