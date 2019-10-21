# Flashing the ATmega1284P through USB

To program the ATmega1284P, install download AVROSP.

This guide assumes that you have AVROSP added to your PATH.

1) When you first plug in the board

2) Hold RESET and SW0

3) Let go of RESET

4) Let go of SW0

5) In the terminal, enter the command "mode comx baud=57600 parity=n data=8".
    Replace the "x" in "comx" with the COM port that your board is plugged into.
    (This can be found in the "Device Manager" on windows)

6) In the folder where your .hex file is, run the following command:
    "AVROSP -dATmega1284P -cCOMx -pf -vf -if"filename.hex" -e".
