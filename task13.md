# Experiment: 555 Astable Multivibrator (Duty Cycle ≈ 60%)

## Aim
To design and build a 555 astable multivibrator with a duty cycle of about 60% and observe the output waveform using a Digital Storage Oscilloscope (DSO).

## Components Used
- IC 555 timer  
- Resistors (R1, R2)  
- Capacitor (C)  
- Breadboard  
- Connecting wires  
- Power supply  
- DSO (Digital Storage Oscilloscope)

## Theory
A 555 timer in astable mode produces a continuous square wave.  
The duty cycle is given by:

D = (R1 + R2) / (R1 + 2R2)

By selecting suitable values of R1 and R2, I can get a duty cycle close to 60%.  
If R1 = R2, the duty cycle becomes about 66% (which is not needed) so me went with described ratio of 1:2.

## Procedure
1. I calculated suitable values of R1 and R2 for ~60% duty cycle.  
2. I connected the 555 timer circuit on the breadboard.  
3. I provided power supply to the circuit.  
4. I connected the output pin to the DSO using probes.  
5. I observed and measured the waveform on the DSO.

## Observation
- A square wave output was observed on the DSO.  
- The ON time was slightly more than the OFF time.  
- The measured duty cycle was approximately 60% (if precise, then it was around 59.4 ig).

## Result
I successfully designed and implemented a 555 astable multivibrator with a duty cycle close to 60% and verified the output using a DSO. (I did face a problem of getting result duty cycle of 47%, which was diagnosed by my friend and mistake was using 1000microF capacitor which was more than required amount).

## Conclusion
The experiment was successful. I learned how to design an astable multivibrator and verify its output waveform practically.

https://github.com/user-attachments/assets/1e5c80d6-f2c0-4ba3-84af-d9b5671404fe
