Introduction
============

The goal of this project is make a single framework to learn about microcontroller Cortex-M0+.&nbsp;  The project is a fork of [OpenKL25Z](https://github.com/1nv1/OpenKL25Z) which was based on [bare-metal ARM](https://github.com/payne92/bare-metal-arm).&nbsp;  It is a bare-metal runtime for the 
[Freescale Freedom FRDM-KL25Z](http://www.freescale.com/webapp/sps/site/prod_summary.jsp?code=FRDM-KL25Z) 
ARM development board ($12.95).&nbsp;  It builds with the GCC ARM toolchain, with no other external dependencies.

Quick start on Ubuntu 20.04 LTS (in 2022):

+ Install the tools <br />
`sudo apt install git screen gcc-arm-none-eabi`

+ Connect the cable to the USB port marked as SDA, then mount (or click on the) `FRDM-KL25Z` USB removable disk.

+ `git clone https://github.com/RoGeorge/OpenKL25Z` <br />
`cd OpenKL25Z` <br />
`make deploy` <br />
will make the project and will program the devboard by copying the `.SREC` file to the `FRDM-KL25Z` volume

+ The RGB LED will flash quickly.
 
+ To connect to the serial port <br />
`screen /dev/ttyACM0 115200` <br />

+ Use the capacitive touch to navigate the menu and select items.&nbsp;  The part of capacitive sensor near of QR code in the board is for navigate, the rest is for select action.

+ To disconnect and kill the `screen` session press `CTRL+a \`

Status
------
It compiles and run, menu text appears in 'screen', seems frozen.
