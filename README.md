# Control Systems Engineer

I am a Master's student at NC State University with a specialization in Power Electronics and Control Systems. I'm skilled in converter and motor modeling, simulation, and control system design and implementation. I have worked with conventional PMSMs but also the not-so-common Switched Reluctance Machines (SRMs). I am skilled in dynamometer bench setup and embedded coding on TI DSPs. I have also used tools such as dSPACE for rapid control prototyping and evaluation.

## 💻 Technical Skills
- **Programming** | MATLAB/Simulink, Embedded C, Python
- **Software** | LTspice, PLECS, Code Composer Studio, Altium
- **Hardware** | Dynamometer, TI C2000 MCU, dSPACE

## 🎓 Education
- **Master of Science, Electrical Engineering** <br>
_North Carolina State University (Aug 2022 - Jul 2024)_
- **Bachelor of Technology, Electronics and Communication Engineering** <br>
_Indian Institute of Space Science and Technology (Aug 2014 - May 2018)_

## 💼 Work Experience
**Research Assistant @ FREEDM Systems Center - NCSU** <br>
_Jan 2023 - Present_
- Designed and implemented robust motor control algorithms, such as two degree-of-freedom (2DoF), for Switched Reluctance Machines (SRM) to enhance tracking performance and minimize torque ripple under parameter variations.
- Established and configured a dynamometer test bench, integrating and validating motor control algorithms on an embedded microcontroller platform (TI C2000).

**Mechatronics and Control Systems Intern @ Nexteer Automotive** <br>
_May 2023 - Aug 2023_
- Designed and implemented a novel Model Predictive Control (MPC) algorithm with Integral action for a 12V SRM in an automotive steering application, eliminating steady-state error and achieving a 26% reduction in command tracking error.
- Leveraged rapid prototyping methodologies to implement and validate various control strategies on a dynamometer, using dSPACE for real-time execution, and post-processed the experimental data in MATLAB.

**Scientist/Engineer @ Indian Space Research Organization (ISRO)** <br>
_Aug 2018 - Jul 2022_
- Conducted performance validation of aerospace electromechanical actuators and identification of system parameters.
- Performed mission-critical operations on launch vehicle avionic sub-assemblies; streamlined the testing process through the development of automation sequences, resulting in a 30% reduction in testing time and eliminating user operational error.


## 📚 Academic Projects
### Modeling and Decoupled Control of Series-Connected Split-Phase Synchronous Machines with Open-Circuit Fault
[Publication](https://ieeexplore.ieee.org/abstract/document/8891722)

I started with developing a model for field-oriented control of a split-phase PMSM in Simulink. I verified the decoupled control by providing control voltages in the &alpha; - &beta; frame, which corresponded to torque-producing voltages. However, when the control voltages in the z<sub>1</sub>-z<sub>2</sub> plane were applied, the machine did not produce any torque. Further, I experimentally verified the speed control of two series-connected PMSMs driven by a single six-phase inverter, with coding in TI F28335S microcontroller. This research illustrated the potential applications of split-phase machines in electric vehicles and rovers. 

<centering>
<video width="320" height="240" controls muted>
  <source src="/assets/decoupled_comp.mp4" type="video/mp4">
</video>
</centering>

<!-- ![PMSM_decoupled](/assets/setup_2.jpg)  -->
The video illustrates the decoupled control of the two motors, where one motor runs at a constant speed and the second motor undergoes a transient. It is seen that the speed reversal is smooth and does not affect the dynamics of the first motor.

### Control scheme using Reaction Control Thrusters for Pitch Stability during Atmospheric Abort of Crew Module
[Publication](https://link.springer.com/chapter/10.1007/978-981-19-3938-9_11)

We started by identifying the crew module's region of stability, by utilizing the wind tunnel data to identify the trim points. Then, a hysteresis controller (shown below) was designed that utilized the flight path angle and angle of attack data to generate the required control action. A feasibility study was also conducted to determine the optimum RCS thruster force for achieving desired mission objectives within the specified time. A modified control logic was also designed that aimed at reducing the thruster chattering and enhancing fuel efficiency.

![CrewModule_Control](/assets/on_off_control.png)

### Simulation and Control of a Half-bridge Center-tapped Series Resonant Converter (SRC)

I developed an LTspice simulation model of the converter using the manufacturer’s component models. The converter operation under ZVS and non-ZVS conditions was verified and loss analysis was performed. To design the controller, first, a small signal model of the converter was developed, and its operation was compared against the switching model in Simulink. Then a voltage compensator was designed using frequency response analysis (shown below) in the continuous-time domain. The controller was discretized using Backward-Euler approximation and the performance of both continuous and its discrete-time equivalent was compared. The compensator was then implemented on a TI F28379D MCU. The closed loop system performance was verified by providing changes in reference, input voltage, and output load. The maximum output settling time observed was 10ms.

![SRC_592](/assets/bode_designer_592.png)

### Design, Simulation and Control of a Multi-Output Flyback DC/DC Converter

Conducted trade-off studies for the selection of MOSFETs/Diodes and reactive components to meet 92% converter efficiency. A model of the converter was simulated in PLECS. A small-signal model of the converter was derived and a lead-lag compensator using frequency response analysis was designed to meet the specifications. The closed loop system performance (shown below) was validated in PLECS, where I achieved a 10% maximum overshoot and 20ms settling time under various transient conditions.

![Flyback_534](/assets/schematic_closedloop_534.png)

### Torque and Speed Control of a Three-phase Induction Machine (IM) in an EV propulsion drive

I developed a model of a 3-phase Induction Machine in Simulink incorporating the vehicle load model which included the aerodynamic drag, rolling resistance and gravitational force. I then designed cascaded control loops using frequency response analysis for field-oriented torque and speed control. Both direct and indirect rotor flux estimation methods were used and their impact on control performance under parameter estimation errors was discussed. Finally, the transient response (shown below) was verified for a given speed profile.

![IM_732](/assets/torque_profile_IM.png)

### Control Software-in-Loop (SIL) Validation of a Grid Connected Voltage Source Inverter (VSI)

I designed and implemented cascaded control loops using droop control equations for real and reactive power regulation of a grid-connected inverter. A space vector PWM scheme was used to generate the modulation signals. I then wrote an external C-code for the controller and validated the system performance using the UNIFI SIL wrapper library in Simulink. The results (shown below) show a good transient response of terminal voltage at the Point of Contact (PoC) and the grid side current.

![SIL_792](/assets/demoResultDroop.png)


## 🖋️ Publications
1. N. Gupta, G. T. G. and R. S. Kaarthik, "Modeling and Decoupled Control of Series-Connected Split-Phase Synchronous Machines With Open-Circuit Fault," in IEEE Transactions on Industry Applications, Jan.-Feb. 2020, doi: 10.1109/TIA.2019.2951508
2. Sakunthala, S., Gupta, N., Roy, A. and Sharma, K.K., 2021, October. On–Off Control Scheme Using Reaction Control Thrusters for Pitch Stability During Atmospheric Abort of Crew Module. In National Conference on Multidisciplinary Analysis and Optimization (pp. 113-121). Singapore: Springer Nature Singapore.
3. Gupta, N. and Kaarthik, R.S., 2018, December. Decoupled control of two series connected split-phase synchronous machines from a single six-phase inverter. In 2018 IEEE International Conference on Power Electronics, Drives and Energy Systems (PEDES) (pp. 1-6). IEEE.
4. Gopika, T.G., Gupta, N. and Kaarthik, R.S., 2018, December. Modeling, simulation, and analysis of series-connected split-phase synchronous motor drive. In 2018 8th IEEE India International Conference on Power Electronics (IICPE) (pp. 1-6). IEEE.

## 📜 Certifications
- Introduction to Self-Driving Cars [Credential](https://www.coursera.org/account/accomplishments/verify/VL4CYKBNCTFT)
- Machine Learning [Credential](https://www.coursera.org/account/accomplishments/verify/DJMPDFPA8MM3)
