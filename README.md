# rgb-rev-lights
A State-Controlled Gear selection with a LED feedback powered by STM32 Nucleo

## Introduction

This project has been inspired by the following Youtube video based on an Arduino project:

[![](https://img.youtube.com/vi/u5kZjg_sJdg/0.jpg)](https://www.youtube.com/watch?v=u5kZjg_sJdg)


## The goal 🎯

Learn how to combine Simulink, Simscape and Stateflow and use them to control a gear selection system with a LED feedback from a [NUCLEO-L476RG](https://www.st.com/en/evaluation-tools/nucleo-l476rg.html).

## Tasks

- [ ] Implement a State-Controlled Four-Gear Selection based on the Simulink example.
- [ ] Each time a gear is scaled up/down the LED should blink once.
- [ ] Once the the system reaches the last gear and the engine is revving, the LED should blink rapidely.

### Optionals

- The intensity of main LED (PIN 13) should be managed proportionaly to the current gear selected.
- If you own an RGB LED stripe you can use it instead of the main LED.
