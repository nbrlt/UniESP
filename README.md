# UniESP
This is a simple board to control a telescope mount using OnStepX and unipolar Steppers. It relies on an ESP32 dev board with 30 pins and a RP2040 in the form of the Raspberry pico zero from waveshare as the driver logic. 

The code for OnStepX is found here: https://github.com/nbrlt/OnStepX (for now).
## The RP2040
The RP2040 is used to convert the StepDir interface of OnStepX to a 4 pin control for the DRV8932. I used that specific bridge driver to have a current control on the stepper (I could not find any StepDir bridge with proper current control).

The code for the Raspberry pico zero can be found here: [https://github.com/nbrlt/RP2040_Unipolar_StepDir_Driver](https://github.com/nbrlt/RP2040_StepDirToPWM_StepperLogic)
