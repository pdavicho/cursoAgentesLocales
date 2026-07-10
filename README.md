# 🤖 Curso: Agentes de IA Locales

Sitio del curso (5 días × 2 horas, apto para modalidad asíncrona) para crear agentes de IA **sin programar**: 100% local con Ollama + AnythingLLM, más talleres bonus en la nube (Zapier y MindStudio). ISTER 2026.

## Estructura

```
index.html                  → Portada del curso
assets/curso.css            → Estilos compartidos (portada, labs y manuales)
dia1/  slides.html + lab.html → Qué es un agente · instalar Ollama, chat sin internet
dia2/  slides.html + lab.html → Instrucciones y memoria (RAG) · AnythingLLM con tus PDFs
dia3/  slides.html + lab.html → Herramientas: @agent, web, archivos · primer agente completo
dia4/  slides.html + lab.html → Visión (fotos→datos), leer páginas, gráficos, memoria
dia5/  slides.html            → Multi-agente, ética, quiz final y graduación
dia5/  oficina.html           → 🏢 La Oficina de Agentes: 4 agentes colaborando con el
                                Ollama local del estudiante (con modo demo sin Ollama)
dia5/  proyecto.html          → Proyecto final: ficha, rúbrica /10 y entrega asíncrona
talleres/zapier.html          → Bonus ☁️: agente analista de correos → Telegram
talleres/mindstudio.html      → Bonus ☁️: agente analizador de hojas de vida
```

## La Oficina de Agentes

`dia5/oficina.html` llama a la API local de Ollama (`http://localhost:11434`) desde el navegador. Servida desde GitHub Pages, Ollama bloqueará la llamada por CORS: la propia página explica al estudiante cómo autorizarla (`setx OLLAMA_ORIGINS "*"` + reiniciar Ollama) o usar el modo demo 🎬, que no requiere nada.

## Publicar en GitHub Pages

1. Crear un repositorio en GitHub (ej. `curso-agentes`) y subir este contenido a la rama `main`.
2. En el repo: **Settings → Pages → Source: Deploy from a branch → Branch: `main` / `(root)`** → Save.
3. El sitio queda en `https://<usuario>.github.io/curso-agentes/`.

## Ver en local

Basta con abrir `index.html` en el navegador (no requiere servidor). Las slides se navegan con las flechas ← →, barra espaciadora, botones en pantalla o deslizando en táctil.

## Notas de diseño

- Todo autocontenido: sin CDNs ni librerías externas, para que funcione proyectando sin internet.
- El progreso de los checklists de los labs se guarda en `localStorage` del navegador de cada estudiante.
- Los manuales tienen estilos de impresión (`Ctrl+P` produce una versión limpia en blanco).
