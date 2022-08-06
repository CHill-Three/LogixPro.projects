## CHill-Three's github.io LogixPro 500 PLC Sim (RSLogix 500 Emulator) Page
Welcome to my LogixPro 500 PLC Sim (RSLogix 500 Emulator) repository created on August 6, 2022. LogixPro 500 PLC Sim is an educational resource focusing on learning the essentials of RSLogix ladder logic programming. LogixPro 500 PLC Sim heavily emulates Allen Bradley's RSLogix 500 program. Thank you for your time!
<!-- Table of Contents (TITLES) -->

## My Main Projects (Section One: LogixPro 500 PLC Sim Starter Projects)
<!-- DIVIDER ---------------------------------------------------------------------------------------------------------------------------------------------------------->
## Project 1: Simple I/O with XIC and XIO gates

![XIC_XIOButtons](https://raw.githubusercontent.com/CHill-Three/logixpro.projects/main/Project%201%3A%20Simple%20I-O%20with%20XIC%20and%20XIO%20gates/XIC_XIOButtons.PNG?raw=true "XIC_XIOButtons")

#### Description: 
Using XIC instruction, the instruction is only activated when the memory location is one. So, when the push button is not pressed, the logic state is zero, the instruction is false, and the light will not turn on. When the push button is pressed, meaning the logic state now is true, equals one, then the instructions are highlighted, and the light will turn on according to the continuity. XIC, Examine If Close instruction is true when the logic state equals 1. Now, with the Examine If Open instruction: XIO instruction acts the opposite way. It is activated when the logic state is zero and not when the logic state is one. When the push button is not pressed, the logic state is 0, and since we are using XIO instruction, it's activated, and the light will be on. When the push button is pressed, the logic state is one, true, meaning the XIO instruction is false and is not highlighted, and the light will not turn on. XIO is true when its logic state equals 0. This means that the tag assigned to the XIO instruction is active. 
