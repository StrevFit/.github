<div align="center">

<a href="./README.md">
  <img src="https://img.shields.io/badge/ES-56b8d4?style=for-the-badge&labelColor=0f172a&color=56b8d4" alt="README en Espanol" />
</a>
<a href="./README.en.md">
  <img src="https://img.shields.io/badge/EN-1f2937?style=for-the-badge&labelColor=0f172a&color=1f2937" alt="README in English" />
</a>

<h1>Liftnotch</h1>

<p><strong>Software para entrenamiento serio.</strong></p>
<p>Planifica mejor. Registra mas rapido. Lee el progreso sin ruido.</p>

<p>
  <img src="https://img.shields.io/badge/Beta-Abierta-56b8d4?style=flat-square&labelColor=0f172a" alt="Beta abierta" />
  <img src="https://img.shields.io/badge/Stack-React%2019%20%2B%20Express%205-56b8d4?style=flat-square&labelColor=0f172a" alt="Stack principal" />
  <img src="https://img.shields.io/badge/Core-MongoDB%20%2B%20Zod-56b8d4?style=flat-square&labelColor=0f172a" alt="Core" />
</p>

<p>
  <a href="https://liftnotch.com">Web</a> ·
  <a href="https://liftnotch.com/waitlist">Waitlist</a> ·
  <a href="mailto:alexmico2006@gmail.com">Contacto</a>
</p>

</div>

---

## Tesis

Liftnotch se esta construyendo como un `training operating system` para entrenadores, clientes y atletas independientes. La prioridad no es producir otra app de fitness generica, sino resolver la operativa real del entrenamiento: planificar, ejecutar y leer progreso desde un mismo sistema.

La mayor parte del codigo sigue siendo privada mientras el producto evoluciona. Este perfil publico existe para compartir la direccion del proyecto, sus principios y la manera en la que pensamos producto e ingenieria.

> El software de entrenamiento no deberia estorbar durante una sesion real.
> Deberia acelerar decisiones, reducir friccion y aguantar uso diario.

## Donde Aporta Valor

<table>
  <tr>
    <td width="33%" valign="top">
      <h3>Plan</h3>
      <p>Rutinas, bloques y asignacion para que la programacion no viva repartida entre mensajes, notas y hojas de calculo.</p>
    </td>
    <td width="33%" valign="top">
      <h3>Log</h3>
      <p>Registro de sesiones pensado para tocar, confirmar y seguir entrenando sin friccion innecesaria.</p>
    </td>
    <td width="33%" valign="top">
      <h3>Read</h3>
      <p>Metricas y progreso con lectura operativa para decidir el siguiente paso sin ruido analitico.</p>
    </td>
  </tr>
</table>

## Para Quien

- `Trainer`: crea rutinas, asigna clientes y revisa progreso con una operativa `desktop-first`.
- `Client`: recibe la planificacion, registra sesiones y reporta contexto con experiencia `mobile-first`.
- `Independent`: gestiona sus propios bloques y sesiones sin depender de herramientas dispersas.

## Principios De Producto

- `Desktop-first` para coach ops y trabajo de gestion.
- `Mobile-first` para logging durante el entreno.
- Menos clicks, menos campos inutiles, mas continuidad en flujos criticos.
- IA util solo si ayuda; siempre desacoplada del core transaccional.

## Estado Del Producto

- Registro y login con seleccion de rol.
- Creacion, edicion y asignacion de rutinas.
- Logging de sesiones con series, reps, peso y notas.
- Dashboard con progreso por ejercicio y metricas semanales.
- Base preparada para modulos de IA y flujos premium.

## Arquitectura

```text
web (React / Vite)
        |
        v
api (Express)
        |
        v
db (MongoDB / Mongoose)
```

### Principios de sistema

- `controllers -> services -> repositories -> models`
- validacion de entrada con `Zod`
- roles de dominio explicitos: `trainer`, `client`, `independent`
- frontend orientado a producto y uso real, no a una demo bonita
- modulos de IA aislados del core

## Lo Que Compartimos Aqui

Este perfil publico se usa para compartir:

- tesis de producto
- decisiones de arquitectura
- repositorios publicos auxiliares cuando tenga sentido
- puntos de entrada para colaboracion tecnica o estrategica

## Contacto

- Web: `https://liftnotch.com`
- Waitlist: `https://liftnotch.com/waitlist`
- General: `alexmico2006@gmail.com`
- Partnerships: `alexmico2006@gmail.com`

---

<div align="center">

<strong>Software para gente que entrena de verdad.</strong>

</div>
