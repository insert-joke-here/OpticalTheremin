# OpticalTheremin

<img width="697" height="344" alt="entry3pic5" src="https://github.com/user-attachments/assets/9291467f-63e6-420f-8e03-c765c20f30a3" />

This is an optical theremin using the esp-32 based microcontroller LILYGO T7-S3. A theremin is an instrument where it is not touched while playing, instead sensing the position of the player's hand in the air. A normal theremin uses electromagnetic fields and capacitance to detect the player's hand, while this theremin instead uses a distance sensor to detect the position. While this provides much less sensitivity, it is more straightforward to implement and relatively software dependent. The sensor used here is an Adafruit VL6180X. An optical sensor is used over the more typical ultrasound detectors because of the better precision that the optical sensor provides, and its tighter cone, to protect it from undesired interference. 

It uses three sliders, one for the volume, one for the sensitivity (which determines the pitch), and one for the vibrato, which makes the instrument sound less dry. This vibrato is done by using a sine wave that centers around the desired pitch, whose amplitude is defined by the slider. 

Since this theremin uses an actual speaker over a buzzer, it requires an amplifier, which here is the Adafruit MAX98357 breakout board.



Schematic:

<img width="600" height="517" alt="entry3pic6" src="https://github.com/user-attachments/assets/af3b8d44-c730-4a26-a0e6-90e3b6f2ffec" />

