#Project Overview

This project demonstrates inter-task communication using FreeRTOS Queue on STM32 Nucleo-F446RE. One task works as a producer that generates data, while another task works as a consumer that receives the data.

#Objective

To implement communication between two tasks using FreeRTOS Message Queue.

#Hardware Required
STM32 Nucleo-F446RE Board
USB Cable


#Software Required
STM32CubeIDE
STM32CubeMX
FreeRTOS

#Tasks Used
Producer Task - Sensor_Read
Generates distance values every 1 second
Sends data to queue
Consumer Task - Motion_Control
Waits for data from queue
Receives and prints data