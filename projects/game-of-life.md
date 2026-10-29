# Game of Life

**EPFL · Computer Architecture · RISC-V assembly · Gecko5**

[← All projects](../README.md)

## The project

An implementation of Conway's Game of Life in RISC-V assembly, developed in the school's virtual machine for the Gecko5 environment.

Cells evolve on a grid according to their neighbours. The simulation appears on an LED display, with buttons to control its state and progression.

## Features

- Updating the cell grid from one generation to the next.
- Displaying the grid through memory-mapped LEDs.
- Reading button input and handling pause and speed controls.
- Selecting initial patterns or generating a random grid.
- Showing the step count on a seven-segment display.

## Working closer to the hardware

This project involved registers, memory addresses, procedure calls and direct interaction with simulated peripherals. Compared with my Java projects, it required a much more explicit view of how the program stores state and performs each operation.

## Context

I worked on this project in EPFL's Computer Architecture course, using the supplied template and Gecko5 environment. The coursework source code is kept private.

## A first in assembly

This was my first assembly project. I wanted to understand at least the foundations of what happens beneath the languages I usually write. Registers and memory addresses made the computer's architecture much more concrete. Python had been quietly doing quite a lot for me.
