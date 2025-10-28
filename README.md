# AgenteRAG
Agente RAG desarrollado con Flowise y OpenAI GPT-4o-mini.  Ejemplo demostrativo que responde preguntas basadas en un documento real sobre Fake News.

# 🧠 Agente RAG sobre Fake News  
**Proyecto demostrativo desarrollado con Flowise y OpenAI GPT-4o-mini**
## 🌐 Agente

➡️ [**Ver demo del proyecto**](https://cartup90.github.io/AgenteRAG/)


---

## 📄 Descripción general

Este proyecto muestra el funcionamiento de un **agente RAG (Retrieval-Augmented Generation)** implementado con **Flowise**, integrado en una web desarrollada en HTML/CSS.

El agente fue configurado para responder preguntas sobre el documento *“Fake News e Inteligencia Artificial”* publicado por el Gobierno de la Ciudad de Buenos Aires.  
El objetivo es **demostrar cómo un modelo de lenguaje puede responder basándose en información real cargada por el usuario**, en lugar de usar únicamente conocimiento general.

> 💡 El tema de las fake news se utiliza únicamente con fines demostrativos.  
> El agente puede adaptarse fácilmente a cualquier otro documento o dominio (por ejemplo, catálogos de empresa, manuales técnicos, papers científicos, etc.).

---

## ⚙️ Tecnologías utilizadas

- 🧩 **Flowise** – para construir y desplegar el agente RAG visualmente.  
- 🤖 **OpenAI GPT-4o-mini** – modelo de lenguaje usado para la generación de respuestas.  
- 🔤 **Embeddings OpenAI** – para convertir fragmentos de texto en vectores semánticos.  
- 💾 **Vector Store** – almacenamiento temporal de los vectores para búsqueda contextual.  
- 🌐 **HTML + CSS (vanilla)** – diseño de la interfaz web de demostración.  
- ⚡ **Flowise Embed** – para integrar el chatbot en el sitio web.

---

## 🧱 Flujo de trabajo del agente

El pipeline RAG implementado en Flowise sigue la siguiente estructura:

1. **File Loader** – carga el documento PDF “B8_Fake news.pdf”.  
2. **Text Splitter** – divide el texto en fragmentos de ~700 caracteres con solapamiento.  
3. **OpenAI Embeddings** – convierte cada fragmento en un vector numérico.  
4. **Vector Store** – almacena los embeddings para búsquedas semánticas.  
5. **Conversational QA Chain** – combina la búsqueda contextual con GPT-4o-mini.  
6. **Chatbot UI (Flowise Embed)** – interfaz que permite la interacción del usuario.

---

## 🔍 Modelo y configuración

| Parámetro | Valor | Descripción |
|------------|--------|-------------|
| **Modelo** | `gpt-4o-mini` | Versión optimizada de GPT-4 para respuesta rápida. |
| **Temperatura** | `0.2` | Reduce la creatividad para priorizar exactitud y coherencia. |
| **Modo** | Conversational QA | Recupera contexto relevante antes de generar respuesta. |

---

## 💡 Casos de uso de un agente RAG

Los agentes RAG son ideales para proyectos donde se necesita **buscar información en documentos propios y generar respuestas contextuales**.  
Algunos ejemplos prácticos:

- 🏢 **Soporte al cliente:** responde preguntas sobre políticas o manuales internos.  
- 🛒 **Catálogos empresariales:** permite búsquedas inteligentes entre fichas de producto.  
- 🎓 **Educación:** tutorías basadas en materiales cargados por el docente.  
- 🧾 **Investigación:** resumir papers o responder consultas sobre informes extensos.  
- ⚖️ **Ámbito legal:** consultas rápidas sobre cláusulas o contratos cargados al sistema.

---

