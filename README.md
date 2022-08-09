## CHill-Three's github.io LogixPro 500 PLC Sim (RSLogix 500 Emulator) Page
Welcome to my LogixPro 500 PLC Sim (RSLogix 500 Emulator) repository created on August 6, 2022. LogixPro 500 PLC Sim is an educational resource focusing on learning the essentials of RSLogix ladder logic programming. LogixPro 500 PLC Sim heavily emulates Allen Bradley's RSLogix 500 program. Thank you for your time!
<!-- Table of Contents (TITLES) -->

## My Main Projects (Section One: LogixPro 500 PLC Sim Starter Projects)
<!-- DIVIDER ---------------------------------------------------------------------------------------------------------------------------------------------------------->
## Project 1: Simple I/O with XIC and XIO gates

![XIC_XIOButtons](https://raw.githubusercontent.com/CHill-Three/logixpro.projects/main/Project%201%3A%20Simple%20I-O%20with%20XIC%20and%20XIO%20gates/XIC_XIOButtons.PNG?raw=true "XIC_XIOButtons")

#### Description: 
Using XIC instruction, the instruction is only activated when the memory location is one. So, when the push button is not pressed, the logic state is zero, the instruction is false, and the light will not turn on. When the push button is pressed, meaning the logic state now is true, equals one, then the instructions are highlighted, and the light will turn on according to the continuity. XIC, Examine If Close instruction is true when the logic state equals 1. Now, with the Examine If Open instruction: XIO instruction acts the opposite way. It is activated when the logic state is zero and not when the logic state is one. When the push button is not pressed, the logic state is 0, and since we are using XIO instruction, it's activated, and the light will be on. When the push button is pressed, the logic state is one, true, meaning the XIO instruction is false and is not highlighted, and the light will not turn on. XIO is true when its logic state equals 0. This means that the tag assigned to the XIO instruction is active.
<!-- DIVIDER ---------------------------------------------------------------------------------------------------------------------------------------------------------->
## Project 2: Stop Button Example

![StopButton](https://raw.githubusercontent.com/CHill-Three/logixpro.projects/main/Project%202%3A%20Stop%20Button%20Example/StopButton.PNG?raw=true "StopButton")

#### Description: 
In the beginning, nothing is activated. But as soon as the pushbutton is pressed, the instruction is highlighted, and the conveyor starts. Now, the memory address of the conveyor within PLC software equals one. So as soon as the pushbutton is released, the Ladder Logic will use the CLN instruction to keep the output on, to keep the conveyor working. Since we're using a normally open contact for the Stop Pushbutton, we will use an XIO instruction to preserve the continuity. Now, in a normal situation, the Stop pushbutton is not pressed. It's a normally open contact. So the memory location equals zero. And when using an XIO instruction, the instruction is highlighted when the memory location is zero. When both inputs are on, the output is on as a result. And the CLN instruction works the same way. The output will stay on even if the Start pushbutton is released. As soon as the operator presses the Stop pushbutton, remember it's a normally open contact, so it changes the state to one. And this means the XIO instruction is not activated anymore. And as a result, the conveyor stops.  
<!-- DIVIDER ---------------------------------------------------------------------------------------------------------------------------------------------------------->
## Project 3: Conveyor Example

![Conveyor](https://raw.githubusercontent.com/CHill-Three/logixpro.projects/main/Project%203%3A%20Conveyor%20Example/Conveyor.PNG?raw=true "Conveyor")

#### Description:
In this example, we have one input and two outputs. The input, in this case, is the conveyor memory bit. Remember that inputs and outputs can be in internal bits. So now, using the memory as its location of the conveyor bit to turn on the two lights. Since we have multiple outputs, we add them in parallel. Now once the operator pushes the start push button, the conveyor starts. As soon as the conveyor starts, the two lights turn on. The last thing to program is adding the red light when the conveyor is not working. For this task, the exact memory location of the conveyor bit. But this time, we use an XIO instruction to indicate that the output is only on when the conveyor is not working when the conveyor is not on. Note that the same address for the conveyor for the two green lights — the same address as the conveyor to connect it to the red light. The only difference is that an XIO instruction was used. For the demonstration, the first light is yellow to indicate that the conveyor is on. The second light is the first green light. The third light is for the second green light.
<!-- DIVIDER ---------------------------------------------------------------------------------------------------------------------------------------------------------->
## Project 4: Simple Latching and Unlatching Example

![Latching-Unlatching](https://raw.githubusercontent.com/CHill-Three/logixpro.projects/main/Project%204%3A%20Simple%20Latching%20and%20Unlatching%20Example/Latching-Unlatching.PNG?raw=true "Latching-Unlatching")

#### Description:
An output latching instruction is used to maintain or latch output on, even if the input condition changes. So, if any run has a latching instruction, the output reference to the latching instruction is turned on, even if the run logic or the PLC power is lost. Latch, to latch output on; the output stays on until unlatch instruction becomes true. Unlatch instruction to unlatch a latched-on instruction with the same address.
