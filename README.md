# Servicios-del-nucleo-Linux

# Uso de la memoria RAM
## Objetivo

Implementar un servicio del sistema que registre el uso de la memoria RAM cada 15 segundos en el archivo `/tmp/ram_usage.log`,utilizando un script en Bash gestionado por systemd.

##
1. Se crea el programa que leera la Ram cada 15s:

  <img width="663" height="219" alt="image" src="https://github.com/user-attachments/assets/692db097-261b-4fe3-8a2a-bd0c8dc108bc" />

2. Seguido de haber creado el archivo se guarda y ejecuta en otro terminal:

  <img width="1349" height="721" alt="image" src="https://github.com/user-attachments/assets/e67e2de1-cb56-48a4-9516-3523a7ba147a" />

3. Se mueve el archivo a ejecutables del sistema sudo porque ese directorio pertenece a root y se crea el servicio, ademas se comprueba con sudo systemctl status ram_logger 

  <img width="979" height="511" alt="image" src="https://github.com/user-attachments/assets/4a4e9461-31c2-42df-98a2-464843410a27" />

4. Ejecucion del servicio

  <img width="710" height="388" alt="image" src="https://github.com/user-attachments/assets/349036ed-0533-4794-a515-0ef3e39163e9" />

5. Ejecucion despues de aproximadamente dos minutos 

  <img width="788" height="486" alt="image" src="https://github.com/user-attachments/assets/44d794ed-bdda-45e2-ab66-746908250cec" />

#  Servidor web usando python y flask.
## Objetivo

Implementar un servidor web usando Python y Flask, ejecutado como servicio gestionado por systemd.

1. Se instalan las dependencias
   
   sudo apt install python3.12-full -y

2. Se crea un entorno virtual usando flask
   
   <img width="970" height="507" alt="image" src="https://github.com/user-attachments/assets/f6a742dc-63f4-4fef-ad35-c13e9c889d73" />

3. Se crea el archivo nano app.py
   
   <img width="539" height="223" alt="image" src="https://github.com/user-attachments/assets/d5d515a3-0818-4539-890f-0127c49a5bb4" />

5. A continuación se prueba su funcionamiento
   
   <img width="960" height="305" alt="image" src="https://github.com/user-attachments/assets/7124b769-b1d3-4f05-9b36-e347c79f4b40" />
   
   <img width="1363" height="680" alt="image" src="https://github.com/user-attachments/assets/d7b534e0-01c8-46ba-82e9-64d177451f50" />

7. Se crea el servidor
   
   <img width="969" height="512" alt="image" src="https://github.com/user-attachments/assets/859b075d-f5b2-46ed-9940-1b98d3617df8" />
   
8. Se comprueba el estado del mismo:
   
   <img width="976" height="508" alt="image" src="https://github.com/user-attachments/assets/1cf05e95-b5a9-48fd-ba67-975b8bbd4759" />

## Conclusión

Se implementaron correctamente los objetivos mediante servicios gestionados por systemd, tanto el servicio de monitoreo de memoria RAM como el servidor web Flask; ambos sistemas se ejecutan en segundo plano y además inician automáticamente al arrancar el sistema. Para el primero, se ejecutó un script en Bash en un sistema para que se ejecutara en segundo plano automáticamente; mientras tanto, el segundo se creó dentro de un entorno virtual para mantener aisladas sus dependencias, igualmente como un servicio para funcionamiento continuo.











