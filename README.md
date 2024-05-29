# Control Systems Engineer

**Summary:** I am a Master's student at NC State University with a specialization in Power Electronics and Control Systems. I'm skilled in converter and motor modeling, simulation, and control system design and implementation. I have worked with conventional PMSMs but also the not-so-common Switched Reluctance Machines (SRMs). I am skilled in dynamometer bench setup and embedded coding on TI DSPs. I have also used tools such as dSPACE for rapid control prototyping and evaluation.

## 💻 Technical Skills
|      |     |
|:-----|:----|
| **Programming** | MATLAB/Simulink, Embedded C, Python |
| **Software** | LTspice, PLECS, Code Composer Studio, Altium |
| **Hardware** | Dynamometer, TI C2000 MCU, dSPACE |
|     |      |

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

Developed a model for field-oriented control of a split-phase PMSM in Simulink utilizing a sinusoidal modulation technique. Experimentally verified the speed control of two series-connected PMSMs driven by a single six-phase inverter, utilizing the TI 
F28335S microcontroller; illustrating potential applications in electric vehicles and rovers.

![EEG Band Discovery](/assets/setup_2.jpg)

### Control scheme using Reaction Control Thrusters for Pitch Stability during Atmospheric Abort of Crew Module
[Publication](https://link.springer.com/chapter/10.1007/978-981-19-3938-9_11)

Utilized wind tunnel data to identify the crew module’s stable trim points and identify regions of stability. Designed a hysteresis controller utilizing flight path angle and angle of attack data to generate the required control action. Conducted a feasibility study to determine the optimum RCS thruster force for achieving desired mission objectives. Designed and implemented a modified control logic to reduce thruster chattering and enhance fuel efficiency.

![Bike Study](/assets/on_off_control.png)

### Torque and Speed Control of a Three-phase Induction Machine (IM) in an EV propulsion drive

Developed a model of an IM in Simulink incorporating a vehicle load model and conducted robustness studies. Designed cascaded control loops using frequency response analysis for field-oriented torque and speed control. Implemented indirect rotor flux estimation methods and verified the transient response for a given speed profile.

![Bike Study](/assets/torque_profile_IM.png)

### Control Software-in-Loop (SIL) Validation of a Grid Connected Voltage Source Inverter (VSI)

Designed and implemented cascaded control loops for real and reactive power regulation of a grid-connected inverter. Implemented a space vector PWM technique to generate modulation signals and verified the operation. Developed C-code for the controller and validated system performance using the UNIFI SIL wrapper library in Simulink.

![Bike Study](/assets/demoResultDroop.png)

### Simulation and Control of a Half-bridge Center-tapped Series Resonant Converter (SRC)

Developed an LTspice simulation model of the converter using the manufacturer’s component models and performed loss analysis. Developed a small signal model of the converter, and validated the performance with the converter switching model in Simulink. Designed and implemented a voltage compensator on a TI F28379D MCU, achieving a maximum output settling time of 10ms.

![Bike Study](/assets/bode_designer_592.png)

### Design, Simulation and Control of a Multi-Output Flyback DC/DC Converter

Conducted trade-off studies for the selection of MOSFETs/Diodes and reactive components to meet 92% converter efficiency. Designed a lead-lag compensator using frequency response analysis and validated its performance in PLECS, achieving 10% maximum overshoot and 20ms settling time.

![Bike Study](/assets/schematic_closedloop_534.png)

## 🖋️ Publications
1. N. Gupta, G. T. G. and R. S. Kaarthik, "Modeling and Decoupled Control of Series-Connected Split-Phase Synchronous Machines With Open-Circuit Fault," in IEEE Transactions on Industry Applications, Jan.-Feb. 2020, doi: 10.1109/TIA.2019.2951508
2. Sakunthala, S., Gupta, N., Roy, A. and Sharma, K.K., 2021, October. On–Off Control Scheme Using Reaction Control Thrusters for Pitch Stability During Atmospheric Abort of Crew Module. In National Conference on Multidisciplinary Analysis and Optimization (pp. 113-121). Singapore: Springer Nature Singapore.
3. Gupta, N. and Kaarthik, R.S., 2018, December. Decoupled control of two series connected split-phase synchronous machines from a single six-phase inverter. In 2018 IEEE International Conference on Power Electronics, Drives and Energy Systems (PEDES) (pp. 1-6). IEEE.
4. Gopika, T.G., Gupta, N. and Kaarthik, R.S., 2018, December. Modeling, simulation, and analysis of series-connected split-phase synchronous motor drive. In 2018 8th IEEE India International Conference on Power Electronics (IICPE) (pp. 1-6). IEEE.

## 📜 Certifications
- Introduction to Self-Driving Cars [Credential](https://www.coursera.org/account/accomplishments/verify/VL4CYKBNCTFT)
- Machine Learning [Credential](https://www.coursera.org/account/accomplishments/verify/DJMPDFPA8MM3)
