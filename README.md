# MSPM0 Embedded RPG

[Watch the gameplay demo](https://www.youtube.com/watch?v=2-qhBU9jKmY)

A role-playing game built in C for the TI MSPM0G3507 as a two-person
UT Austin Embedded Systems Honors project.

## My contribution

I led the coding and firmware development, including gameplay logic
and integration of the physical controls, LCD, and DAC audio.

## How it works

A 30 Hz timer drives gameplay updates. The game reads player input,
updates player and enemy behavior, checks collisions, and draws the
result on the LCD. It includes six game states, two maps, and four
enemy types.

The course source code is kept private.
