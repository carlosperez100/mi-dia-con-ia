# Mi Día con IA

Dashboard de productividad personal en **un solo `index.html`** — HTML + CSS + JS embebidos, sin dependencias, sin login, sin backend. Listo para GitHub Pages.

**Demo:** https://carlosperez100.github.io/mi-dia-con-ia/

## Qué incluye

- Vista **Hoy**: tarjetas KPI con tendencia de 7 días + línea de tiempo del día por horas (bloques con duración e hitos puntuales) + insight generado localmente con reglas (sin backend).
- Vista **Semana**: barras apiladas por día, horas de foco por día y comparación por tipo de actividad — todo en SVG puro, sin librerías.
- Toggle **Ingeniero ↔ Contador**: cambia etiquetas, iconos y datos (commits/PRs/reviews/tickets ↔ asientos/facturas/conciliaciones/cierres).
- Modo **oscuro/claro** con la convención visual **GEMSES**: edición "Ónix Marino" (negro + esmeralda neón + aqua + oro) y edición clara de procesos. Paleta de series validada para daltonismo (protán/deután/tritán) en ambos modos.
- Responsive mobile-first, preferencias guardadas en `localStorage`.

## Cómo cargar tus datos

Edita la constante `SEED` al inicio del `<script>` en `index.html`:

- `hoy.eventos`: el día detallado — con `fin` es un bloque con duración; sin `fin` es un hito puntual (`cantidad` opcional). Los KPI de hoy se calculan solos desde estos eventos.
- `semana`: 6 días con totales + la fila de hoy (auto-calculada).

© CIIDEG · Modelo GEMSES — Mg. Carlos Pérez Pérez
