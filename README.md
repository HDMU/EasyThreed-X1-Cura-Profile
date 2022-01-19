# EasyThreed-X1-Cura-Profile

Add custom FFF Printer


Start gcode:

M109 S180;              wait for 180
G21;                    unit millimeters
G90;                    posizione assoluta
M82;                    estrusore assoluto
M106 S0;
G28 X0 Y0;              move X/Y to min endstops
G28 Z0;                 move Z to min endstops
G1 Z15.0 F900
G92 E0;                 zero the extruded length
G1 F200 E10
G92 E0;                 zero the extruded length again




End gcode:
M140 S0
M104 S0
G91
G1 E-1 F300
G28 X0 Y0
M84
G90


In Extruder 1 check Compatible material diameter
it must be 1.75 instead of 2.85
