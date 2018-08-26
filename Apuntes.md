## APUNTES SOBRE KLIPPER

HELP - Socorro, te saca todos los comandos.

STATUS - Check de la maquina

RESTART - menu

FIRMWARE_RESTART -

PROBE - Hasta romperte la cama

QUERY_PROBE - Muestra el estado de Z probe

QUERY_ENDSTOPS - M119

DELTA_CALIBRATE - 

PID_CALIBRATE HEATER=extruder/heater_bed TARGET=<temperature> [WRITE_FILE=1] - log a /tmp/heattest.txt

DUMP_TMC STEPPER=stepper_a/b/c - Estado del driver tmc

^ pin con pullup
! inversor de logica 

*por configurar:

BED_MESH_CALIBRATE

BED_MESH_OUTPUT

BED_MESH_OUTPUT

BED_MESH_CLEAR

## CALIBRACIÓN

DELTA_CALIBRATE - 

Recv: // stepper_a: position_endstop: 301.367232 angle: 90.053255
Recv: // stepper_b: position_endstop: 301.092982 angle: 210.061794
Recv: // stepper_c: position_endstop: 300.737168 angle: 330.000000
Recv: // delta_radius: 135.200867
Recv: // To use these parameters, update the printer config file with
Recv: // the above and then issue a RESTART command
