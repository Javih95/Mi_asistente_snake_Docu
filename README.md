# Snake Assistant - Asistente Conversacional Inteligente

![Python](https://img.shields.io/badge/Python-3.14-blue)
![Tkinter](https://img.shields.io/badge/Tkinter-UI-green)
![SQLite](https://img.shields.io/badge/SQLite-DB-orange)
![Gemini API](https://img.shields.io/badge/Gemini-API-purple)

**Snake** es una aplicación de escritorio en Python que funciona como asistente conversacional inteligente. Permite interactuar mediante texto y voz, gestionar múltiples chats, guardar historial de conversaciones y descargar respuestas. Está diseñada con una interfaz moderna en modo oscuro con detalles en violeta, inspirada en aplicaciones de mensajería.

---

## Características principales

- Gestión de múltiples chats con creación, selección y eliminación.
- Interfaz gráfica interactiva con burbujas de chat diferenciadas por usuario y asistente.
- Entrada de texto con ajuste automático de altura y scroll dinámico.
- Respuestas generadas usando el modelo **Gemini 2.5** mediante la API de Google.
- Soporte de entrada por voz (grabación y transcripción).
- Guardado y recuperación de historial de conversaciones usando SQLite.
- Copiar y descargar respuestas del asistente en archivos de texto.
- Interfaz responsive que se adapta a diferentes tamaños de ventana.
- Manejo de errores de la API y mensajes amigables para saturación del modelo.

---

## Tecnologías utilizadas

- **Python 3.14**: Lenguaje principal del proyecto.
- **Tkinter**: Librería para la interfaz gráfica de escritorio.
- **SQLite**: Base de datos local para almacenar chats y mensajes.
- **Threading**: Para ejecución asíncrona de llamadas a la API y grabación de voz sin bloquear la UI.
- **Google Gemini API**: Para generación de respuestas del asistente.
- **ttk**: Estilos modernos de widgets dentro de Tkinter.
- **speech_recognition**: Integración básica para entrada por voz (grabación y transcripción).
- **OS / File Dialog**: Manejo de archivos locales para guardar respuestas.
- **Datetime**: Para timestamp de mensajes y archivos descargados.

---

## Estructura del proyecto
Mi_asistente_snake/
│
├─ backend/
│ ├─ cliente_gemini.py # Funciones para interactuar con la API de Gemini
│ ├─ voz.py # Funciones para grabación de audio y transcripción
| ├─ logica.py # Funciones para manejo del chat
│ └─ guardarArchivo.py # Funciones auxiliares para guardar archivos
│
├─ data/
│ ├─ db.py # Gestión de SQLite (crear chat, guardar mensajes, borrar)
│ └─ history.db # Base de datos SQLite
│
├─ ui/
│ └─ asistente_ui.py # Interfaz gráfica con Tkinter
│
├─ main.py # Punto de entrada de la aplicación
└─ requirements.txt # Dependencias del proyecto
## Mejoras planeadas

- Modo de chat “rol definido” donde el asistente se comporte según un system prompt predefinido.

- Integración de un historial global con búsqueda y filtros.
## Demostración
<iframe width="560" height="315" src="https://www.youtube.com/embed/7EG01CCD1PA?si=7gwhoNr6iiKS9odb" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
## Licencia

MIT License © 2025 - Javier Aguirre
