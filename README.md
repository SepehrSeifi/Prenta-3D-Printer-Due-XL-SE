For checking the information on how to use the 3D Printer in Agora Basement Lab see [HERE](https://github.com/SepehrSeifi/Prenta-3D-Printer-Due-XL-SE/blob/main/Agora_Basement_Lab_3D_Printer.md)

# Prenta-3D-Printer-Due-XL-SE
Settings for Prenta 3D Printer Due XL SE

In Ultimaker Cura:
- Add a printer
- Under "Add a non-networked printer", Under "Custom", Select "Custom FFF printer" and press "Add"
- In "Machine Settings", Set the settings as follow:
## "Printer" tab
### Printer Settings
X(Width):  400 mm

Y(Depth):  200 mm

Z(Height): 200 mm

Built plate shape: Rectangular

Origin at center:  

Heated bed:  X

G-code flavor: Repetier
### Printhead Settings
X min: 0 mm

Y min: 0 mm

X max: 395 mm

Y max: 195 mm

Gantry Height: 0 mm

Number of Extruders: 2

Apply Extruder offsets to GCode:  (Only select this option if offsets has NOT been set on the printer itself)
### Start G-code
G21 ;metric values

G28 ;home all

G90 ;absolute positioning

G0 Z15.0 ; move extruder up 15mm
### End G-code
G28 X0 Y0; Home X and Y

G0 Z50.0 ; move extruder up 50mm

M104 S0 ; turn off extruder

M140 S0 ; turn off bed

M107; turn off fans

M84 ; disable motors

## "Extruder 1" tab
### Nozzle Settings
Nozzle size: 0.4 mm

Compatible material diameter: 1.75 mm

Nozzle offset X: -17.62 mm

Nozzle offset Y:  0 mm

Cooling Fan Number: 0
### Extruder Start G-code
T0; Activate Extruder 1
### Extruder End G-code
M104 S0 ; turn off extruder

## "Extruder 2" tab
### Nozzle Settings
Nozzle size: 0.4 mm

Compatible material diameter: 1.75 mm

Nozzle offset X: 18 mm

Nozzle offset Y:  0 mm

Cooling Fan Number: 0
### Extruder Start G-code
T1; Activate Extruder 2
### Extruder End G-code
M104 S0 ; turn off extruder


** Try to find the correct offsets for your own 3D Printer (Follow the instruction in printer user manual)**
