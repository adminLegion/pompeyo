# Estrategia — Pompeyo

> Visión de Pompeyo como asistente personal. No comercial.
>
> **Última actualización:** 2026-04-22
> **Owner:** Fabio Romero

---

## 1. Propósito

Servir como asistente personal integral de Fabio. Compañero AI que asiste transversalmente en ingeniería, estrategia, vida personal, y operación del día a día.

Inspiración: JARVIS (Iron Man). La aspiración es un asistente que **conoce el contexto completo del usuario** y reduce carga cognitiva en todas las facetas de vida.

## 2. Visión

Pompeyo es, en estado objetivo, un asistente que:

1. Recuerda de forma persistente lo importante (proyectos, personas, decisiones, preferencias).
2. Es accesible desde cualquier dispositivo (hoy Telegram; mañana voz, wearable).
3. Integra herramientas del ecosistema de Fabio (calendario, notas, repos, finanzas, salud).
4. Protege la privacidad — servidor personal, no SaaS.
5. Evoluciona iterativamente con cada uso; cada conversación refina sus capacidades.

## 3. Diferenciadores vs alternativas (ChatGPT apps, Claude app, etc.)

- **Memoria real persistente** (no solo contexto de conversación).
- **Servidor propio** — privacidad total, control de datos.
- **Integrable con herramientas personales** (calendar, notes, GitHub, etc.) sin cloud de terceros.
- **Modo multi-dispositivo nativo** vía Tailscale.
- **Construido por y para el usuario** — no generic.

## 4. Capacidades actuales

En `training-fabio/projects/priamo/`:

- Bot de Telegram funcional.
- Claude API como backend LLM.
- SQLite para memoria (conversaciones, recuerdos, proyectos).
- FastAPI para endpoints.
- Tailscale para acceso remoto.

## 5. Capacidades aspiracionales (roadmap informal)

- Integración con calendario real (Google Calendar / Apple Calendar).
- Notas bidireccionales (Obsidian / Notion).
- Integración con GitHub (estado de repos, PRs, notificaciones).
- Recordatorios proactivos (no solo reactivos).
- Voz (STT + TTS).
- Contexto de salud (si aplica, desde Apple Health).
- Resúmenes diarios / semanales proactivos.
- Integración con otros agentes de Legion (Legion Cloud tooling, Legion Defense sandbox).

## 6. Modelo económico

**Ninguno.** Pompeyo es personal. No se vende, no se SaaS-ifica. Si algún día se comercializa (derivado), sería un producto separado bajo Legion con rebranding.

## 7. Decisiones clave

| Fecha | Decisión | Motivo |
|---|---|---|
| 2026-04-22 | Crear repo separado `pompeyo/` | Darle madurez de producto versionable, separado de training |
| 2026-04-22 | Renombrar "Priamo" → "Pompeyo" | — (decisión de Fabio) |
| 2026-04-22 | No migrar código todavía | Separar decisión de repo vs migración; código sigue funcional en training-fabio |
