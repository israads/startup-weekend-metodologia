# Startup Weekend — Mentor Digital Interactivo

El mentor digital que tu equipo necesita durante las 54 horas de Startup Weekend. No solo explica — hace preguntas, facilita debates, descubre el problema real y produce outputs concretos en cada etapa.

Funciona en Claude Code, ChatGPT, Claude.ai, Gemini, Cursor, Windsurf y cualquier LLM.

---

## ¿Qué hace diferente este mentor?

La mayoría de los recursos de Startup Weekend te dicen **qué** hacer. Este mentor te pregunta **por qué** crees que lo que estás haciendo tiene sentido — y luego te ayuda a verificarlo.

**Siempre muestra en qué etapa estás:**
```
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
 STARTUP WEEKEND · ETAPA 2/3
 Validación y Desarrollo · Sábado
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
```

**Opera en 4 modos:**

| Modo | Cuándo | Qué hace |
|------|--------|---------|
| **DESCUBRIR** | El problema no está claro | Pipeline socrático de 5 niveles hasta la causa raíz |
| **DEBATIR** | El equipo está atascado | Protocolo de 10 minutos que fuerza una decisión |
| **CONSTRUIR** | Necesitan un output | Genera pitch, canvas, MVP, deck, Q&A personalizado |
| **REVISAR** | Quieren saber si están listos | Auditoría de calidad por checklist de etapa |

---

## Las 3 Etapas del Evento

### Etapa 1 — Viernes: Ideación y Formación (18:00-22:00)
- Evaluación de ideas con criterios objetivos
- Generación del pitch de 60 segundos
- Formación del equipo y kick-off
- Preparación del customer discovery del sábado

### Etapa 2 — Sábado: Validación y Desarrollo (08:00-22:00)
- Script personalizado de customer discovery
- Análisis de entrevistas y decisión de pivot
- Especificación del MVP (scope, stack, criterio de done)
- Lean Canvas completo con marcadores de validación
- Brief de mentoría para cada ronda de mentores

### Etapa 3 — Domingo: Presentación Final (08:00-17:00)
- Script del pitch de 5 minutos con timing exacto
- Contenido del deck slide por slide
- Q&A preparado para las 10 preguntas más comunes de jueces
- Checklist técnico completo antes de presentar

---

## Instalación por Plataforma

### Claude Code (Skill)
```bash
git clone https://github.com/israads/startup-weekend-metodologia.git \
  ~/.claude/skills/startup-weekend
```
Luego: `claude /startup-weekend`

### Claude.ai
Ir a Projects → New Project → pegar `prompts/claude-project-instructions.md`

### ChatGPT Custom GPT
Explore GPTs → Create → Configure → pegar `prompts/chatgpt-custom-gpt.md`

### Gemini Gem
Gems → Create a Gem → pegar `prompts/universal-system-prompt.md`

### Cursor / Windsurf
Usar `prompts/cursor-rules.md` o `.windsurfrules` incluido en el repo

### Cualquier LLM
Copiar el contenido de `prompts/universal-system-prompt.md` como System Prompt

Ver `INSTALL.md` para instrucciones detalladas de cada plataforma.

---

## Comandos (Claude Code)

```
/startup-weekend              → Diagnóstico: ¿en qué etapa y modo?
/startup-weekend progreso     → Tracker de progreso del equipo
/startup-weekend descubrir    → Motor de descubrimiento del problema
/startup-weekend debatir      → Facilitador de debates (10 min)
/startup-weekend etapa1       → Guía completa del viernes
/startup-weekend etapa2       → Guía completa del sábado
/startup-weekend etapa3       → Guía completa del domingo
/startup-weekend pitch1       → Genera el pitch de 60 segundos
/startup-weekend pitch5       → Genera el pitch de 5 minutos completo
/startup-weekend canvas       → Genera el Lean Canvas completo
/startup-weekend mvp          → Especificación del MVP
/startup-weekend script       → Script de customer discovery
/startup-weekend deck         → Contenido del deck slide por slide
/startup-weekend jueces       → Q&A preparado para jueces
/startup-weekend revisar      → Auditoría de calidad
/startup-weekend vmost        → Framework VMOST del equipo
```

---

## Estructura del Proyecto

```
startup-weekend-metodologia/
│
├── SKILL.md                               ← Skill principal (Claude Code)
├── INSTALL.md                             ← Guía de instalación
├── README.md                              ← Este archivo
├── .windsurfrules                         ← Config Windsurf
│
├── prompts/
│   ├── universal-system-prompt.md         ← Para cualquier LLM
│   ├── chatgpt-custom-gpt.md             ← ChatGPT Custom GPT
│   ├── claude-project-instructions.md    ← Claude.ai Projects
│   └── cursor-rules.md                   ← Cursor IDE
│
└── references/
    ├── mentor-mode.md                     ← Cómo opera el mentor
    ├── descubrimiento-problema.md         ← Motor de descubrimiento (NUEVO)
    ├── debate-facilitator.md              ← Facilitación de debates (NUEVO)
    ├── etapa1-ideacion.md                 ← Viernes: guía detallada
    ├── etapa2-validacion.md               ← Sábado: guía detallada
    ├── etapa3-presentacion.md             ← Domingo: guía detallada
    ├── vmost-framework.md                 ← Metodología VMOST
    └── herramientas-canvas.md             ← Lean Canvas y BMC
```

---

## Sobre Startup Weekend

Startup Weekend es un evento global de 54 horas organizado por Techstars donde equipos multidisciplinarios construyen startups desde cero. Opera en +150 países con la filosofía **"No Talk, All Action"**. Los equipos combinan developers, designers y perfiles de negocio para validar ideas, construir MVPs y presentar ante jueces.

## Licencia

MIT — úsalo, modifícalo y compártelo libremente.
