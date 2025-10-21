## Instrucciones rápidas para agentes de IA

Estas instrucciones ayudan a los agentes a contribuir efectivamente en este repositorio mínimo.

- Contexto del proyecto: repositorio pequeño con una página estática `index.html` en la raíz. No hay frameworks ni configuraciones adicionales detectadas.

- Objetivo del agente: realizar cambios claros y limitados en archivos existentes, añadir contenido estático (HTML/CSS/JS) y crear documentación mínima bajo `.github/` cuando se solicite.

- Convenciones detectables:
  - Archivo principal: `index.html`. Mantén el DOCTYPE y la estructura básica (head/meta/body) cuando edites.
  - No hay package.json, build scripts ni carpetas de código. Evita añadir dependencias innecesarias.

- Comportamiento esperado del agente:
  1. Antes de editar, hacer lectura completa de los archivos relevantes (por ejemplo `index.html`) y resumir cambios propuestos en 1-2 líneas.
  2. Preferir cambios pequeños y verificables: añadir snippets, corregir meta tags, o crear archivos de documentación en `.github/`.
  3. No ejecutar o asumir build/test commands que no existan. Si el usuario pide añadir un build, proponer una lista de archivos a crear (p. ej. `package.json`) y pedir confirmación.

- Ejemplos concretos desde este repositorio:
  - Meta viewport: conservar la línea `<meta name="viewport" content="width=device-width, initial-scale=1.0">` cuando se mejore la plantilla.
  - Si se añade CSS o JS, crear carpetas `css/` y `js/` en la raíz y referenciarlas desde `index.html` con rutas relativas.

- Integraciones y límites:
  - No hay servicios externos detectados (APIs, bases de datos, CI). No agregar claves ni llamadas de red.
  - Si se necesita CI/automatización, proponer archivos (p. ej. `.github/workflows/ci.yml`) y pedir permiso antes de crearlos.

- Etiqueta de commits y mensajes:
  - Mensajes cortos, en español, que indiquen propósito: "docs: agregar instrucciones Copilot", "fix(html): corregir meta viewport".

- Qué preguntar al usuario cuando algo no es claro:
  - "¿Deseas agregar un sistema de construcción (npm, Maven) o mantener el proyecto como estático?"
  - "¿Puedo crear carpetas para CSS/JS si añado recursos estáticos?"

Mantén las contribuciones no intrusivas y confirma cambios estructurales antes de aplicarlos.
