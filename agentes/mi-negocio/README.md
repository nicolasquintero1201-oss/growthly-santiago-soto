Tus archivos propios (agentes que modificaste, notas, outputs). Limitless nunca toca esta carpeta.

## Memoria por agente

Esta carpeta tiene tres subcarpetas espejo, cada una dividida por agente (usando el mismo slug que en `.agentes-index.json`, ej. `arquitecto-oferta`, `agente-guiones-reels`):

```
mi-negocio/
├── outputs/<agente>/      — todo lo que ese agente entregó, con fecha. No se borra nada.
├── templates/<agente>/    — solo lo aprobado, copiado desde outputs/ con una nota de por qué funcionó.
└── feedback/<agente>/     — lo que se corrigió: qué se pidió → qué se entregó → qué se corrigió → por qué.
```

Como este negocio tiene un solo "cliente" (vos), no hay una capa de cliente arriba — cada agente tiene una línea directa en las tres carpetas.

### Ritual (seguirlo siempre que se use un agente)

1. **Antes de crear algo** con el agente X: leer `feedback/X/*` + `templates/X/*` + `CONTEXTO.md` (y la sección [COMPLETÁ ESTO] del agente).
2. **Crear** → guardar en `outputs/X/AAAA-MM-DD-descripcion.md`.
3. **Preguntar**: "¿quedó bien o hay algo que ajustar?"
4. a) Si se aprueba → copiar a `templates/X/` + agregar una nota arriba del archivo explicando por qué funcionó.
   b) Si se corrige → guardar en `feedback/X/AAAA-MM-DD-descripcion.md` con el patrón fijo: **qué se pidió → qué se entregó → qué se corrigió → por qué**.

Esto hace que cada agente acumule su propio historial de aciertos y errores, aislado del de los demás, y que la próxima vez que se le pida algo parecido, arranque mejor informado en vez de repetir el mismo error.
