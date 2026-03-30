<div align="center">

<a href="./README.md">
  <img src="https://img.shields.io/badge/ES-1f2937?style=for-the-badge&labelColor=0f172a&color=1f2937" alt="README en Espanol" />
</a>
<a href="./README.en.md">
  <img src="https://img.shields.io/badge/EN-56b8d4?style=for-the-badge&labelColor=0f172a&color=56b8d4" alt="README in English" />
</a>

<h1>Liftnotch</h1>

<p><strong>Software for serious training.</strong></p>
<p>Plan better. Log faster. Read progress without noise.</p>

<p>
  <img src="https://img.shields.io/badge/Beta-Open-56b8d4?style=flat-square&labelColor=0f172a" alt="Beta" />
  <img src="https://img.shields.io/badge/Stack-React%2019%20%2B%20Express%205-56b8d4?style=flat-square&labelColor=0f172a" alt="Primary stack" />
  <img src="https://img.shields.io/badge/Core-MongoDB%20%2B%20Zod-56b8d4?style=flat-square&labelColor=0f172a" alt="Core" />
</p>

<p>
  <a href="https://liftnotch.com">Website</a> ·
  <a href="https://liftnotch.com/waitlist">Waitlist</a> ·
  <a href="mailto:alexmico2006@gmail.com">Contact</a>
</p>

</div>

---

## Thesis

Liftnotch is being built as a `training operating system` for coaches, clients, and independent athletes. The goal is not to ship another generic fitness app. The goal is to improve real training operations: planning better, logging without friction, and turning data into usable decisions.

Most of the application code remains private while the product evolves. This public profile exists to share product direction, engineering principles, and ways to connect with the team.

> Training software should not get in the way during a real session.
> It should reduce friction, speed up decisions, and survive daily use.

## Where It Creates Value

<table>
  <tr>
    <td width="33%" valign="top">
      <h3>Plan</h3>
      <p>Routines, blocks, and assignment flows so programming does not live across messages, notes, and spreadsheets.</p>
    </td>
    <td width="33%" valign="top">
      <h3>Log</h3>
      <p>Session logging built for the training moment: tap, confirm, move on, and keep the workout going.</p>
    </td>
    <td width="33%" valign="top">
      <h3>Read</h3>
      <p>Metrics and progress views designed for operational clarity instead of analytical noise.</p>
    </td>
  </tr>
</table>

## Who It Is For

- `Trainer`: builds routines, assigns clients, and reviews progress through `desktop-first` operations.
- `Client`: receives programming, logs sessions, and reports context through a `mobile-first` experience.
- `Independent`: manages personal blocks and sessions without relying on scattered tools.

## Product Principles

- `Desktop-first` for coach ops and management work.
- `Mobile-first` for session logging during training.
- Fewer clicks, fewer useless fields, more continuity in critical flows.
- AI only where it helps, always isolated from the transactional core.

## Product Status

- Role-based signup and login.
- Routine creation, editing, and assignment.
- Session logging with sets, reps, load, and notes.
- Dashboards with exercise progress and weekly metrics.
- Foundation ready for premium modules and AI-assisted workflows.

## Architecture

```text
web (React / Vite)
        |
        v
api (Express)
        |
        v
db (MongoDB / Mongoose)
```

### System principles

- `controllers -> services -> repositories -> models`
- input validation with `Zod`
- explicit domain roles: `trainer`, `client`, `independent`
- frontend designed for product use, not just polished demos
- AI modules isolated from the core

## What We Share Here

This public profile is used to share:

- product thesis
- architecture decisions
- public supporting repositories when relevant
- entry points for technical or strategic collaboration

## Contact

- Website: `https://liftnotch.com`
- Waitlist: `https://liftnotch.com/waitlist`
- General: `alexmico2006@gmail.com`
- Partnerships: `alexmico2006@gmail.com`

---

<div align="center">

<strong>Liftnotch is building software for people who actually train.</strong>

</div>
