# Anti-tilt System
An anti-tilt sensing system implemented using an accelerometer of FRDM-K64M board. The system is
intended for being embedded in the cargo bay of heavy-duty vehicles, and it serves to warn
about any odd distribution of the cargo.

*Requirements
1. Implemented the embedded system using the FRDM K64F board, where the
FXOS8700CQ is used as accelerometer, and the RGB LED is used as status indicator as
follows:
• In case of no warning, the GREEN LED is on and the others are off;
• In case of warning, the RED LED is on and the others are off;
• BLUE LED shall be turned on for the duration of the calibration phase, if needed.

The LED colors are updated every 100 msec, after an initial calibration phase (if
needed) that shall last no more than 1 minute;
2. The Simulink model organized in three units, one managing the acquisition of
the raw data from the accelerometer, one devoted to processing and output
computation, and one for the control of the LEDs;
3. A test harness used for functional testing of the unit devoted to
processing and output computation, which shall provide suitable test stimuli.
