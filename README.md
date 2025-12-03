# 🤖 AI Autonomous Research Agent

![Python](https://img.shields.io/badge/Python-3.12-blue?style=for-the-badge&logo=python&logoColor=white)
![LangChain](https://img.shields.io/badge/LangChain-v0.2-green?style=for-the-badge&logo=langchain&logoColor=white)
![OpenAI](https://img.shields.io/badge/AI-GPT--4-412991?style=for-the-badge&logo=openai&logoColor=white)

> **Un agente inteligente capaz de investigar, razonar y generar informes estructurados de forma autónoma.**

---

## 💡 ¿Qué hace este proyecto?

Este no es un simple chatbot. Es un sistema de **Agentes Autónomos** diseñado para realizar tareas de investigación completas sin supervisión humana.

El agente recibe un tema (ej: *"Investiga sobre el CEO de OpenAI"*) y sigue su propio flujo de pensamiento:

1.  🧠 **Razona:** Decide qué información le falta y dónde buscarla.
2.  🔎 **Investiga:** Navega por internet en tiempo real usando **DuckDuckGo**.
3.  📚 **Contrasta:** Consulta **Wikipedia** para obtener contextos biográficos y definiciones precisas.
4.  💾 **Persiste:** Guarda automáticamente los hallazgos en archivos de texto locales.
5.  ✅ **Estructura:** Entrega un resumen final en formato JSON limpio y validado.

---

## 🛠️ Tecnologías & Arquitectura

El proyecto combina las herramientas más potentes del ecosistema de IA actual:

| Tecnología | Función en el Proyecto |
| :--- | :--- |
| **🐍 Python 3.12** | Lenguaje base del desarrollo. |
| **🦜🔗 LangChain** | Orquestación del agente y gestión de herramientas (Tool Calling). |
| **🧠 GPT-4o** | El "cerebro" que toma decisiones y procesa el lenguaje natural. |
| **🛡️ Pydantic** | Validación estricta de datos para asegurar salidas sin errores. |
| **🌐 DuckDuckGo & Wiki API** | Herramientas externas que el agente aprende a usar. |

---

## 📸 Flujo de Trabajo Real

El agente no sigue un script fijo; **toma decisiones en tiempo real**:

```mermaid
graph TD
    A[Usuario pide información] --> B{Agente GPT-4}
    B -->|Necesito datos actuales| C[🔍 Herramienta: DuckDuckGo]
    B -->|Necesito biografía| D[📖 Herramienta: Wikipedia]
    C --> B
    D --> B
    B -->|Tengo suficiente info| E[💾 Herramienta: Guardar Archivo]
    E --> F[✅ Respuesta Final JSON]
```

---

### 🚀 Estado del Proyecto
Este proyecto es funcional y demuestra la capacidad de integrar **LLMs con herramientas externas** para resolver problemas del mundo real.

---
*Developed by Vanessa Larrosa*
