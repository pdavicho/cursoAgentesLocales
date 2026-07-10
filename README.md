# 🤖 Curso: Agentes de IA Locales

Sitio del curso (5 días × 2 horas) para crear agentes de IA **sin programar**: núcleo 100% local (Ollama + AnythingLLM) más talleres en la nube (Zapier y MindStudio). ISTER 2026.

## Estructura

```
index.html                  → Portada del curso
assets/curso.css            → Estilos compartidos (portada, labs y manuales)
dia1/slides.html            → Slides interactivas Día 1 (autocontenidas, funcionan sin internet)
dia1/lab.html               → Lab Día 1: instalar Ollama y chatear sin internet
talleres/zapier.html        → Manual Día 4: agente analista de correos → Telegram
talleres/mindstudio.html    → Manual Día 5: agente analizador de hojas de vida
```

Pendientes: Día 2 (AnythingLLM + RAG), Día 3 (agente local con habilidades), cierre/proyecto final con rúbrica.

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
