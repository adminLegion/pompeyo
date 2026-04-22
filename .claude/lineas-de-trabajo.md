# Líneas de trabajo — Pompeyo

> Ver definición de estados en `../../templates/lineas-de-trabajo.md.template`.

---

## Líneas activas

### Mantener operación diaria

- **Estado:** `live`
- **Owner:** Fabio
- **Objetivo:** mantener Pompeyo funcional en el día a día. Fix bugs, mejorar prompts, ajustar tools según uso real.
- **Ubicación código:** `training-fabio/projects/priamo/` (hasta migración).

## Líneas en exploración

### Migración a repo `pompeyo/`

- **Estado:** `exploring`
- **Objetivo:** mover el código de `training-fabio/projects/priamo/` a este repo, con historial limpio y estructura productiva.
- **Motivación:** dar estabilidad, CI, versionado serio.
- **Siguiente paso:** decidir si `git subtree split` preserva historial parcial, o comienzo limpio con referencia al origen.

### Integración calendario

- **Estado:** `exploring`
- **Objetivo:** Pompeyo puede leer y crear eventos en calendario personal.
- **Motivación:** uno de los usos más demandados en asistentes personales.
- **Siguiente paso:** elegir API (Google o Apple) y diseñar scope mínimo (solo lectura primero).

### Recordatorios proactivos

- **Estado:** `idea`
- **Objetivo:** Pompeyo envía mensajes por iniciativa propia cuando detecta eventos relevantes (inicio de día, reuniones próximas, pendientes vencidos).
- **Motivación:** asistente pasivo vs activo. Pasar a activo es el siguiente nivel.
- **Siguiente paso:** definir qué triggers son útiles vs ruidosos.

### Voz (STT + TTS)

- **Estado:** `idea`
- **Objetivo:** interacción por voz, tanto entrada (transcripción) como salida (respuesta hablada).
- **Motivación:** manos libres, uso en carro, situaciones sin pantalla.
- **Siguiente paso:** evaluar pipelines (Whisper local vs API, ElevenLabs vs alternativas).

### Integraciones multi-agente con Legion

- **Estado:** `idea`
- **Objetivo:** Pompeyo puede invocar/consultar agentes internos de Legion (ej. consultar estado de PRs, lanzar tareas de análisis).
- **Motivación:** Pompeyo deja de ser solo "chat" y se vuelve hub de orquestación.
- **Siguiente paso:** revisar cuando Legion tenga agentes internos utilizables.

## Líneas archivadas

(Vacío.)

---

**Última actualización:** 2026-04-22
