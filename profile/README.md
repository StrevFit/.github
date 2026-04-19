<div align="center">

<a href="./README.md">
  <img src="https://img.shields.io/badge/ES-activo-56b8d4?style=for-the-badge&labelColor=0f172a" alt="Español" />
</a>
&nbsp;
<a href="./README.en.md">
  <img src="https://img.shields.io/badge/EN-english-475569?style=for-the-badge&labelColor=0f172a" alt="English" />
</a>

<br /><br />

<h1>Strev</h1>

<p><strong>Software de gestión para entrenadores personales freelance.</strong></p>
<p>Registra un set en 2 taps. Gestiona 30 clientes sin Excel ni WhatsApp. Cobra con Stripe.</p>

<br />

<a href="https://strev.app">
  <img src="https://img.shields.io/badge/strev.app-visitar-56b8d4?style=flat-square&labelColor=0f172a" alt="strev.app" />
</a>
<a href="https://strev.app/waitlist">
  <img src="https://img.shields.io/badge/Lista%20de%20espera-abierta-22c55e?style=flat-square&labelColor=0f172a" alt="Waitlist abierta" />
</a>
<img src="https://img.shields.io/badge/Lanzamiento-1%20Jun%202026-f59e0b?style=flat-square&labelColor=0f172a" alt="Lanzamiento" />

</div>

---

## El problema

Los entrenadores personales freelance con 5–30 clientes activos gestionan su negocio con tres herramientas que no hablan entre sí: **Excel** para rutinas y progreso, **WhatsApp** para comunicación, y **notas en papel** durante el entrenamiento. El resultado es horas perdidas cada semana en tareas que no aportan valor al cliente.

Strev reemplaza ese stack con una sola plataforma optimizada para el flujo real del entrenador.

---

## Para quién es

<table>
  <tr>
    <td width="50%" valign="top">
      <h3>Entrenador personal freelance</h3>
      <p>Crea rutinas, las asigna y personaliza por cliente sin duplicar trabajo. Revisa adherencia y señales de estancamiento desde el dashboard. Cobra suscripciones mensuales o anuales. Exporta todo a Excel si quiere salir.</p>
    </td>
    <td width="50%" valign="top">
      <h3>Atleta independiente</h3>
      <p>Registra sesiones en 1–2 taps. Ve sus récords personales en el acto. Analiza su técnica con IA. Sin entrenador, sin fricción, sin perder datos.</p>
    </td>
  </tr>
</table>

---

## El core loop

```
Abrir app → ver siguiente ejercicio → registrar set → PR badge → siguiente
```

Todo lo demás — gestión, pagos, métricas, IA — está construido para no añadir fricción a este flujo.

---

## Planes

**Entrenadores**

| Plan | Precio | Clientes | IA / día |
|---|---|---|---|
| Free | €0 | 5 | 1 |
| Pro | €24 / mes | 20 | 5 |
| Master | €49 / mes | 50 | 10 |
| Elite | €79 / mes | 100 | 20 |

**Atletas independientes:** Free (€0) · Athlete Pro (€9 / mes)

Descuento anual: **2 meses gratis** en todos los planes de pago.

---

## Arquitectura

```
strev-web (React 19 · Vite · Tailwind · Framer Motion)
          ↓
strev-api (Express 5 · Node 22 · Zod · JWT)
          ↓
MongoDB Atlas · Cloudflare R2 · Upstash Redis
```

- Capas: `controllers → services → repositories → models`
- Roles explícitos: `trainer` · `client` · `independent`
- Dark-first con toggle. Sin dependencias de tema en tiempo de ejecución.
- IA asíncrona con BullMQ, desacoplada del core transaccional.

---

## Repositorios

| Repo | Descripción |
|---|---|
| [strev-web](https://github.com/StrevFit/strev-web) | Frontend React — landing, dashboard, workout session, métricas |
| [strev-api](https://github.com/StrevFit/strev-api) | Backend Express — API REST, auth, gamificación, IA, pagos |

---

## Estado del producto

- Auth, rutinas, sesiones, clientes, métricas, gamificación ✅
- Pagos Stripe (Pro / Master / Elite / Athlete Pro) ✅
- Anamnesis digital, análisis IA de vídeo, perfil público del entrenador ✅
- Monitorización: Sentry + BetterStack + Umami ✅
- **Lanzamiento público:** 1 de junio de 2026

---

<div align="center">

**[strev.app](https://strev.app) · [hola@strev.app](mailto:hola@strev.app)**

*Construido para la gente que entrena de verdad.*

</div>
