<div align="center">

<a href="./README.md">
  <img src="https://img.shields.io/badge/ES-1f2937?style=for-the-badge&labelColor=0f172a&color=1f2937" alt="README en Espanol" />
</a>
<a href="./README.en.md">
  <img src="https://img.shields.io/badge/EN-56b8d4?style=for-the-badge&labelColor=0f172a&color=56b8d4" alt="README in English" />
</a>

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0a0a0a,60:141b2d,100:56b8d4&height=180&section=header&text=Trainity&fontColor=ffffff&fontSize=54&fontAlignY=40&desc=Training%20Operating%20System%20for%20Coaches%20and%20Athletes&descAlignY=66" alt="Trainity banner" />

### Product infrastructure for serious training

<p>
  <img src="https://img.shields.io/badge/Beta-Open-56b8d4?style=flat-square&labelColor=0f172a" alt="Beta" />
  <img src="https://img.shields.io/badge/Frontend-React%20%2B%20Vite-56b8d4?style=flat-square&labelColor=0f172a" alt="Frontend" />
  <img src="https://img.shields.io/badge/Backend-Express%20%2B%20MongoDB-56b8d4?style=flat-square&labelColor=0f172a" alt="Backend" />
  <img src="https://img.shields.io/badge/Contracts-Zod-56b8d4?style=flat-square&labelColor=0f172a" alt="Contracts" />
  <img src="https://img.shields.io/badge/Mode-Dark--first-56b8d4?style=flat-square&labelColor=0f172a" alt="Dark first" />
  <img src="https://img.shields.io/badge/Focus-Mobile%20Logging-56b8d4?style=flat-square&labelColor=0f172a" alt="Mobile logging" />
</p>

</div>

---

## Thesis

Trainity is being built as a training operating system for coaches and athletes who need speed, operational clarity, and a premium product experience. The focus is not "fitness content." The focus is execution: planning better, logging without friction, and turning training data into usable decisions.

> Most application code remains private while the product is under active development. This public profile is focused on architecture, product direction, and ways to engage with the team.

## What We Are Building

<table>
  <tr>
    <td width="50%" valign="top">
      <h3>Coach Ops</h3>
      <p>Routines, assignments, follow-up, and daily operations for coaches managing real athlete progress, not scattered spreadsheets.</p>
    </td>
    <td width="50%" valign="top">
      <h3>Session Logging</h3>
      <p>Mobile-first session logging for real workouts, optimized for speed, context, and minimum friction during training.</p>
    </td>
  </tr>
  <tr>
    <td width="50%" valign="top">
      <h3>Metrics</h3>
      <p>Clear metrics for adherence, volume, progression, and operational visibility across a training block.</p>
    </td>
    <td width="50%" valign="top">
      <h3>AI Modules</h3>
      <p>AI capabilities kept separate from the transactional core for video review, technical feedback, and coach-assisted flows.</p>
    </td>
  </tr>
</table>

## Architecture

```text
web (React / Vite)
        |
        v
api (Express)
        |
        v
db (MongoDB)
```

### System principles

- `controllers -> services -> repositories -> models`
- Input validation with `Zod`
- Clear domain roles: `trainer`, `client`, `independent`
- Mobile-first logging, desktop-first trainer operations
- AI modules isolated from the transactional core

## Engineering Thesis

<table>
  <tr>
    <td width="33%" valign="top">
      <h3>Speed</h3>
      <p>We reduce friction in critical flows. The product has to feel fast during a real session, not only in a demo.</p>
    </td>
    <td width="33%" valign="top">
      <h3>Clarity</h3>
      <p>Clear contracts, explicit ownership, and an interface that does not ask users to parse noise.</p>
    </td>
    <td width="33%" valign="top">
      <h3>Durability</h3>
      <p>Architecture that is clean enough to evolve without rebuilding the product every few weeks.</p>
    </td>
  </tr>
</table>

## For Technical Talent

We care about people who think about product and systems at the same time.

- Engineering with product and UX judgment, not feature output alone.
- Clean backend boundaries, robust contracts, and real ownership.
- Frontend work with hierarchy, intention, and perceived performance.
- Interest in internal tooling, AI-assisted workflows, and execution quality.

## For Partners And Investors

Trainity is not trying to compete on content volume. The bet is to build product infrastructure for serious training.

- Coach operations with a focus on daily adoption.
- Mobile experience designed for the actual training moment.
- Technical foundation prepared for premium modules and AI-assisted workflows.
- Product direction driven by systems thinking, not interface polish alone.

## Community

We are opening Trainity's public profile to start sharing the direction of the company and create clear entry points for collaboration.

- `Waitlist`: `https://placeholder.trainity.dev/waitlist`
- `Website`: `https://placeholder.trainity.dev`
- `Partnerships`: `alexmico2006@gmail.com`
- `Technical conversations`: `alexmico2006@gmail.com`

## Contact

- Email: `alexmico2006@gmail.com`
- Website: `coming soon`
- Waitlist: `coming soon`

---

<div align="center">

**Trainity is building software for people who actually train.**

</div>
