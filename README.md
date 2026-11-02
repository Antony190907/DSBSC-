# DSBSC


# EX NO: 2	DSB-SC-AM MODULATOR AND DEMODULATOR

**AIM:**

To write a program to perform DSBSC modulation using SCI LAB and study its spectral characteristics.

**APPARATUS REQUIRED:**

•	Computer with i3 Processor
•	SCI LAB

**Note:** Keep all the switch faults in off position

**ALGORITHM:**

***1.	Define Parameters:***
•	Fs: Sampling frequency.
•	T: Duration of the signal.
•	Fc: Carrier frequency.
•	Fm: Frequency of the message signal.
•	Amplitude: Maximum amplitude of the message signal.

***2.	Generate Signals:***
•	Message Signal: A sinusoidal signal that will be modulated.
•	Carrier Signal: A high-frequency sinusoidal signal used for modulation.

***3.	DSBSC Modulation:***
•	Modulated Signal: Multiply the message signal by the carrier signal to produce the DSBSC signal.

***5.	Visualization:***
Plot the message signal, carrier signal, and DSBSC modulated signal.

**PROCEDURE:**

•	Refer Algorithms and write code for the experiment.

•	Open SCILAB in System

•	Type your code in New Editor

•	Save the file
 
•	Execute the code

•	If any Error, correct it in code and execute again

•	Verify the generated waveform using Tabulation and Model Waveform

**MODEL WAVEFORM:**

<img width="703" height="679" alt="image" src="https://github.com/user-attachments/assets/e7c7c7f8-ccf2-41ac-b1f3-325989941a6f" />

**PROGRAM:**
~~~
fm=304;
Am=2.45;
fc=10*fm;
Ac=1.8*Am;
fs=10*fc;
t=0:1/fs:2/fm;
em=Am*cos(2*3.14*fm*t);
ec=Ac*cos(2*3.14*fc*t);
eAM1=(Ac+em).*cos(2*3.14*fc*t);
eAM2=(Ac-em).*cos(2*3.14*fc*t);
eDSBSC=eAM1-eAM2;
subplot(3,1,1);
plot(t,em);
subplot(3,1,2);
plot(t,ec);
subplot(3,1,3);
plot(t,eDSBSC);
~~~

**OUTPUT GRAPH:**

<img width="1097" height="622" alt="Exp2 output" src="https://github.com/user-attachments/assets/aa611e0b-bbca-4c48-a2d3-49d10e758005" />



**TABULAR COLUMN:**

<img width="3359" height="2060" alt="IMG_20261102_191833_edit_140314561568693 jpg" src="https://github.com/user-attachments/assets/9087e33b-bf7f-4536-8330-aad0bbd89d2e" />


**RESULT:**

Thus the DSB-SC-AM Modulation is generated.

