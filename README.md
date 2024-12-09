##README: Micro:bit IoT Project
#Overview
This project demonstrates a simple IoT application using two Micro:bit devices: one acting as a sender and the other as a receiver. The devices communicate using the Micro:bit's built-in radio functionality. Commands sent by the sender trigger specific actions on the receiver, such as toggling an LED, blinking another LED, or controlling a piezo buzzer with a potentiometer.

##Components Used
Micro:bit (2 units) - One for sending commands, the other for receiving and controlling components.
Kitronik Edge Connector Breakout Board - To interface the Micro:bit with external components.
External Components:
2 LEDs
330Ω Resistors (2 units)
Piezo Buzzer
Potentiometer
Wires:
Female-to-male wires for connections to the breakout board.
Male-to-male wires for breadboard connections.
##Functionality
Sender Micro:bit:

Toggles between sender and receiver mode using Button A.
Sends commands using buttons:
Button B: Toggles the first LED.
Buttons A+B: Blinks the second LED.
External Button: Sends a command for the buzzer to operate based on the potentiometer value.
Receiver Micro:bit:

Executes commands received via the radio:
CMD_TOGGLE_LED: Toggles the first LED (connected to P8).
CMD_BLINK_LED: Blinks the second LED (connected to P13).
CMD_BUZZER: Operates the buzzer based on the potentiometer value (potentiometer on P10, buzzer on P15).

