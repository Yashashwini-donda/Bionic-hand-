# Bionic-hand

OVERVIEW

This project implements a responsive, functional prosthetic hand operated via EMG (electromyography) signals. EMG signals detected from the user's muscles enable intuitive gesture control, with movement decoded by an Arduino-based embedded system and actuated via lightweight mechanisms.

FEATURES 

3D-Printed Prosthetic Hand: Lightweight mechanical construction optimized for comfort and ease of control.

Gesture Control: Interprets EMG signals for intuitive hand movements and gestures.

Arduino-Based: Utilizes Arduino UNO as the main controller for signal processing and motor actuation.

Embedded Signal Processing: Custom techniques for EMG signal acquisition, filtering, and movement prediction.


HARDWARE REQUIREMENTS

Arduino UNO board

EMG sensor module (e.g., MyoWare or AD8226-based sensor)

3D-printed prosthetic hand assembly

Actuator-Shape memory alloy of 0.5mm (for finger and thumb movement)

Instrumentation Amplifier

Standard electrodes (for muscle signal collection)

External power supply or batteries (+Vs, -Vs) for sensors


SIGNAL PROCESSING 

Arduino code for EMG data acquisition and servo control.

Signal processing (rectification, smoothing, thresholding) implemented onboard Arduino.

Gesture mapping (open/close hand, thumbs up, etc.) triggered based on muscle activation patterns.


SETUP AND HARDWARE ASSEMBLY 

Print prosthetic hand components and assemble per mechanical guide.

Attach servo motors for fingers and thumb.

Connect electrodes to chosen muscle group (e.g., forearm).

Wire EMG sensor output to Arduino analog pin (recommended: A0/A1).

Power setup: Use two batteries to establish +Vs and -Vs for proper EMG sensor bias


ARDUINO CODE UPLOAD

Use provided Arduino sketch to read EMG analog signals.

EMG signal range typically maps to 0–1023 for Arduino analog input.

Code interprets muscle contraction to actuate servos for selected gestures.


CALIBRATION 

Place electrodes according to muscle anatomy for optimal signal acquisition (e.g., green on muscle belly, red on muscle end, yellow on nearby bone).

Use Arduino Serial Plotter to monitor signal and adjust thresholds for reliable gesture detection.
