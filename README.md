3. ##**EX.NO:
** 3  EXPERIMENTAL VERIFICATION OF INTEGRATOR AND DIFFERENTIATOR USING OP-AMP 
            
**DATE:** 09/09/2025 
             3A INTEGRATOR
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
| 6 | Resistors | 15k 1.5k  | 2 |
| 7 | capacitors | 0.1µF| 1 |
| 8 | Connecting wires and probes | As required | — |

---

## THEORY
INTEGRATOR
A circuit in which the output voltage waveform is the integral of the input voltage waveform is the integrator. Such a circuit is obtained by using a basic inverting amplifier configuration if the feedback resistor Rf is replaced by a capacitor Cf . The expression for the output voltage is given as,
Vo = - (1/Rf C1 ) ∫ Vi dt

Here the negative sign indicates that the output voltage is 180 0 out of phase with the input signal. Normally between fa and fb the circuit acts as an integrator. Generally, the value of fa < fb . The input signal will be integrated properly if the Time period T of the signal is larger than or equal to Rf Cf . That is,
T ≥ Rf Cf

The integrator is most commonly used in analog computers and ADC and signal-wave shaping circuits.
CIRCUIT DIAGRAM
## CIRCUIT DIAGRAM

![WhatsApp Image 2025-11-26 at 21 05 19_8d59d7fe](https://github.com/user-attachments/assets/8e821771-9bd8-4f95-b294-3968d6467689)

## MODEL GRAPH
<img width="556" height="380" alt="image" src="https://github.com/user-attachments/assets/caa7461c-69f7-4636-8e31-eea6db6efbb5" />

<img width="847" height="553" alt="image" src="https://github.com/user-attachments/assets/d8d3e586-8e58-47ba-baae-2794c7955d51" />

---

## DESIGN

To obtain the output of an Integrator circuit with component values R1Cf = 0.1ms , Rf = 10 R1 and Cf = 0.01 µF and also if 1 V peak square wave at 1000Hz is applied as input.
We know the frequency at which the gain is 0 dB, fb = 1 / (2π R1 Cf) Therefore fb = 	 Since fb = 10 fa , and also the gain limiting frequency fa = 1 / (2π Rf Cf)
We get , R1 =	and hence Rf = 	

![WhatsApp Image 2025-11-26 at 21 02 06_a7b95560](https://github.com/user-attachments/assets/69656228-ad33-41f4-a73a-8506f49cb7d7)


## PROCEDURE

1.	Connections are given as per the circuit diagram
2. + Vcc and - Vcc supply is given to the power supply terminal of the Op-Amp IC.
3.	By adjusting the amplitude and frequency knobs of the function generator, appropriate input voltage is applied to the inverting input terminal of the Op- Amp.
4.	The output voltage is obtained in the CRO and the input and output voltage waveforms are plotted in a graph sheet.


## TABULATION                              
		
![WhatsApp Image 2025-11-26 at 21 02 41_7ebca6b5](https://github.com/user-attachments/assets/214a1aab-e2f9-4b9e-9884-f8e05d847606)

---

## OUT PUT WAVEFORM AND DISCUSSION 
![WhatsApp Image 2025-11-26 at 21 02 22_f4b07e0a](https://github.com/user-attachments/assets/21e7fb78-1a4e-4f08-bdad-cf9310163f50)

![WhatsApp Image 2025-11-26 at 21 02 55_1ace6dc7](https://github.com/user-attachments/assets/011be2af-2c2f-4d32-876c-3937b96f3f51)

---
**DATE:** 16/09/2025 
             3 B DIFFERENTIATOR
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
| 6 | Resistors | 15k  1.5k | 2 |
| 7 | capacitors | 0.001µF,0.01µF | 1 |
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

![WhatsApp Image 2025-11-26 at 21 03 11_d312573c](https://github.com/user-attachments/assets/972f565c-e993-4293-926c-68904f0cd6d5)


## MODEL GRAPH

(i)	 SINE WAVE INPUT

<img width="687" height="479" alt="image" src="https://github.com/user-attachments/assets/c89226c0-c2bb-4544-b355-27fc0d923f1a" />
---

AND

(ii) SQUARE WAVE INPUT

<img width="758" height="447" alt="image" src="https://github.com/user-attachments/assets/cda33b00-c40c-490f-a9bd-e06107119c25" />


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

![WhatsApp Image 2025-11-26 at 21 03 25_45f7af4e](https://github.com/user-attachments/assets/74086b84-1880-42e7-85da-f289436ba87f)

## PROCEDURE

1.	Connections are given as per the circuit diagram
2. + Vcc and - Vcc supply is given to the power supply terminal of the Op-Amp IC.
3.	By adjusting the amplitude and frequency knobs of the function generator, appropriate input voltage is applied to the inverting input terminal of the Op- Amp.
4.	The output voltage is obtained in the CRO and the input and output voltage waveforms are plotted in a graph sheet.

 ## TABULATION
 
 ![WhatsApp Image 2025-11-26 at 21 03 53_db2099fd](https://github.com/user-attachments/assets/3d4f33fd-7070-401d-b3ab-6a63ff94adb6)

		

## OUT PUT WAVEFORM AND DISCUSSION 

![WhatsApp Image 2025-11-26 at 21 03 41_31d73b48](https://github.com/user-attachments/assets/a2e99cef-b41b-4fd1-b63e-404133463c95)

![WhatsApp Image 2025-11-26 at 21 02 55_f6fcf74f](https://github.com/user-attachments/assets/c9ba456d-4788-4fe5-958a-0678aa166103)

---

RESULT:
Thus an Integrator and Differentiator using op-amp are designed and their performance was successfully tested using op-amp IC 741.
---



