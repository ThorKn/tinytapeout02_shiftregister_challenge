![](../../workflows/gds/badge.svg) ![](../../workflows/docs/badge.svg)

Go to https://tinytapeout.com for instructions!

# Shiftregister Challenge 40 Bit

## TinyTapeout 02

This repository contains a mikrochip design done for TinyTapeout.
Go to https://tinytapeout.com for more informations.

This is a re-submission from TinyTapeOut 01. So the code in this project is a clone from the TT01 project (same wokwi ID).

## Wokwi project

https://wokwi.com/projects/341516949939814994

## Information about the design

author:       "Thorsten Knoll"

title:        "Shiftregister Challenge 40 Bit"

description:  "The design is a 40 bit shiftregister with a hardcoded 40 bit number. The challenge is to find the correct 40 bit to enable the output to high. With all other numbers the output will be low."

how_it_works: "Shift a 40 bit number into the chip with the two inputs data (IN0) and clk (IN1). If the shifted 40 bit match the hardcoded internal 40 bit, then and only then the output will become high. Having only the mikrochip without the design files, one might need reverse engineering and/or side channel attacks to find the correct 40 bit."

how_to_test:  "Get the correct 40 bit from the design and shift them into the shiftregister. Each rising edge at the clk will push the next data bit into the register. At the correct 40 bit, the output will enable high."

external_hw:  "To test when knowing the correct 40 bit, only a dipswitch (data), a button (clk) and a LED (output) is needed. Without knowing the number it becomes the challenge and more hardware might be required."

language:     "wokwi"

wokwi_id:     341516949939814994

pictures:      
<img src=shiftregister_challenge.png>
<img src=shiftregister_challenge_gds_render.png>

inputs:
  - data
  - clk
  - none
  - none
  - none
  - none
  - none
  - none

outputs:
  - output
  - none
  - none
  - none
  - none
  - none
  - none
  - none
