# FHTW_BIC_MCSD_Assign1 Description:
The purpose of this task is to become familar with microcontroller and how to program and configure it. This involves:

skim-reading the reference manual

becoming familiar with the board schematics

become familiar with the stm32l432xx.h header file

become familiar with the STM32 HAL library

The following tasks shall be implemented in two separate versions, once using a barebone apporoach and once using the STM32 HAL library. The functional description is valid for both task versions.

Functional Description
Write a function blinky() that allows to toggle one of the LEDs (LED_ABRG located on the Click Schield) with a given brightness. The LED as well as the brightness are to be specified as parameters, e.g. 10% brightness when switching on. Alternatively, you can also use a parameter to specify the on and off times of the LED, e.g. 10 ms off, 90 ms on.

Write a function buttoncheck() that allows to determine whether a button (use SW1 from the Click Shield) was pressed or not. The function shall be able to properly deal with bouncing behavior of the button.

Debouncing can be done in many ways. For example, you can use special input circuits on the switch. However, for us it is easier to perform debouncing in the software. Basically, you have to detect a change in value on the input pin (the switch has been pressed) and from that point you start counting. If the value does not change after e.g. 5 times of reading the switch, you can assume that the bounce phase is finished. There are many other software debouncing methods you can use. If you do a simple web search using the keyword "software debouncing", you are sure to find good articles on the subject.
Implement following behaviour in the main() loop:

Define three brightness levels of the LED and change them with each button press.

When the button is pressed for one second, turn off the LED.

For this use the functions blinky() and buttoncheck()

# Points:

5/10
