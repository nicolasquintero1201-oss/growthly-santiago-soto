# Instrucciones para Claude Code en este repo

Este repo es la copia de los agentes de Limitless para tu negocio.

1. **Nunca edites ni crees archivos dentro de `agentes/` ni `.claude/skills/`.** Limitless los gestiona y los sobrescribe en cada `git pull upstream main`; cualquier cambio ahí se pierde. Si el usuario quiere modificar un agente, copiá ese `.md` a `mi-negocio/` y editá la copia ahí.
2. **Todo lo que generes** (el resultado de correr un agente, borradores, notas) guardalo dentro de `mi-negocio/`, no en la raíz del repo ni dentro de `agentes/`. Si no hay una carpeta clara para el tema, creá una nueva subcarpeta en `mi-negocio/`.
3. Si la sección **[COMPLETÁ ESTO]** de un agente está vacía, leé `CONTEXTO.md` primero; si falta el dato ahí, preguntaselo al usuario antes de asumir nada.
4. No edites `CONTEXTO.md` salvo que el usuario te lo pida explícitamente — es la fuente de verdad sobre su negocio.
5. **Memoria por agente.** `mi-negocio/` tiene tres carpetas espejo —`outputs/`, `templates/`, `feedback/`— cada una con una subcarpeta por agente (slug igual al de `.agentes-index.json`). Antes de usar un agente X, leé `mi-negocio/feedback/X/*` y `mi-negocio/templates/X/*` para no repetir errores ya corregidos y para modelar sobre lo que ya funcionó con ese agente. Después de entregar algo, guardalo en `mi-negocio/outputs/X/AAAA-MM-DD-descripcion.md` y preguntale al usuario si quedó bien o hay que ajustar algo; si se aprueba copialo a `templates/X/` con una nota de por qué funcionó, si se corrige guardá la corrección en `feedback/X/` con el patrón qué se pidió → qué se entregó → qué se corrigió → por qué. Detalle del ritual en `mi-negocio/README.md`.
