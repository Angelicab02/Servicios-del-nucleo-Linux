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
