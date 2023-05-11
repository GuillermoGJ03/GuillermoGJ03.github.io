## Projects made throughout my career

---

### FPGA-controlled cyber-physical Pong game



This project was done in collaboration with Intel and consisted of making an application-specific cyber-physical system using an FPGA.

In this team project, a Pong game was made in Processing and controlled by the FPGA using the built-in accelerometer and an infrared sensor. I contributed mainly by writing the code for the FPGA to function as the contol unit, specifically DE10-Lite Altera MAX 10 FPGA model, using VHDL as the hardware descriptor language and Intel Quartus Prime as the software design.

---

### Microcontroller-based gas detection safety system

For this team project, made in collaboration with Intel, a digital system for gas detection and measurement of environmental variables for alarm activation and a ventilation system was designed and prototyped, in addition to a dashboard showing the levels of the measured variables.

I contributed in this project collaborating in the writing of the code in C for the ATMega16 microcontroller to use and coordinate several of its components and functions such as: Timers, GPIOs, Serial communication (UART), PWM and interrupts. In addition, I was in charge of the selection of the system components (bill of material).

<figure>
  <img src="images/diagrama_gases.png?raw=true"/>
  <figcaption>gas detector system block diagram</figcaption>
</figure> 

<figure>
  <img src="images/algoritmo_gases.png?raw=true" width="800"/>
  <figcaption>Flowchart</figcaption>
</figure>
 
<figure>
  <img src="images/esquematico_gas.png?raw=true"/>
 <figcaption> Electric diagram </figcaption>
</figure>

<figure>
  <img src="images/resultado_circuito_gas.png?raw=true"/>
 <figcaption>Resulting gas detector circuit</figcaption>
</figure>

<figure>
  <img src="images/modelo_gas.png?raw=true"/>
 <figcaption>Final prototype of gas detector system</figcaption>
</figure>

<figure>
 <p float="center">
   <img src="images/modelo_gas_1.png" width="300" />
   <img src="images/modelo_gas_2.png" width="300" />
   <img src="images/modelo_gas_3.png" width="300" />
 </p>
 <figcaption>Final prototype of gas detector system</figcaption>
</figure>

---

### Smart framework for air pressure control in agricultural equipment

This project consisted in the design and development of a system to measure the pressure of a tire and adjust it to the desired value by the user through a remote graphical interface (dashboard). The objective of this was to be able adapt the tires of John Deere vehicles to the conditions of the terrain and thus maximize their lifespan.

To achieve this team project, my teammates and I used a development board with an STM32 microcontroller, in which we implemented a closed-loop PID control system, and an ESP32 to send data to a remote server using the MQTT protocol. Also, we implemented the CAN protocol between the STM32 and the ESP32 to send and receive tire pressure data. As an extra, a Fourier analysis was implemented to compensate the noise caused by the air pump in the pressure measurement. In addition, to make the project more reliable and professional, we implemented the control system in real-time using FreeRTOS, and use multicore programming to separate the system tasks. One core, an ARM Cortex-M4, was in charge of the control system and the preassure measurement, while in the other core, an ARM Cortex-M7, the communication with the remote server and the frequency analysis were carried out.

In this project I collaborated designing the control system with MATLAB and programming it in C for the STM32 microcontroller. Also, I assisted in the multicore and RTOS implementation. In addition, I was in charge in writing the C program for frequency analysis, specifically implementing the Fast Fourier Transform.



<figure> 
  <img src="images/P1-control-diagram.png?raw=true"/>
  <figcaption>Closed-loop control system diagram</figcaption>
</figure>

<figure>
  <img src="images/P1-schematic.png?raw=true"/>
  <figcaption>Electric diagram</figcaption>
</figure>

<figure>
  <img src="images/P1-freq.png?raw=true"/>
  <figcaption>Frequency analysis results</figcaption>
</figure>

<figure>
  <img src="images/P1-GUI.png?raw=true"/>
  <figcaption>Remote server dashboard</figcaption>
</figure>


---

### Closed-loop control system for a DC motor using ROS

This project consisted of designing and implementing a closed-loop control system for speed and position of a DC motor in conjunction with ROS.

The controller was implemented in a Simulink model, which received the reference through a slider and the motor velocity and position feedback through subscription nodes. In addition, it sent the PWM control signal through the pubisher node to the motor. The DC motor was connected to a development board with an ATMega256 microcontroller to calculate the position and velocity of the motor. It received the control PWM signal through a subscriber node and sent the position and velocity values through a publisher node.

In this project I contributed writing the C code to make the motor speed and position measurements, as well as adjusting the controller gains using methods such as Ziegler-Nichols and Root Locus.

<p>
  <img src="images/controlador_velocidad.png" />
  <em>Controlador de velocidad en MATLAB </em>
</p>



---


<!-- Remove above link if you don't want to attibute -->
