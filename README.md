# Embedded Systems Lab 6: Data Acquisition, DMA, and Interrupt

This repository contains the solution to **Lab 6: Data Acquisition, DMA, and Interrupt**. The project demonstrates the configuration of **ADC (Analog-to-Digital Converter) with DMA (Direct Memory Access)** on an **STM32 microcontroller**, acquiring temperature sensor data and handling it using interrupts for efficient data processing.

---

## Problem Statement

The objective of this lab is to set up an **ADC** to sample data from the **STM32 internal temperature sensor** at a fixed frequency, using **DMA** and **interrupts** to manage data transfer and print sensor values via UART. This lab requires:

1. **ADC and Timer Configuration**: Setting up **ADC1** to sample data at a fixed frequency, using **TIM1** as the trigger. The parameters for sampling frequency must be set and explained.
2. **RTOS Task Notification**: Using an interrupt to notify an RTOS task to output temperature values through **UART** after each ADC conversion.
3. **DMA Implementation**: Configuring **DMA** to transfer data from the ADC data register to a specific buffer. 
4. **Buffer and Interrupt Handling**: Generating interrupts when each half of the buffer is filled, allowing for efficient data transfer and printing of sensor values.
