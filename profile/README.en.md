<div align="center">

<a href="./README.md">
  <img src="https://img.shields.io/badge/ES-español-475569?style=for-the-badge&labelColor=0f172a" alt="Español" />
</a>
&nbsp;
<a href="./README.en.md">
  <img src="https://img.shields.io/badge/EN-active-56b8d4?style=for-the-badge&labelColor=0f172a" alt="English" />
</a>

<br /><br />

<h1>Strev</h1>

<p><strong>Training management software for freelance personal trainers.</strong></p>
<p>Log a set in 2 taps. Manage 30 clients without spreadsheets. Get paid with Stripe.</p>

<br />

<a href="https://strev.app">
  <img src="https://img.shields.io/badge/strev.app-visit-56b8d4?style=flat-square&labelColor=0f172a" alt="strev.app" />
</a>
<a href="https://strev.app/waitlist">
  <img src="https://img.shields.io/badge/Waitlist-open-22c55e?style=flat-square&labelColor=0f172a" alt="Waitlist open" />
</a>
<img src="https://img.shields.io/badge/Launch-Jun%201%202026-f59e0b?style=flat-square&labelColor=0f172a" alt="Launch date" />

</div>

---

## The problem

Freelance personal trainers managing 5–30 active clients run their business across three tools that don't talk to each other: **Excel** for routines and progress, **WhatsApp** for communication, and **handwritten notes** during sessions. The result is hours lost every week on admin work that creates zero value for clients.

Strev replaces that stack with a single platform built around the trainer's actual workflow.

---

## Who it's for

<table>
  <tr>
    <td width="50%" valign="top">
      <h3>Freelance personal trainer</h3>
      <p>Build routines, assign and personalise them per client without duplicating work. Monitor adherence and stagnation signals from the dashboard. Charge monthly or annual subscriptions. Export everything to Excel whenever you want.</p>
    </td>
    <td width="50%" valign="top">
      <h3>Independent athlete</h3>
      <p>Log sessions in 1–2 taps. See personal records instantly. Analyse technique with AI. No coach required, no friction, no lost data.</p>
    </td>
  </tr>
</table>

---

## The core loop

```
Open app → see next exercise → log set → PR badge → next exercise
```

Everything else — client management, payments, metrics, AI — is built to stay out of the way of this flow.

---

## Pricing

**Trainers**

| Plan | Price | Clients | AI / day |
|---|---|---|---|
| Free | €0 | 5 | 1 |
| Pro | €24 / mo | 20 | 5 |
| Master | €49 / mo | 50 | 10 |
| Elite | €79 / mo | 100 | 20 |

**Independent athletes:** Free (€0) · Athlete Pro (€9 / mo)

Annual discount: **2 months free** on all paid plans.

---

## Architecture

```
strev-web (React 19 · Vite · Tailwind · Framer Motion)
          ↓
strev-api (Express 5 · Node 22 · Zod · JWT)
          ↓
MongoDB Atlas · Cloudflare R2 · Upstash Redis
```

- Layers: `controllers → services → repositories → models`
- Explicit domain roles: `trainer` · `client` · `independent`
- Dark-first UI with toggle. No runtime theme dependencies.
- Async AI pipeline with BullMQ, isolated from the transactional core.

---

## Repositories

| Repo | Description |
|---|---|
| [strev-web](https://github.com/StrevFit/strev-web) | React frontend — landing, dashboard, workout session, metrics |
| [strev-api](https://github.com/StrevFit/strev-api) | Express backend — REST API, auth, gamification, AI, payments |

---

## Product status

- Auth, routines, sessions, clients, metrics, gamification ✅
- Stripe payments (Pro / Master / Elite / Athlete Pro) ✅
- Digital anamnesis, AI video analysis, public trainer profile ✅
- Monitoring: Sentry + BetterStack + Umami ✅
- **Public launch:** June 1, 2026

---

<div align="center">

**[strev.app](https://strev.app) · [hola@strev.app](mailto:hola@strev.app)**

*Built for people who actually train.*

</div>
