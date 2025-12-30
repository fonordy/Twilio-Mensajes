# 🌦️ Weather Alert System

> **Cloud Automation & Data Processing**
> Microservicio diseñado para monitorear condiciones climáticas en tiempo real y enviar alertas automatizadas vía SMS/WhatsApp mediante la API de Twilio.

---

## 📖 Descripción del Proyecto
Este sistema automatiza el monitoreo de precipitaciones para ciudades específicas. El script extrae pronósticos detallados, utiliza **Pandas** para filtrar únicamente las horas con probabilidad de lluvia en un rango diurno (06:00 - 22:00) y notifica al usuario de forma proactiva.



## 🛠️ Stack Tecnológico
![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)
![Pandas](https://img.shields.io/badge/pandas-%23150458.svg?style=for-the-badge&logo=pandas&logoColor=white)
![AWS](https://img.shields.io/badge/AWS-%23FF9900.svg?style=for-the-badge&logo=amazon-aws&logoColor=white)
![Twilio](https://img.shields.io/badge/Twilio-F22F46?style=for-the-badge&logo=twilio&logoColor=white)

---

## ⚙️ Características Técnicas (utils.py)
* **Data Sourcing:** Conexión con **WeatherAPI** mediante manejo de excepciones y validación de respuestas JSON.
* **Transformación de Datos:** Procesamiento de listas de diccionarios a **Pandas DataFrames**.
* **Lógica de Negocio:** Filtrado inteligente de datos para reportar solo eventos de lluvia en horarios relevantes (6 AM a 10 PM).
* **Integración de Mensajería:** Uso del SDK de **Twilio** para la generación dinámica de cuerpos de mensaje con el reporte del clima.

---

## 📂 Estructura del Repositorio
```text
.
├── twilio-script.py      # Flujo de ejecución principal
├── utils.py              # Funciones de API, Procesamiento de Datos y Envío
├── twilio_config.py      # Configuración de credenciales (Omitido por seguridad)
├── requirements.txt      # Dependencias (pandas, twilio, requests, tqdm)
└── README.md             # Documentación del proyecto
