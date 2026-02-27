# Servicios-del-nucleo-Linux
[Unit]
Description=Servidor Web Flask
After=network.target

[Service]
Type=simple
User=angel
WorkingDirectory=/home/angel/flask_app
ExecStart=/home/angel/flask_app/venv/bin/python /home/angel/flask_app/app.py
Restart=always
RestartSec=3
StartLimitIntervalSec=0

[Install]
WantedBy=multi-user.target

# Uso de la memoria RAM
Se crea el programa que leera la Ram cada 15s:

<img width="1366" height="768" alt="image" src="https://github.com/user-attachments/assets/8d9c1a76-e9cf-4b98-97f8-b380196e21a3" />

Seguido de haber creado el archivo se guarda y ejecuta en otro terminal:

<img width="1349" height="721" alt="image" src="https://github.com/user-attachments/assets/e67e2de1-cb56-48a4-9516-3523a7ba147a" />

Se mueve el archivo a ejecutables del sistema sudo porque ese directorio pertenece a root y se crea el servicio 

<img width="993" height="511" alt="image" src="https://github.com/user-attachments/assets/5bc806ff-cd24-45e0-8876-c97b5b00b848" />


