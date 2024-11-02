# Two-Stage Operational Amplifier Design with Miller Compensation (65nm Technology)
Design and analysis of a two-stage operational amplifier using Miller compensation in 65nm technology, optimized to meet specified performance requirements.


## Objective
The objective of this project is to design and analyze a two-stage operational amplifier using 65nm technology, incorporating Miller compensation to achieve the desired performance metrics.


## Specifications
The design requirements for the two-stage operational amplifier are as follows:
- Technology: 65nm CMOS
- Architecture: Two-stage operational amplifier with Miller compensation
- Supply Voltage (VDD): 1.2V
- Input Common Mode Range (ICMR): 0.6V to 1V
- Target DC Gain: 60 dB
- Unity Gain Bandwidth (UGB): ≤ 30 MHz
- Phase Margin: ≥ 60°
- Slew Rate: 20 V/µs
- Load Capacitance (CL): 2 pF
- Power Dissipation: ≤ 150 µW

These specifications aim to balance gain, stability, and speed while ensuring the amplifier operates within the provided common mode range and supply constraints.


## Design Approach
The design of the two-stage operational amplifier using Miller compensation in 65nm technology involves several key considerations to achieve the desired performance metrics. The following outlines the approach taken in the design process:

1. **Circuit Topology**:
The amplifier is based on a two-stage configuration, which includes a differential input stage and a gain stage.
The differential input stage amplifies the input signal and provides a high input impedance, while the gain stage further amplifies the signal to meet the target DC gain of 60 dB.

3. **Miller Compensation**:
Miller compensation is employed to enhance stability by controlling the dominant pole location in oredr to achieve the desired Phase Margin and bandwidth for the amplifier.
A compensation capacitor is strategically placed between the output of the first stage and the input node of the second stage to ensure a phase margin of at least 60°.

5. **Zero Location Assumption**:
It is assumed that the zero location is set at ten times the unity gain bandwidth (UGB). This assumption helps in optimizing the frequency response and ensuring the stability of the amplifier within the specified bandwidth constraints.

7. **Transistor Sizing**:
Transistor sizes were initially calculated based on the given specifications to ensure that the design met the target performance criteria, including Phase Margin, Slew Rate, Unity Gain Bandwidth, Input Common Range and Assumption used.
After initial calculations, the transistor sizes were fine-tuned through simulation iterations to achieve the desired results and optimize performance.

9. **Simulation and Iteration**:
Extensive simulations using Cadence Virtuoso analyzed the amplifier's gain, phase response, and stability. Parametric analysis evaluated the effects of various parameters, leading to adjustments in transistor sizes and compensation capacitor values. Iterative refinements were made to fine-tune performance and ensure compliance with design specifications.


## Hand Calculations and Design Analysis
This section presents the theoretical calculations and analyses performed during the design of the two-stage operational amplifier. 
Detailed hand calculations for various parameters, including Phase Margin, Slew Rate, Unity Gain Bandwidth, Input Common Range, were conducted to establish a solid foundation for the design.
To support the design process, an image containing all calculations and analyses is provided at the end of this README file. This document includes:
- Theoretical derivations for key performance metrics.
- Calculations for transistor sizing based on the specified requirements.
- A description of the fine-tuning process to optimize performance and meet the targeted specifications.

The results from these calculations were critical in guiding the design decisions and ensuring that the amplifier met the targeted specifications.


## Simulation Results and Performance Summary
The performance of the two-stage operational amplifier was thoroughly evaluated through simulations conducted in Cadence Virtuoso. 
The results are illustrated in the following plots, which includes markings for critical parameters such as- Unity Gain Bandwidth (UGB), 3 dB Cutoff Frequency, Phase Margin, Gain Margin, Phase Crossover Frequency, Gain Crossover Frequency etc.
The amplifier achieved a DC gain ≥ 60 dB and Phase Margin: ≥ 60°, successfully meeting the design target. 
The gain and phase plots display the amplifier's frequency response and provide insights into its stability.

There are two different graphs plotted for minimum and maximum input common mode range, Vcm (0.6V-1V).

**Frequency Response for Vcm=0.6V**

![gain_phase_plot_Vin_600mV](https://github.com/user-attachments/assets/acf35639-c509-4cc9-a4ef-929b8b7a91a8)

**Frequency Response for Vcm=1V**

![gain_phase_plot_Vin_1V](https://github.com/user-attachments/assets/5a5438e4-d7c6-4c44-a2ce-dc73255fe5b6)

Exact values of parameters obtained is shown in the **Hand Calculations and Design Analysis** document at the end of this README file (pdf also attached above).
All results obtained were in accordance with the design specification limits, which can be verified from the provided plot images. The detailed markings on the plots aid in understanding the operational characteristics of the amplifier.


## Conclusion
The design of the two-stage operational amplifier using Miller compensation in 65nm technology successfully met the performance specifications, achieving a DC gain of 60 dB, a phase margin above 60°, and maintaining power dissipation under 150 µW. 
Through extensive simulations in Cadence Virtuoso and a thorough fine-tuning process, the amplifier demonstrated robust stability and compliance with design targets across the input common mode range. 
This project highlights the importance of iterative design and simulations in optimizing analog circuits.


## Hand Calculations and Design Analysis Document
![test_schematic111](https://github.com/user-attachments/assets/361f651a-a298-4381-9201-e9fbb10aea29)
![2 Stage OP-AMP](https://github.com/user-attachments/assets/6c405013-a76f-41e3-901a-92ef6f6e95e9)
