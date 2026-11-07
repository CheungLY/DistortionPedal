# DistortionPedal
A pedal that uses diode clipping to generate light distortion in a circuit.

To do this I followed this guide: https://curiousmotor.com/2019/12/07/distortion-pedal-electronics-explained/ and added a few modifications.

This is the what the schematic looks like which can be divided into 3 sections:
<img width="792" height="587" alt="image" src="https://github.com/user-attachments/assets/ee2efb56-259c-4ec0-9009-6ba92c90b63f" />

On the left is the input section:
This is just the part where the signal (in the form of an alternating current enters)

The middle section is the amplicification stage:
This part sends the signal through a transistor which amplifies it and leads it go to out, the output jack

The top section is clipping or fxIn and fxOut:
The diodes clip the amplitude to about 0.7v which is then amplified in the system.

This is the look of the PCB
<img width="438" height="517" alt="Screenshot 2026-11-07 180230" src="https://github.com/user-attachments/assets/006ad564-e1be-451f-8e42-cb912d2fe72f" />

And this is the 3D model:
<img width="945" height="736" alt="image" src="https://github.com/user-attachments/assets/0a276743-952b-42cd-8ad2-becd7eb6c962" />

The Gerber is attached in the Distortion pedal.zip and schematic with PCB as well.

The only specifically unique component is the 3PDT STOMP SWITCH, Kicad inherintly does not have this switch so you may need to design one yourself using the different symbols for SPDT switches. This is a specific switch used in most pedals
