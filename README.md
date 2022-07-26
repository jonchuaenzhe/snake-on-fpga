March 2020
# Snake (Game) on FPGA

As part of the NUS module EE2026 Digital Design, this project implements a sound-activated snake game on a Basys-3 FPGA with a small LED screen attached.

## Demo

https://user-images.githubusercontent.com/59247141/175206782-ab4825d0-3e95-4a00-8c69-665f64886dcb.mp4

## Game Features

The game is similar to the traditional snake, except that it turns only when the FPGA detects the right sound pitch. If a high-pitched sound is detected, the snake turns right, while the right volume bar will light up. If a low-pitched sound is detected, the snake will turn left and the opposite volume bar lights up.

## Main Functions

"plot_snake_test.v" contains the key logic for a memory efficient implementation of the snake game. This is especially important when "appending" to an array is not feasible in Verilog.

"lpf.v" and "hpf.v" contains the code for finite impulse response filters that process the incoming sound to trigger the snake movement.

"Audio_Capture.v" contains code to interface the FPGA with the microphone module.

"Oled_Display.v" contains the code to interface the FPGA with the LED screen.