UniHelperBot – Proyecto de Bot Educativo con Red Neuronal (PyTorch + Telegram)

Este repositorio contiene el desarrollo de UniHelperBot, un asistente educativo para estudiantes de la Universidad del Valle, implementado en Python con soporte de redes neuronales basadas en PyTorch.
El proyecto integra inteligencia artificial con un bot de Telegram para ofrecer ayuda académica, acceso a licencias y soporte institucional.

Estructura del proyecto

El proyecto parte de las redes neuronales originales (red_1 a red_4) y las adapta para tareas semánticas dentro del bot, añadiendo nuevos módulos para la interacción con Telegram.

Carpetas y archivos principales:

red_1.py — Red neuronal base (entrenamiento de comprensión de texto).

red_2.py — Red neuronal para clasificación semántica de intenciones.

red_3.py — Red neuronal adaptada para predecir y procesar respuestas cortas.

red_4.py — Red neuronal final, optimizada para uso en el bot (predicciones integradas).

bot_main.py — Código principal del bot en Telegram.

utils/ — Funciones auxiliares, preprocesamiento de texto, carga de modelos y predicciones.

datasets/ — Contiene los datos de entrenamiento (intents.json, train_data.csv).

requirements_bot.py — Dependencias necesarias del bot y las redes.

.env — Variables de entorno (TOKEN del bot y configuraciones).

README.md — Este archivo.

Instalación y configuración
 Requisitos previos

Asegúrate de tener instalado:

Python 3.10 o superior

pip (gestor de paquetes)

PyTorch

python-telegram-bot

numpy, pandas, torchtext

dotenv (para leer el TOKEN del bot)

 Clonar el repositorio
git clone https://github.com/tuusuario/UniHelperBot.git
cd UniHelperBot

 Crear entorno virtual
python -m venv venv
source venv/bin/activate      # Linux/Mac
venv\Scripts\activate         # Windows

 Instalar dependencias
pip install -r requirements_bot.py

 Configurar el bot

Crea un archivo .env en la raíz del proyecto y agrega:

TELEGRAM_TOKEN=tu_token_de_bot_aquí


Puedes obtener tu token creando un bot desde Telegram con @BotFather
.

 Ejecutar el bot
python bot_main.py


Una vez iniciado, abre Telegram y busca tu bot (por ejemplo, @UniHelperBot) para comenzar a interactuar 🤖

 Funcionalidades principales

Comprensión básica del lenguaje natural mediante redes neuronales.

Respuestas automáticas a preguntas frecuentes.

Enlaces directos a herramientas y licencias institucionales (MS365, MATLAB, GitHub Student Pack).

Guías rápidas sobre el uso de Google Classroom, Meet y Moodle.

Recordatorios y notificaciones personalizadas.

Soporte educativo 24/7 para estudiantes universitarios.
