<div align="center">

<h1>Peakly</h1>

<p><strong>La app de entrenamiento que no te roba tiempo.</strong></p>
<p>Registra sets en 1–2 taps. Sin fricción. Sin distracción. Solo entrenar.</p>

<p>
  <img src="https://img.shields.io/badge/Lanzamiento-1%20Jun%202026-56b8d4?style=flat-square&labelColor=0f172a" alt="Lanzamiento" />
  <img src="https://img.shields.io/badge/Stack-React%2019%20%2B%20Express%205-56b8d4?style=flat-square&labelColor=0f172a" alt="Stack principal" />
  <img src="https://img.shields.io/badge/Core-MongoDB%20%2B%20Zod-56b8d4?style=flat-square&labelColor=0f172a" alt="Core" />
</p>

<p>
  <a href="https://peaklyfit.com">Web</a> ·
  <a href="https://peaklyfit.com/waitlist">Waitlist</a> ·
  <a href="mailto:alexmico2006@gmail.com">Contacto</a>
</p>

</div>

---

## Tesis

Peakly se construye como el sistema operativo del entrenamiento para entrenadores, atletas y clientes. La prioridad no es otra app de fitness genérica — es resolver la operativa real: planificar, ejecutar y leer progreso desde un mismo sistema con fricción mínima.

> El software de entrenamiento no debería estorbar durante una sesión real.
> Debería acelerar decisiones, reducir fricción y aguantar uso diario.

## Dónde aporta valor

<table>
  <tr>
    <td width="33%" valign="top">
      <h3>Plan</h3>
      <p>Rutinas, bloques y asignación para que la programación no viva repartida entre mensajes, notas y hojas de cálculo.</p>
    </td>
    <td width="33%" valign="top">
      <h3>Log</h3>
      <p>Registro de sesiones pensado para tocar, confirmar y seguir entrenando sin fricción innecesaria.</p>
    </td>
    <td width="33%" valign="top">
      <h3>Read</h3>
      <p>Métricas y progreso con lectura operativa para decidir el siguiente paso sin ruido analítico.</p>
    </td>
  </tr>
</table>

## Para quién

- `Trainer` — crea rutinas, asigna clientes y revisa progreso con una operativa `desktop-first`.
- `Client` — recibe la planificación, registra sesiones con experiencia `mobile-first`.
- `Independent` — gestiona sus propios bloques y sesiones sin herramientas dispersas.

## Principios de producto

- `Mobile-first` para logging durante el entreno.
- `Desktop-first` para coach ops y gestión.
- Menos clicks, menos campos inútiles, más continuidad en flujos críticos.
- IA útil solo si ayuda; siempre desacoplada del core transaccional.

## Arquitectura

```text
peakly-web (React / Vite)
        |
        v
peakly-api (Express)
        |
        v
MongoDB / Mongoose
```

- `controllers → services → repositories → models`
- Validación de entrada con `Zod`
- Roles de dominio explícitos: `trainer`, `client`, `independent`

## Repositorios

| Repo | Descripción |
|------|-------------|
| [peakly-web](https://github.com/PeaklyFit/peakly-web) | Frontend React — landing, dashboard, workout logging |
| [peakly-api](https://github.com/PeaklyFit/peakly-api) | Backend Express — API REST, auth, gamificación, IA |

## Contacto

- Web: `https://peaklyfit.com`
- Waitlist: `https://peaklyfit.com/waitlist`
- General: `alexmico2006@gmail.com`

---

<div align="center">
<strong>Software para gente que entrena de verdad.</strong>
</div>
