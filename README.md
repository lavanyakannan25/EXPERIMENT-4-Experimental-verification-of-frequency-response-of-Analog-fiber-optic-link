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
Fiber optic links can be used for transmission of digital as well as analog signals. Basically a fiber optic link contains three main elements, a transmitter, an optical fiber and a receiver. The transmitter module takes the input signal in electrical form and then transforms it into optical (light) energy containing the same information. The optical fiber is the medium which takes the energy to the receiver. At the receiver light is converted back into electrical form with the same pattern as originally fed to the transmitter.

TRANSMITTER: Fiber Optic transmitters are typically composed of a buffer, driver and Optical Source. The buffer electronics provides both an electrical connection and isolation between the transmitter and the electrical system supplying the data. The driver electronics provides electrical power to the Optical source in a fashion that duplicates the pattern of data being fed to the transmitter. Finally the optical source (LED) converts the electrical current to light energy with the same pattern. The LED SFH450V (950nm) supplied with this kit operates outside the visible light spectrum. Its Optical output is centered at near infrared wavelength of 950nm. The LED SFH756V (660nm) supplied with this kit operates at the visible light spectrum. Its Optical output is centered at wavelength of 660nm.

RECEIVER: The function of the receiver is to convert the optical energy into electrical form, which is then conditioned to reproduce the transmitted electrical signal in it's original form. The detector SFH350V (Photo Transistor Detector) used in the kit has a transistor type output. The parameters usually considered in the case of detector are it's responsivity at peak wavelength and response time. SFH350V (Photo Transistor Detector) has responsivity of about 0.8mA/10uW at 660nm. But its response time is quite large and thus has lower bandwidth of about 300 KHz. When optical signal falls on the base of the transistor detector, proportional

current flows through its emitter generating the voltage across the resistance connected between emitter and ground. This voltage is the duplication of the transmitted electrical signal, which can be amplified.

---

## PROCEDURE
Refer to the block diagram & carry out the following connections and settings.

Connect the power supply with proper polarity to the kit link-B and switch it on.

Keep all Switch Faults in OFF position.

Keep switch SW8 towards TX position.

Keep switch SW9 towards TX1 position.

Keep Jumper JP5 towards +12V position.

Keep Jumpers JP6, JP9, JP10 shorted.

Keep Jumper JP8 towards sine position.

Keep Intensity control pot P2 towards minimum position.

Feed about 2Vpp sinusoidal signal of 1 KHz from the function generator to the IN post of Analog Buffer.

<img width="685" height="292" alt="image" src="https://github.com/user-attachments/assets/3771c564-f5f8-4f61-bc2b-3d8665520c2d" />

Connect the output post OUT of Analog Buffer to the post TX IN of Transmitter.

Slightly unscrew the cap of SFH756V (660nm). Do not remove the cap from the connector. Once the cap is loosened, insert the one meter fiber into the cap. Now tighten the cap by screwing it back.

Connect the other end of the Fiber to detector SFH350V (Photo Transistor Detector) very carefully.

Observe the detected signal at post ANALOG OUT on oscilloscope. Adjust Intensity control pot P2 Optical Power control potentiometer so that you receive signal of 2Vpp amplitude.

<img width="743" height="301" alt="image" src="https://github.com/user-attachments/assets/c215b43f-a810-4cc2-aae9-36757dd2ab9b" />

To measure the analog bandwidths of the phototransistor vary the input signal frequency and observe the detected signal at various frequencies.

Plot the detected signal against applied signal frequency and from the plot determine the 3dB down frequency.

Keep switch SW9 towards TX2 position.

Keep Jumper JP7 towards +12V position.

Remove fiber cable from SFH756V (660nm) and slightly unscrew the cap of SFH450V (950nm). Do not remove the cap from the connector. Once the cap is loosened, insert the one meter fiber into the cap. Now tighten the cap by screwing it back.

Observe the detected signal at post ANALOG OUT on oscilloscope.

<img width="721" height="292" alt="image" src="https://github.com/user-attachments/assets/3a2ded69-511b-4b1d-a76b-4cfc53a7806f" />
 

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
