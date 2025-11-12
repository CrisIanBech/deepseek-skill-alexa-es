# 🤖 Alexa con Deepseek API

Bienvenido al proyecto **Alexa con Deepseek**, una adaptación del repositorio [skill-alexa-chatgpt4](https://github.com/alexandremendoncaalvaro/skill-alexa-chatgpt4), ahora utilizando la **API de Deepseek** para dar voz a la inteligencia artificial.

---

## 📚 Sobre el Proyecto

Este proyecto es un **fork adaptado** del repositorio original [skill-alexa-chatgpt4](https://github.com/alexandremendoncaalvaro/skill-alexa-chatgpt4), diseñado específicamente para facilitar la importación y configuración como skill de Alexa.

### ¿Qué se ha adaptado?

Este fork incluye las siguientes mejoras y adaptaciones:

- ✅ **Configuración completa para Español de México (es-MX)**: Todos los mensajes, prompts y modelos de interacción están traducidos y adaptados
- ✅ **Estructura lista para importar**: Los archivos están organizados y configurados para importarse directamente en el Developer Console de Alexa
- ✅ **Integración con Deepseek API**: Adaptado para utilizar el modelo `deepseek-chat` en lugar de ChatGPT
- ✅ **Validaciones mejoradas**: Manejo de errores y casos edge mejorados para una mejor experiencia de usuario

El objetivo principal de este fork es proporcionar una versión **lista para usar** que pueda importarse fácilmente sin necesidad de realizar modificaciones adicionales en la estructura del proyecto.

---

## 🎥 Tutorial en Vídeo

¿Quieres ver el paso a paso de cómo integrar Deepseek en tu Alexa?

📺 Consulta el video completo en YouTube en el Canal Café con bug:  
👉 [link del video en youtube](https://youtu.be/lhqpAaIosmI)

---

## 🔗 Repositorio Original

Este proyecto es un fork y adaptación del repositorio original:

🔗 https://github.com/mrtrycatch/deepseek-skill-alexa

**Nota**: Este fork ha sido adaptado específicamente para facilitar la importación como skill de Alexa en Español de México, con todas las configuraciones necesarias ya implementadas.

---

## ✨ Tecnologías Utilizadas

- **Alexa Skills Kit (ASK)**
- **Python 3**
- **AWS Lambda**
- **Deepseek API**

---

## 🌎 Configuración de Idioma

Este proyecto está configurado para **Español de México (es-MX)**. Todos los mensajes y el modelo de interacción están traducidos y adaptados para este idioma.

### Archivos de Configuración

- `interactionModels/custom/es-MX.json` - Modelo de interacción en español de México
- `skill.json` - Configuración del skill con locale es-MX
- `lambda/lambda_function.py` - Código Python con mensajes en español

---

## 🚀 Configuración e Importación

Este proyecto está diseñado para ser **fácilmente importable** como skill de Alexa. Sigue estos pasos:

### Paso 1: Configurar API Key

1. Edita el archivo `lambda/lambda_function.py` y configura tu API key de Deepseek:
   ```python
   openai_api_key = "TU-API-KEY-DEEPSEEK"
   ```

### Paso 2: Desplegar en AWS Lambda

2. Crea un paquete de despliegue con el código y las dependencias
3. Despliega la función Lambda en AWS
4. Copia el ARN de la función Lambda

### Paso 3: Importar en Alexa Developer Console

5. Ve al [Alexa Developer Console](https://developer.amazon.com/alexa/console/ask)
6. Crea un nuevo skill o importa desde `skill.json`
7. En la sección de **Build**, importa el modelo de interacción desde `interactionModels/custom/es-MX.json`
8. Configura el endpoint de Lambda con el ARN copiado en el paso 2

### Paso 4: Probar

9. Usa el simulador de Alexa o un dispositivo físico para probar:
   - Di: **"Alexa, abre deepseek"**
   - Luego haz cualquier pregunta

**¡Listo!** El skill está configurado y listo para usar en Español de México.

---

## 📄 Licencia

Este proyecto sigue los términos de la MIT License
