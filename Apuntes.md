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

   DELTA_CALIBRATE

Tras la calibracion tendremos esta salida por terminal, tenemos que editar el printer.cfg con dichos valores y ejecutar RESTART.

Recv: // stepper_a: position_endstop: xxx.xxxxxx angle: xxx.xxxxxx
Recv: // stepper_b: position_endstop: xxx.xxxxxx angle: xxx.xxxxxx
Recv: // stepper_c: position_endstop: xxx.xxxxxx angle: xxx.xxxxxx
Recv: // delta_radius: xxx.xxxxxx

   PID_CALIBRATE HEATER=extruder/heater_bed TARGET=Temperatura 
  
Tras terminar el ajuste PID, hay que introducir los valores nuevos en el printer.cfg y ejecutar RESTART.

Recv: // PID parameters: pid_Kp=xx.xxx pid_Ki=x.xxx pid_Kd=xxx.xxx


Si añadimos [WRITE_FILE=1] se envia un log a /tmp/heattest.txt

