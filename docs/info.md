<!---

This file is used to generate your project datasheet. Please fill in the information below and delete any unused
sections.

You can also include images in this folder and reference them in the markdown. Each image must be less than
512 kb in size, and the combined size of all images must be less than 1 MB.
-->

## How it works

SHA-256 core in default mode have memory to write data and control operation. Addresses 0-63 (legacy SHA-256) and 64-79 (expanded for Bitcoin) frame, STATUS_REG at 81 and output result at 86-117.

## How to test

In legacy SHA-256 mode load 512 bits {24'h616263,1'b1,423'd0,64'd24} in the 0-63 bytes ; STATUS_REG bit0 = 1, after calculation validate result to be ba7816bf8f01cfea414140de5dae2223b00361a396177a9cb410ff61f20015ad

## External hardware

List external hardware used in your project (e.g. PMOD, LED display, etc), if any
