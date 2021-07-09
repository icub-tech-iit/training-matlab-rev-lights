# Training Project on Implementing a State-Controlled Gear selection with a LED feedback powered by STM32 Nucleo

This repository consists of folders containing the MATLAB and Simulink files based on the following examples and projects:

- [Model Finite State Machines](https://www.mathworks.com/help/stateflow/gs/finite-state-machines.html)
- [MAKE ARDUINO RGB REV LIGHTS w SIMHUB](https://img.youtube.com/vi/u5kZjg_sJdg/0.jpg)


| [![](https://img.youtube.com/vi/u5kZjg_sJdg/0.jpg)](https://www.youtube.com/watch?v=u5kZjg_sJdg) |
| :---------------: |
| (🔘 click on the image to play teh video on Youtube) |


## Prerequisites

| Knowledge            | Level     |
| -------------        | ---------- |
| Matlab               | ⭐
| Simulink             | ⭐⭐
| Stateflow            | ⭐⭐⭐

**Note:**
We recommend completing the [Getting Started with Simulink Coder Support Package for STMicroelectronics Nucleo Boards](https://www.mathworks.com/help/supportpkg/nucleo/ug/getting-started-with-simulink-coder-support-package-for-stmicroelectronics-nucleo-boards.html) example.


## Required Hardware
- Supported STMicroelectronics Nucleo board
- USB cable type A to Mini-B cable


## The goal 🎯

The purpose of this project is learn how to combine Simulink, Simscape and Stateflow and how we cane use them to control a gear selection system with a LED feedback coming from a [NUCLEO-L476RG](https://www.st.com/en/evaluation-tools/nucleo-l476rg.html) board.

## Tasks

- [ ] Implement a **simplified** State-Controlled Four-Gear Selection based on the [Automatic Transmission Controller](https://www.mathworks.com/help/simulink/slref/modeling-an-automatic-transmission-controller.html) example.
- [ ] Each time a gear is scaled up/down the LED should blink once.
- [ ] Once the the system reaches the last gear and the engine is revving, the LED should blink rapidely.

#### Optionals:

- The intensity of main LED (PIN 13) should be managed proportionaly to the current gear selected.
- If you own an RGB LED stripe you can use it instead of the main LED.

## Main Flow

This section shows the main steps I followed to achieve the goal.

### Learn
- [Simulink onramp](https://www.mathworks.com/learn/tutorials/simulink-onramp.html)
- [Stateflow onramp](https://www.mathworks.com/learn/tutorials/stateflow-onramp.html)
- [Simulink Coder Support Package Using STMicroelectronics Nucleo Boards](https://www.mathworks.com/matlabcentral/fileexchange/58942-simulink-coder-support-package-for-stmicroelectronics-nucleo-boards)

---

### Code
1. [Simulink-Stateflow implementation of the Gear Logic](1_Gear_logic)
2. [Implementing the LED bliking logic](2_Gear_logic_with_LED_feedback)
3. [Code generation and deployment on STM32 Nucleo](3_Gear_logic_on_stm32)

__Note__:
- Each folder contains a README that shows the main work of the relative step.
- All the sources in this repository have been tested on Matlab R2021a.