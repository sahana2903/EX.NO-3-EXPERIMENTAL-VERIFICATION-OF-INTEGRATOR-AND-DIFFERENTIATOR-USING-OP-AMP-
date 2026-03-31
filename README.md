## EX.NO: 3  EXPERIMENTAL VERIFICATION OF INTEGRATOR AND DIFFERENTIATOR USING OP-AMP 

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

 ![WhatsApp Image 2026-03-31 at 8 40 22 AM](https://github.com/user-attachments/assets/d90445e4-4763-4235-8256-a1189833d680)



## MODEL GRAPH

![WhatsApp Image 2026-03-31 at 8 40 22 AM](https://github.com/user-attachments/assets/3f610a8b-666d-43f3-af59-0c5883a3d8ca)

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

<img width="988" height="1600" alt="image" src="https://github.com/user-attachments/assets/8e310531-3a05-4a54-a539-2ddb7a13d7dc" />


---
## CALCULATION

<img width="988" height="1600" alt="image" src="https://github.com/user-attachments/assets/d0dda6ea-e0d1-417b-8210-67419a9aa1e8" />


## OUT PUT WAVEFORM AND DISCUSSION 

<img width="1600" height="996" alt="image" src="https://github.com/user-attachments/assets/74f90f3e-66ab-414b-8177-25a83690eaa5" />


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


<img width="1600" height="887" alt="image" src="https://github.com/user-attachments/assets/21ab49ef-3ebf-4280-b676-47d25cce9bae" />

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

## PROCEDURE

1.	Connections are given as per the circuit diagram
2. + Vcc and - Vcc supply is given to the power supply terminal of the Op-Amp IC.
3.	By adjusting the amplitude and frequency knobs of the function generator, appropriate input voltage is applied to the inverting input terminal of the Op- Amp.
4.	The output voltage is obtained in the CRO and the input and output voltage waveforms are plotted in a graph sheet.

## TABULATION
<img width="1600" height="887" alt="image" src="https://github.com/user-attachments/assets/47d54860-1ea6-4833-87c6-c4d3fcd4a3a3" />

## CALCULATION
<img width="1600" height="887" alt="image" src="https://github.com/user-attachments/assets/dd7f051b-917a-4502-b8da-94ab2e8207a4" />


## OUT PUT WAVEFORM AND DISCUSSION 
<img width="1600" height="1206" alt="image" src="https://github.com/user-attachments/assets/71dd0b7b-58ff-4ec4-b5c7-fd037c20ae73" />
<img width="1432" height="1089" alt="image" src="https://github.com/user-attachments/assets/67eacee3-a681-4a18-8b81-027f4c8ffaca" />


 ## RESULT:
Thus an Integrator and Differentiator using op-amp are designed and their performance was successfully tested using op-amp IC 741.
 



