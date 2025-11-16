# Exp 4 Experimental verification of frequency response of Analog fiber optic link
# Fiber Optic Link Analysis (660nm)

## AIM
To analyze the relationship between input and received signal of a 660nm fiber optic cable using analog and digital link.

---

## EQUIPMENTS REQUIRED
- Fiber optic trainer kit ST 2502  
- Power supply  
- Patch cords  
- CRO (Cathode Ray Oscilloscope)  
- 660 nm fiber cable  

---

## THEORY

Fiber optic links can be used for transmission of digital as well as analog signals. A fiber optic link typically consists of three main elements:
- **Transmitter**: Converts the electrical input signal into optical (light) energy.
- **Optical Fiber**: Serves as the transmission medium for the light signal.
- **Receiver**: Converts the received light back into an electrical signal, preserving the original signal pattern.

---

## PROCEDURE

1. Connect the power supply to the board.  
2. Ensure that all switched faults are set to ‘Off’.  
3. Make the following connections (as shown in Figure 19):  
   a. Connect the 1KHz sine wave output to emitter 1's input.  
   b. Connect the fiber optic cable between emitter output and detector input.  
   c. Connect detector 1's output to AC amplifier 1 input.  
4. On the board, switch emitter 1's driver to analog mode.  
5. Switch on the power.  
6. Observe the input to emitter 1 (TP5) and the output from AC amplifier 1 (TP28). Verify that both signals are identical.  
7. Vary the frequency between 10 Hz to 1 MHz and observe the output voltage for a constant input voltage of 5V.  
8. Calculate the bandwidth by determining the gain in decibels (dB).  

---

## BLOCK DIAGRAM

<img width="725" height="424" alt="image" src="https://github.com/user-attachments/assets/96ac1444-b7bf-4361-acfd-9462a9e47767" />

---


## TABULATION  
**Transmission through Analog Link**

| Frequency (Hz) | Output Signal Amplitude (Vo) | Gain = Vo/Vi | Gain in dB |
|----------------|------------------------------|--------------|------------|
|  800Hz         | 120mv                        |  0.024       |  -32.395   |
|  1.5Hz         | 216mv                        |0.0432        | -27.290    |
|3KHz            |	412mV                      |	0.0824	   |  -21.681   |
|   5KHz	        |670mV                        	|0.134	      |-17.457     |
|7KHz	           |924mV	                        |0.1848	      |-14.665     |
|9KHz            |950mv                         |	0.19	      |-14.424     |
|11KHz	        |950mV	                        |0.19          |	-14.424   |
|13KHz	        |950mV                         |	0.19	      |-14.424     |
|15KHz           |950mV	                        |0.19	         |-14.424     |
|50KHz	        |840mV	                        |0.168         |	-15.493   |
|200KHz	        |385mV                         |	0.077	      |-22.270      |
|600KHz	        |280mV                         |	0.056	      |-25.036      |
|800KHz	        |95mV	                        |0.019	       |-34.424      |
|1MHz            |	58mV	                      |0.011	       |-39.172      |
---

## MODEL GRAPH

<img width="837" height="367" alt="image" src="https://github.com/user-attachments/assets/1d3665ac-f0e1-4471-9db2-c6c9c731e5b1" />

---
## GRAPH
<img width="1500" height="1228" alt="image" src="https://github.com/user-attachments/assets/f76d5175-e45f-40bb-99ab-08f43f536b7b" />


## RESULT
Thus, the frequency response of the analog fiber optic link was successfully studied, and the bandwidth was determined to be 75 kHz.
