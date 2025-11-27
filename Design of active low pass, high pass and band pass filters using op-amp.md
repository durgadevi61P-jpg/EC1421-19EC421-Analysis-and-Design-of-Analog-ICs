# EC1421-19EC421-Analysis-and-Design-of-Analog-ICs
# DESIGN OF ACTIVE LOW PASS,HIGH PASS AND BAND PASS FILTERS USING OP-AMP 

## AIM: 

To design and obtain the frequency response of 
i) First order Low Pass Filter (LPF) 
ii) First order High Pass Filter (HPF) 
iii) Band pass filter
 
## APPARATUS REQUIRED

<img width="625" height="170" alt="image" src="https://github.com/user-attachments/assets/900fc8b3-3a8c-4208-bf52-98cc9e281e21" />

## THEORY
## LOW PASS FILTER 
 A LPF allows frequencies from 0 to higher cut of frequency, fH.  At fH the gain is 0.707 
Amax, and after fH gain decreases at a constant rate with an increase in frequency.  The gain 
decreases 20dB each time the frequency is increased by 10.  Hence the rate at which the gain 
rolls off after fH is 20dB/decade or 6 dB/ octave, where octave signifies a two fold increase in 
frequency.  The frequency f=fH is called the cut off frequency because the gain of the filter at this 
frequency is down by 3 dB from 0 Hz.  Other equivalent terms for cut-off frequency are -3dB 
frequency, break frequency, or corner frequency.
# HIGH PASS FILTER 
The frequency at which the magnitude of the gain is 0.707 times the maximum value of 
gain is called low cut off frequency.  Obviously, all frequencies higher than fL are pass band 
frequencies with the highest frequency determined by the closed –loop band width all of the op
amp. 
# BAND PASS FILTER 
A band pass filter has a pass band between two cutoff frequencies fH and fL such that fH > 
fL.  Any input frequency outside this pass band is attenuated.  There are two types of band-pass 
filters.  Wide band pass and Narrow band pass filters.  We can define a filter as wide band pass if 
its quality factor Q <10.  If Q>10, then we call the filter a narrow band pass filter.  A wide band 
pass filter can be formed by simply cascading high-pass and low-pass sections.  The order of 
band pass filter depends on the order of high pass and low pass sections.

## CIRCUIT DIAGRAM: 
## LOW_PASS
![WhatsApp Image 2025-11-27 at 23 51 20_188e7799](https://github.com/user-attachments/assets/d6492f6b-15d5-49ba-aed7-736a5e626e17)
## HIGH-PASS
![WhatsApp Image 2025-11-27 at 23 51 21_ccc150e8](https://github.com/user-attachments/assets/7c63fc02-93c8-467a-a5d6-1f2adc988b28)
## BAND-PASS
![WhatsApp Image 2025-11-27 at 23 51 19_14440e79](https://github.com/user-attachments/assets/95fbbefd-78de-4de9-95ae-a4797c478c2f)


## MODEL GRAPH:
## LOW_PASS
![WhatsApp Image 2025-11-27 at 23 50 19_30bdf02f](https://github.com/user-attachments/assets/49f347da-10ff-45bf-a7a0-16c63cb6f3b2)
## HIGH-PASS
![WhatsApp Image 2025-11-27 at 23 50 20_3fb32aa8](https://github.com/user-attachments/assets/81cb432f-6e76-484d-8649-585301278cf9)
## BAND-PASS
![WhatsApp Image 2025-11-27 at 23 51 20_05d2549f](https://github.com/user-attachments/assets/f4fb22ba-87fa-4a0d-8aa0-de4bf4dbb7b6)


## PROCEDURE - (LPF & HPF): 
1. Connect the circuit as shown in the circuit diagram. 
2. Select the corresponding cut-off frequency (higher or lower) and determine the value of C&R. 
select the value of R1 & Rf depending on desired passband gain Af.. 
3. Apply a constant voltage input sinusoidal signal to the non-inverting terminal of op-amp. 
4. Tabulate the output voltage Vo with respect to different values of input frequency. 
5. Calculate passband gain and plot the graph of frequency versus voltage gain & check the 
graph to  get approximately the same characteristic as shown in the model graph. 
# PROCEDURE:BAND PASS FILTER 
1. Select the lower and higher cut-off frequency and calculate the value of R & C for the given 
frequencies. 
2. Design for LPF & HPF separately and then combine the circuit by first placing the HPF 
followed by a LPF (i.e) HPF in series with LPF. 
3. Connect the circuit as shown in the circuit diagram. 
4. Apply a constant voltage input sinusoidal signal to the non-inverting terminal of op-amp. 
5. Tabulate the output voltage Vo with respect to different values of input frequency. 
6. Calculate passband gain and plot the graph of frequency versus voltage gain & check the 
graph to get approximately the same characteristic as shown in the model graph

## DESIGN:LPF & HPF:

<img width="429" height="324" alt="image" src="https://github.com/user-attachments/assets/b0f0ac0a-3006-494c-9096-e91ae2d6e87c" />

# DESIGN: BAND PASS FILTER
Design a BPF to pass a band of 400Hz to 2KHz with a pass band gain of 4.  
1. Select the highest cut-off frequency of LPF as fH = 10 KHz and the lowest cut-off frequency 
of HPF as fL = 1 KHz.  
2. Design the HPF first by taking fL = 1KHz. Assume the value of C < 1μf.  
Let C = 0.1μf.  
3. Calculate R from the expression.  
Given: fH = 2KHz  = 1/ (2πR1C1) 
   Let C1 = 0.1 µF, R1 = 7.9 KΩ 
Given: fL = 400Hz  = 1/ (2πR2C2) 
   Let C2 = 0.1 µF, R2 = 39.8 KΩ 
  Pass band Gain=4 
   Now   Ao = 1 + (Rf / R1)  
               2-1=(Rf / Ri) 
                Ri = Rf 
                 Let  Ri = Rf = 10 KΩ
## TABULATION:
## LOW_PASS
![WhatsApp Image 2025-11-27 at 23 51 21_d7b72506](https://github.com/user-attachments/assets/16dcac94-8136-4a0a-9b03-51eafaa82975)
## HIGH-PASS
![WhatsApp Image 2025-11-27 at 23 51 21_a5b58d22](https://github.com/user-attachments/assets/6d1b9987-7f96-4ca3-8b13-da784f920c73)
## BAND-PASS
![WhatsApp Image 2025-11-27 at 23 50 35_36620767](https://github.com/user-attachments/assets/f91c5cd6-ca6e-48fc-bcc3-ea6fcd0f6f4a)

## GRAPH:
## LOW_PASS
![WhatsApp Image 2025-11-27 at 23 51 20_239ffaa3](https://github.com/user-attachments/assets/e7049f5f-96f5-4ebf-ae59-1f988f204aaf)
## HIGH-PASS
![WhatsApp Image 2025-11-27 at 23 51 22_ce379c47](https://github.com/user-attachments/assets/365ea86b-2bac-487b-9ff5-eed01b9e7ff7)
## BAND-PASS
![WhatsApp Image 2025-11-27 at 23 51 22_b447d0b7](https://github.com/user-attachments/assets/975ca42a-1db0-49ec-a5de-362435f2ab25)

 ## RESULTS:
Thus an Active Low pass, High pass and Band Pass Filters are designed and 
tested using op-amp IC 741. 

