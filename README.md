March 2020
# Snake (Game) on FPGA

As part of the NUS module EE2026 Digital Design, this project implements a sound-activated snake game on a Basys 3 FPGA with a small LED screen attached.

## Demo

https://user-images.githubusercontent.com/59247141/175206782-ab4825d0-3e95-4a00-8c69-665f64886dcb.mp4

## Game Features

The game is similar to the traditional snake, except that it turns only when the FPGA detects the right sound pitch. If a high-pitched sound is detected, the snake turns right, while the right volume bar will light up. If a low-pitched sound is detected, the snake will turn left and the opposite volume bar lights up.

## Implementation Challenges

fir

memory