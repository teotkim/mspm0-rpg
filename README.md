# MSPM0 Embedded RPG

[Watch the gameplay demo](https://www.youtube.com/watch?v=2-qhBU9jKmY)

A bare-metal role-playing game written in C for the TI MSPM0G3507.
Built as a two-person project for UT Austin’s Embedded Systems Honors
course, the game runs on a microcontroller with physical controls,
an ST7735 LCD, and DAC audio.

## My contribution

I led the programming and firmware development. My work included
implementing gameplay logic and integrating the controls, display,
and sound so they worked together on the board.

## How the firmware works

A hardware timer sets the pace of gameplay at 30 updates per second.
Each update uses player input to advance the game state, move
characters, and check collisions. The display code draws the map
and sprites on the LCD, and a separate SysTick interrupt supplies
audio samples to the 5-bit DAC.

The game has six states, two maps, and four enemy types. The main
engineering challenge was coordinating gameplay, display updates,
and audio on one microcontroller, each with different timing needs.

## Project materials

The demo shows the game running on the physical hardware. This
repository contains the project write-up and demo link. The course
source code is kept private.
