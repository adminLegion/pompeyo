# Pompeyo — Contexto del repo

> Asistente personal estilo JARVIS del fundador de Legion. Producto personal, no comercial.
>
> Parte de [Legion](../../CLAUDE.md) — holding de divisiones especializadas.

---

## 1. Qué es Pompeyo

Pompeyo es el asistente personal de Fabio (antes llamado "Priamo"). Es un producto **personal y maduro**, en uso diario, no un experimento ni producto comercial. Vive dentro del portfolio de Legion para darle versionado serio, despliegue reproducible y potencial evolución.

**Visibilidad:** Public. Compartimos el enfoque arquitectónico; las integraciones personales se parametrizan.

**Rol en Legion:** producto personal del fundador. Prueba viva de nuestra capacidad con agentes AI. No es servicio comercial.

## 2. Referencias obligatorias

- [`../../CLAUDE.md`](../../CLAUDE.md) — contexto maestro de Legion
- [`../../team/git-workflow.md`](../../team/git-workflow.md) — convenciones Git
- [`../../team/claude-usage.md`](../../team/claude-usage.md) — cómo usar Claude Code
- [`./strategy.md`](./strategy.md) — estrategia / visión
- [`./lineas-de-trabajo.md`](./lineas-de-trabajo.md) — líneas activas

## 3. Stack técnico

```
Lenguaje:              Python 3.12
Backend:               FastAPI + Uvicorn
LLM:                   Anthropic Claude API
Interfaz primaria:     Telegram bot
Persistencia:          SQLite (memoria, conversaciones, proyectos, recuerdos)
Acceso remoto:         Tailscale (acceso desde cualquier dispositivo)
Hosting:               Mac Mini M4 (servidor personal)
```

## 4. Código actual

**El código hoy vive en `training-fabio/projects/priamo/`**, NO en este repo todavía. Este repo se creó con scaffold organizacional; la migración del código se hará cuando Fabio lo decida.

Razón: separar decisión de "crear repo productivo para Pompeyo" de "migrar código existente". Evita que una decisión dependa de la otra.

## 5. Estructura del repo (cuando se migre el código)

```
pompeyo/
├── .claude/
├── app/
│   ├── api/               ← endpoints FastAPI
│   ├── bot/               ← Telegram bot handlers
│   ├── memory/            ← persistencia, recuerdos, proyectos
│   ├── agent/             ← lógica del agente (prompts, routing, tools)
│   └── tools/             ← integraciones externas (calendar, notes, etc.)
├── deployment/            ← scripts de despliegue en Mac Mini
├── tests/
├── docs/
├── README.md
├── pyproject.toml
└── .gitignore
```

## 6. Convenciones locales

**Privacidad:**
- Ningún dato personal de Fabio va al repo (recuerdos, conversaciones reales).
- Memoria persistente (SQLite) está gitignoreada.
- Configuración parametrizable: no hardcodear nombres, rutas personales, tokens.

**Credenciales:**
- API keys (Anthropic, Telegram bot token) solo en `.env` local — nunca commit.

## 7. Co-authorship de Claude

Repo **public** → co-author Claude **permitido y recomendado**. Pompeyo mismo usa Claude, tiene sentido reconocerlo.

## 8. Contactos y responsables

- **Lead:** Fabio Romero (único owner)
- **Equipo:** — (proyecto individual)

## 9. Estado actual

Repo recién creado (2026-04-22) con scaffold docs. Código en `training-fabio/projects/priamo/`. Migración pendiente de priorización.
