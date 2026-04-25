# Startup Weekend — Skill para Claude Code

Skill interactivo para Claude Code que guía equipos a través de las 3 etapas de un Startup Weekend (evento de 54 horas). Hace preguntas, genera outputs reales y acompaña al equipo desde el pitch inicial hasta la presentación ante jueces.

## ¿Qué hace este skill?

No solo explica — **produce**. Según la etapa en que se encuentre el equipo, genera:

- Pitch de 60 segundos (Viernes)
- Script personalizado de customer discovery (Sábado)
- Lean Canvas completo con validación
- Especificación del MVP con scope, stack y criterios de "done"
- Brief de mentoría para cada ronda
- Script completo del pitch de 5 minutos (Domingo)
- Contenido slide por slide del deck de presentación
- Respuestas preparadas para preguntas de jueces
- Framework VMOST del equipo

## Las 3 Etapas del Evento

### Etapa 1 — Viernes: Ideación y Formación de Equipos
Pitch de 60 segundos → Votación → Formación de equipos → Kick-off

### Etapa 2 — Sábado: Validación y Desarrollo
Customer discovery → Síntesis → Pivot o perseverar → MVP → Mentorías → Canvas

### Etapa 3 — Domingo: Presentación Final
Refinamiento → Ensayos → Pitch de 5 minutos → Q&A con jueces

## Metodología VMOST

El skill integra el framework VMOST (Vision, Mission, Objectives, Strategy, Tactics) para mantener al equipo alineado estratégicamente durante las 54 horas del evento.

## Instalación

```bash
# Clonar en tu directorio de skills de Claude Code
git clone https://github.com/israads/startup-weekend-metodologia.git ~/.claude/skills/startup-weekend

# Verificar que el skill está disponible
claude /startup-weekend
```

## Uso

```
/startup-weekend              → Diagnóstico interactivo de etapa
/startup-weekend etapa1       → Guía completa del Viernes
/startup-weekend etapa2       → Guía completa del Sábado
/startup-weekend etapa3       → Guía completa del Domingo
/startup-weekend pitch        → Generador de pitch (1 min o 5 min)
/startup-weekend canvas       → Generador de Lean Canvas completo
/startup-weekend mvp          → Especificación del MVP
/startup-weekend validacion   → Script de customer discovery
/startup-weekend jueces       → Q&A preparado para jueces
/startup-weekend vmost        → Framework VMOST del equipo
```

## Estructura del Repositorio

```
startup-weekend-metodologia/
├── SKILL.md                               # Skill principal (Claude Code lo lee aquí)
├── README.md                              # Este archivo
└── references/
    ├── etapa1-ideacion-formacion.md       # Guía detallada del Viernes
    ├── etapa2-validacion-desarrollo.md    # Guía detallada del Sábado
    ├── etapa3-presentacion-final.md       # Guía detallada del Domingo
    ├── vmost-framework.md                 # Metodología VMOST para startups
    └── herramientas-canvas.md             # Lean Canvas y Business Model Canvas
```

## Sobre Startup Weekend

Startup Weekend es un evento global de 54 horas organizado por Techstars donde equipos multidisciplinarios construyen startups desde cero. El evento opera en más de 150 países con la filosofía **"No Talk, All Action"**. Los equipos combinan perfiles de developers, designers y business para validar ideas, construir MVPs y presentar ante jueces.

## Licencia

MIT — úsalo, modifícalo y compártelo libremente.
