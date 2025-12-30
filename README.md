# 🌦️ Weather Rain Alert System

> **Cloud Automation & Data Processing**
> Microservicio diseñado para monitorear condiciones climáticas en tiempo real y enviar alertas automatizadas vía SMS/WhatsApp mediante la API de Twilio.

---

## 📖 Descripción del Proyecto
Este sistema soluciona la necesidad de monitoreo constante de precipitaciones. El script extrae datos meteorológicos, los procesa mediante **Pandas** para identificar umbrales de lluvia y utiliza un servicio de mensajería para notificar al usuario final. El proyecto está optimizado para ejecutarse 24/7 en la nube.



## 🛠️ Stack Tecnológico
![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)
![Pandas](https://img.shields.io/badge/pandas-%23150458.svg?style=for-the-badge&logo=pandas&logoColor=white)
![AWS](https://img.shields.io/badge/AWS-%23FF9900.svg?style=for-the-badge&logo=amazon-aws&logoColor=white)
![Twilio](https://img.shields.io/badge/Twilio-F22F46?style=for-the-badge&logo=twilio&logoColor=white)

---

## ⚙️ Características Técnicas
* **Data Handling:** Uso de la librería **Pandas** para el parseo de JSON y estructuración de pronósticos por horas.
* **Integración de APIs:** Conexión segura con **WeatherAPI** para obtención de datos y **Twilio SDK** para el envío de mensajes.
* **Cloud Deployment:** Configurado en una instancia **Amazon EC2** (Ubuntu Server).
* **Automatización:** Implementación de **Cron Jobs** en Linux para la ejecución programada del script de forma recurrente.

---

## 📂 Estructura del Repositorio
```text
.
├── main.py               # Lógica principal y conexión de APIs
├── requirements.txt      # Dependencias (pandas, twilio, requests)
├── .env.example          # Plantilla para variables de entorno (API Keys)
└── README.md             # Documentación del proyecto
