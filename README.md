# Servicios-del-nucleo-Linux

# Uso de la memoria RAM
## Objetivo

Implementar un servidor web usando Python y Flask, ejecutado como servicio gestionado por systemd
##
Se crea el programa que leera la Ram cada 15s:

<img width="663" height="219" alt="image" src="https://github.com/user-attachments/assets/692db097-261b-4fe3-8a2a-bd0c8dc108bc" />

Seguido de haber creado el archivo se guarda y ejecuta en otro terminal:

<img width="1349" height="721" alt="image" src="https://github.com/user-attachments/assets/e67e2de1-cb56-48a4-9516-3523a7ba147a" />

Se mueve el archivo a ejecutables del sistema sudo porque ese directorio pertenece a root y se crea el servicio, ademas se comprueba con sudo systemctl status ram_logger 

<img width="979" height="511" alt="image" src="https://github.com/user-attachments/assets/4a4e9461-31c2-42df-98a2-464843410a27" />

Ejecucion del servicio

<img width="710" height="388" alt="image" src="https://github.com/user-attachments/assets/349036ed-0533-4794-a515-0ef3e39163e9" />

Ejecucion despues de aproximadamente dos minutos 

<img width="788" height="486" alt="image" src="https://github.com/user-attachments/assets/44d794ed-bdda-45e2-ab66-746908250cec" />

#  Servidor web usando python y flask.
## Objetivo
Implementar un servidor web usando Python y Flask, ejecutado como servicio gestionado por systemd.


