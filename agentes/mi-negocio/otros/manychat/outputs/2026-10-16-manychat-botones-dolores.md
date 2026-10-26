# ManyChat — Botones por dolor (comentario → DM) — Santiago Soto

**Fecha**: 2026-10-16 (v5, aprobada por Nicolás)
**Pedido**: mejorar los botones del flujo de ManyChat de Santiago para que toquen
dolores de su avatar y, por cada botón, un mensaje con 2–3 problemas para que el
lead responda cuál le pasa y se abra conversación.

**Base**: avatar N2 y mapa de dolores (`clientes/santiago-soto/contexto/avatar-n2-santiago.md`),
dolores aprobados ("modelar videos virales", "tener una audiencia grande") y
narrativa (todos suenan igual → los comparan por precio).

Avatar: experto (coach, consultor, servicios) que vende info (mentoría/curso),
publica hace 3–12 meses, tuvo ventas sueltas, siente que su contenido se parece
al de todos y no convierte su audiencia en alumnos.

---

## Mensaje 1

> Buenas, como vas? Apreta el botón para recibir el recurso:

## Mensaje 2 (con botones)

> por cierto, tengo una carpeta llena de recursos para ayudarte a vender tu
> mentoría o curso con tu marca personal. cuéntame qué quieres mejorar y te la mando 👇

Botones (máx. 20 caracteres en Instagram):
1. `Más clientes` — leads: poco flujo + descalificados (dolores 2 y 4)
2. `Cobrar más caro` — dolor 4
3. `Ser referente` — dolor 1 (psicográfico: "referente auténtico, no uno más")

---

## Respuesta — Más clientes

> okey, normalmente pasa una de estas 2:
>
> 1. nadie responde tus CTAs
> 2. te llegan leads SUPER descalificados
>
> cuál te está pasando?

## Respuesta — Cobrar más caro

> okey, eso suele venir de 3 lados:
>
> 1. te llegan leads que no pueden pagar tu programa
> 2. te da miedo subir el precio porque sientes que no te van a comprar
> 3. te comparan con otros cursos y terminas compitiendo por precio
>
> cuál es el tuyo?

## Respuesta — Ser referente

> buenísimo, lo que normalmente frena eso es una de estas:
>
> 1. tu contenido es igual al de tu competencia
> 2. modelas videos virales
> 3. no te muestras como el experto que eres
>
> cuál te identifica más?

---

## Notas de implementación
- Guardar el botón elegido en un tag / custom field (`dolor_clientes`,
  `dolor_precio`, `dolor_referente`).
- Cuando el lead responda, seguir la conversación a mano con una pregunta
  anclada en lo que dijo. Si responde "las 2/las 3", preguntar cuál le pesa más.

## Pendiente
- "Cobrar más caro": el punto 1 (leads que no pueden pagar) se pisa con el punto
  2 de "Más clientes". Propuesta sin confirmar: dejarlo en 2 problemas (miedo a
  subir el precio + comparación con otros cursos).
- Voz de Santiago sin documentar.
