Download Link: https://assignmentchef.com/product/solved-ve270-assignment-7-design-of-a-digital-device
<br>



To design a digital system that

<ul>

 <li>Rolls your SJTU student ID across the four SSDs on the FPGA board when the system starts, then</li>

 <li>Adds two 4-bit 2’s complement numbers and displays the decimal results with the SSDs on the FPGA board.</li>

</ul>

<ol start="2">

 <li><strong> Requirement</strong></li>

 <li>Part 1. Character Rolling</li>

</ol>

The first part of this lab is to roll the student ID of one of the lab partners through the four SSDs from left to right, or right to left, or back and forth. The rolling should start as soon as the device starts functioning or controlled by a switch. The rolling speed is up to the designers, but should be reasonable so people are comfortable to see each character. Other than the student ID, you may choose to display anything or any pattern you want. Be creative!

The student ID is required to roll through the SSDs for only once. But you may choose to roll it multiple times or any time activated by the control switch. As soon as the rolling is done or disabled by the control switch, the system should enter the normal operation mode – calculator.

Part 2. Simple Calculator

The calculator adds two 4-bit 2’s complement numbers, and outputs one 4-bit 2’s complement number which should be interpreted as a signed decimal number and displayed using one (for positive results) or two (for negative results) SSDs. The “–” sign must be displayed using one SSD for negative numbers. The calculator must also detect if there is any overflow in the results and indicate the overflowed results with an LED.

The two 4-bit operands of the calculator must be entered using the same four switches. Thus the operands have to be entered in turn, one after another. A push button must be used to function as the “enter” or “equal” key of the calculator. After the first number is formed using the four switches, the decimal equivalent should be displayed on the SSDs as soon as the “equal” button is pressed. After the second number is formed using the same four switches, the decimal result should be displayed on the SSDs as soon as the “equal” button is pressed. When the “equal” button is pushed multiple times, the calculator shall keep adding the second number to the results each time the button is pressed. The changing results should be updated on the SSDs accordingly. The following table simulates an example.




<table width="0">

 <tbody>

  <tr>

   <td width="112"><strong>Four Switches </strong></td>

   <td width="107"><strong>Equal Button </strong></td>

   <td width="90"><strong>SSD </strong></td>

   <td width="92"><strong>Overflow </strong></td>

  </tr>

  <tr>

   <td width="112">1000</td>

   <td width="107">push</td>

   <td width="90">-8</td>

   <td width="92">0</td>

  </tr>

  <tr>

   <td width="112">0011</td>

   <td width="107">push</td>

   <td width="90">-5</td>

   <td width="92">0</td>

  </tr>

  <tr>

   <td width="112">No change</td>

   <td width="107">push</td>

   <td width="90">-2</td>

   <td width="92">0</td>

  </tr>

  <tr>

   <td width="112">No change</td>

   <td width="107">push</td>

   <td width="90">1</td>

   <td width="92">0</td>

  </tr>

  <tr>

   <td width="112">No change</td>

   <td width="107">push</td>

   <td width="90">4</td>

   <td width="92">0</td>

  </tr>

  <tr>

   <td width="112">No change</td>

   <td width="107">push</td>

   <td width="90">7</td>

   <td width="92">0</td>

  </tr>

  <tr>

   <td width="112">No change</td>

   <td width="107">push</td>

   <td width="90">-6</td>

   <td width="92">1</td>

  </tr>

  <tr>

   <td width="112">No change</td>

   <td width="107">push</td>

   <td width="90">-3</td>

   <td width="92">0</td>

  </tr>

 </tbody>

</table>

1

The above paragraphs describe the requirements for the device. Feel free to add more features and functions to the device.

<strong>NOTE</strong>: your design must be modeled with Verilog HDL.

3. Simulation, Synthesis, and FPGA Implementation

Simulate your circuit if necessary. It is a good idea to verify the functionality of all sub-circuits before you integrate them all together. Synthesize and implement your design on the Basys 3 FPGA board.


