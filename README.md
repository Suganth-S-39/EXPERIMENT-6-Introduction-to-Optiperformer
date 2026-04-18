
Exp 6 Simulation of Optical Communication System
## Introduction to OptiPerformer 
## Objective
Download and install OptiPerformer software on your computer and run a sample file.

---

## Overview

Optiwave introduces **OptiPerformer**, a free photonic design automation tool that harnesses the full power of OptiSystem and creates specific dynamic design scenarios for student use.

In this exercise, you will:
- Download and install OptiPerformer on your PC/laptop.
- Use your license to load and run OptiSystem simulations prepared for this course.

The first simulation file (`Introduction_OptiPerformer.osp`) models a basic fiber optic system consisting of:
- A transmitter
- A fiber
- A receiver

The system includes:
- An optical power meter at the receiver input (fiber output)
- A Bit Error Rate (BER) analyzer

---

## Instructions

1. Download and install OptiPerformer from [optiwave.com](https://optiwave.com).  
2. Copy the `Introduction_OptiPerformer.osp` file to your PC.  
3. Launch OptiPerformer.  
4. Use the **File** menu or **Open File** button to open the fiber optic system file.  
5. Study the layout:
   - **Transmitter** section includes:
     - Binary source (PRBS generator)
     - Electrical pulse generator
     - Laser diode
     - External modulator  
   - **Receiver** section includes:
     - Photodiode
     - Low-pass filter
     - Decision circuit with BER analyzer  
6. Run the simulation using the **Start** button.  
   - Progress will be displayed.
   - Message “Calculation Finished!” appears upon completion.  
7. Double-click the **optical power meter** and **BER analyzer** windows.  
   - Check “Show Eye Diagram” in the BER window.  
   - Optical power meter shows power in watts and dBm.  
   - BER window displays:
     - Eye diagram
     - Max Q Factor
     - Min BER  
8. The simulation runs 5 iterations with fiber length varying from 50 to 150 km.  
   - Use forward/reverse buttons to step through iterations.  
   - Observe changes in received power, BER, Q factor, and eye diagram.

---

## Report

1. Cover sheet (as per attached example).  
2. Tabulation of received power, Q factor, and BER for 5 fiber lengths.  
3. Plot of received power, Q factor, and BER vs. fiber length.  
4. Description of eye diagram changes with increasing fiber length.

---

## Tabulation

**Transmission Analysis Across Fiber Lengths**

| S.No | Fiber Length (km) | Optical Power (W) | Optical Power (dBm) | Max Q Factor | Min BER        | Eye Height     | Decision Instant |
|------|------------------|-------------------|----------------------|--------------|----------------|----------------|------------------|
| 1    | 60               | 31.056e-6         | -15.079              | 80.778       | 0              | 6.08925e-05    | 0.546875         |
| 2    | 65               | 24.669e-6         | -16.079              | 77.5331      | 0              | 4.83579e-05    | 0.546875         |
| 3    | 75               | 15.318e-6         | -18.148              | 68.1145      | 0              | 3.03516e-05    | 0.546875         |
| 4    | 80               | 12.168e-6         | -19.148              | 57.6252      | 0              | 2.3982e-05     | 0.546875         |
| 5    | 90               | 7.801e-6          | -21.079              | 50.2376      | 0              | 1.49522e-05    | 0.546875         |
---

## Graphs

<img width="1920" height="1080" alt="Screenshot (730)" src="https://github.com/user-attachments/assets/129fdd18-2fd3-4a8e-835b-7d104940e756" />

---

## RESULT

As the fiber length increases from 60 km to 90 km, the received optical power decreases due to attenuation in the fiber. This reduction in power leads to degradation of signal quality, which is observed as a gradual closure of the eye diagram. Consequently, the Q-factor decreases and the Bit Error Rate (BER) tends to increase (though very small in this case). Thus, longer fiber lengths result in poorer system performance and reduced reliability of optical communication.

