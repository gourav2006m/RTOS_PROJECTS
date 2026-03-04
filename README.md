# RTOS_PROJECTS

STM32F446RE RTOS Project Repository
Real-Time Embedded Systems using FreeRTOS

This project repository contains a structured set of Real-Time Operating System (RTOS) based embedded projects implemented on the STM32F446RE microcontroller using STM32CubeIDE and FreeRTOS.

The project demonstrates the transition from Bare-Metal Programming to Super Loop Architecture and finally to Multitasking with FreeRTOS and advanced synchronization techniques.

Project Objective
The goal of this project is to design and implement real-time embedded applications that demonstrate:
- Deterministic task scheduling
- Preemptive multitasking
- Task prioritization
- Interrupt-to-task synchronization
- Inter-task communication
- Shared resource protection
- Timing and processor load analysis


Phase 1 – Embedded Fundamentals (Bare-Metal Programming)

1. GPIO Output – LED Blinking
Objective:
Configure a GPIO pin as digital output and verify LED blinking using software delay routines.

Concepts:
GPIO configuration
Register-level control
Software delay loops


2. Push Button Interface – LED Toggle
Objective:
Interface a push button as digital input and toggle LED state on each valid button press.

Concepts:
Input mode configuration
Pull-up / Pull-down resistors
Button debouncing


3. HC-SR04 Ultrasonic Sensor Interfacing
Objective:
Interface an ultrasonic sensor and classify distance ranges using LEDs.

Concepts:
Trigger and Echo pulse measurement
Timer-based pulse width calculation
Distance computation


4. PWM Generation – LED Brightness Control
Objective:
Generate PWM signal using a timer and control LED brightness by varying duty cycle.

Concepts:
Timer peripheral configuration
PWM modes
Duty cycle control


5. Super Loop Embedded Architecture
Objective:
Implement a sequential embedded program that performs LED blinking, button monitoring, and sensor data acquisition using timing counters.

Concepts:
Cooperative scheduling
Super-loop limitations
Blocking vs Non-blocking execution


Lab Evaluation 1 – Introduction to FreeRTOS

6. Basic FreeRTOS Project
Objective:
Create a single RTOS task to blink an LED.

Concepts:
Task creation
Scheduler start
RTOS vs Bare-metal comparison


7. Task Priorities Analysis
Objective:
Create two tasks with different priorities and analyze their effect on LED blinking behaviour.

Concepts:
Preemptive scheduling
Priority-based execution
Starvation conditions


8. EXTI with Task Notification / Binary Semaphore
Objective:
Configure an external interrupt for a user button and synchronize an LED control task.

Concepts:
ISR to task communication
Binary semaphore
Task notification


9. Queue + UART Communication
Objective:
Task 1 acquires sensor data and sends it to a queue.
Task 2 receives the data and transmits it over UART.

Concepts:
Queue creation
Blocking calls
Safe communication between tasks


Lab Evaluation 2 – Advanced FreeRTOS Concepts

10. Counting Semaphore – Shared Resource Modeling
Objective:
Model a limited shared resource using a FreeRTOS counting semaphore when multiple tasks request access.

Concepts:
Resource allocation
Concurrent task behaviour
Access control


11. Mutex for UART – Mutual Exclusion
Objective:
Implement mutual exclusion for a shared UART peripheral when multiple tasks attempt to transmit data simultaneously.

Concepts:
Mutex vs Semaphore
Priority inheritance
Data corruption prevention


12. Periodic Tasks – vTaskDelayUntil vs vTaskDelay
Objective:
Implement two periodic tasks using vTaskDelayUntil and compare their timing behaviour with tasks implemented using vTaskDelay.

Concepts:
Precise periodic execution
Timing drift
Jitter analysis


Hardware and Tools
Board: Nucleo-F446RE
Microcontroller: STM32F446RE (Cortex-M4)
IDE: STM32CubeIDE
RTOS: FreeRTOS

Peripherals Used:
GPIO
EXTI
UART
Timers
PWM
Ultrasonic Sensor


Learning Outcomes
Through this project the following skills were developed:

RTOS task management
Scheduling and priority control
Inter-task communication
Resource protection mechanisms
Interrupt-driven synchronization
Deterministic periodic systems
Real-time system behaviour analysis

