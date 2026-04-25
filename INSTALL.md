# Guía de Instalación — Startup Weekend Mentor

Este framework funciona en múltiples plataformas. Elige la que uses:

---

## Claude Code (Skill)

El skill más completo. Hace preguntas, genera debates y produce outputs personalizados.

```bash
# Instalar el skill
git clone https://github.com/israads/startup-weekend-metodologia.git \
  ~/.claude/skills/startup-weekend

# Verificar instalación
claude /startup-weekend
```

**Comandos disponibles:**
```
/startup-weekend              → Diagnóstico interactivo
/startup-weekend comenzar     → Onboarding del evento y equipo
/startup-weekend continuar    → Retomar sesión desde sesion/
/startup-weekend progreso     → Tracker de progreso del equipo
/startup-weekend descubrir    → Motor de descubrimiento del problema
/startup-weekend validar-rapido → Test Card + experimento de 30-90 min
/startup-weekend evidencias   → Learning Card + scoring acumulado
/startup-weekend debatir      → Facilitador de debates (10 min)
/startup-weekend duda         → Agente de situaciones comunes
/startup-weekend etapa1       → Guía completa del viernes
/startup-weekend etapa2       → Guía completa del sábado
/startup-weekend etapa3       → Guía completa del domingo
/startup-weekend pitch1       → Generador de pitch de 60 seg
/startup-weekend pitch5       → Generador de pitch de 5 min
/startup-weekend canvas       → Lean Canvas completo
/startup-weekend mvp          → Especificación del MVP
/startup-weekend script       → Script de customer discovery
/startup-weekend deck         → Deck slide por slide
/startup-weekend jueces       → Q&A para preguntas de jueces
/startup-weekend revisar      → Auditoría de calidad
/startup-weekend vmost        → Framework VMOST del equipo
```

---

## Claude.ai (Proyecto)

Para usar sin instalar nada, directamente en claude.ai.

1. Ir a **[claude.ai](https://claude.ai)** → **Projects** → **New Project**
2. Nombre: `Startup Weekend Mentor`
3. Abrir `prompts/claude-project-instructions.md`
4. Copiar el bloque entre ``` ``` ``` al campo **Project Instructions**
5. (Pro/Team) Subir los archivos de `references/` como **Project Knowledge**

Ver instrucciones completas en `prompts/claude-project-instructions.md`

---

## ChatGPT Custom GPT

Para crear un GPT personalizado en ChatGPT.

1. Ir a **[chat.openai.com](https://chat.openai.com)** → **Explore GPTs** → **Create**
2. Click en **Configure** (pestaña)
3. Nombre: `Startup Weekend Mentor`
4. Abrir `prompts/chatgpt-custom-gpt.md`
5. Copiar el bloque de **Instrucciones del Sistema** al campo **Instructions**
6. Configurar los **Conversation Starters** (en el mismo archivo)
7. (Opcional) Subir archivos de `references/` en **Knowledge**
8. Click **Save** → **Publish**

Ver instrucciones completas en `prompts/chatgpt-custom-gpt.md`

---

## Gemini (Gem)

Para crear un Gem personalizado en Google Gemini.

1. Ir a **[gemini.google.com](https://gemini.google.com)** → **Gems** → **Create a Gem**
2. Nombre: `Startup Weekend Mentor`
3. Abrir `prompts/universal-system-prompt.md`
4. Copiar el bloque entre ``` ``` ``` al campo de instrucciones del Gem
5. Click **Save**

---

## Cursor

Para usar en el editor de código Cursor.

**Opción rápida (Rules for AI):**
1. Abrir **Cursor Settings** → **Rules for AI**
2. Pegar:
```
Eres el mentor digital de un equipo en Startup Weekend (54 horas).
Siempre muestra: "ETAPA [X]/3 — [Nombre]" al inicio de cada respuesta.
Modos: DESCUBRIR · VALIDAR RÁPIDO · DEBATIR · CONSTRUIR · REVISAR
Para el sistema completo: lee el archivo prompts/universal-system-prompt.md de este proyecto.
```

**Opción completa (.cursorrules):**
1. Crear `.cursorrules` en la raíz del proyecto
2. Copiar el contenido completo de `prompts/universal-system-prompt.md` (entre las triple comillas)

Ver más opciones en `prompts/cursor-rules.md`

---

## Windsurf

Para usar en el editor Windsurf.

1. El archivo `.windsurfrules` ya está configurado en este repositorio
2. Clona el repositorio en tu proyecto
3. Windsurf leerá automáticamente las reglas

---

## Perplexity AI

Para usar en Perplexity.

1. Ir a **[perplexity.ai](https://perplexity.ai)** → **New Space**
2. Nombre: `Startup Weekend Mentor`
3. En **Space Instructions**, pegar el contenido de `prompts/universal-system-prompt.md`

---

## Cualquier LLM con System Prompt

Para cualquier plataforma que acepte un system prompt (Mistral, LLaMA, Groq, etc.):

1. Abrir `prompts/universal-system-prompt.md`
2. Copiar el bloque completo entre las ``` ``` ``` (el prompt real, sin el encabezado markdown)
3. Pegarlo como **System Prompt** o **System Instructions** de la plataforma

---

## Uso sin instalación (copy-paste directo)

Si no quieres instalar nada, puedes copiar este texto al inicio de cualquier conversación:

```
Actúa como el mentor digital de mi equipo en Startup Weekend (54 horas).
Tu trabajo: hacer preguntas que el equipo no está haciendo, facilitar debates y producir outputs concretos.
Siempre muestra "ETAPA [X]/3 — [Nombre]" al inicio de cada respuesta.
Modos: DESCUBRIR (problema no claro) / VALIDAR RÁPIDO (experimento de 30-90 min + scoring) / DEBATIR (equipo atascado) / CONSTRUIR (necesito un output) / REVISAR (auditoría).
Regla: "me gusta" no valida; busca acciones observables como email, referido, piloto, carta de intención, pago o uso real.
Primero pregúntame: ¿En qué etapa del evento están? (Viernes, Sábado o Domingo)
```

Para el sistema completo, usa el prompt en `prompts/universal-system-prompt.md`.

---

## Estructura del repositorio

```
startup-weekend-metodologia/
│
├── SKILL.md                                ← Claude Code (skill principal)
├── INSTALL.md                              ← Esta guía
├── README.md                               ← Descripción del proyecto
├── LICENSE                                 ← Licencia MIT
├── .windsurfrules                          ← Windsurf config
│
├── prompts/
│   ├── universal-system-prompt.md          ← Para cualquier LLM
│   ├── chatgpt-custom-gpt.md              ← ChatGPT Custom GPT
│   ├── claude-project-instructions.md     ← Claude.ai Projects
│   └── cursor-rules.md                    ← Cursor IDE
│
└── references/
    ├── mentor-mode.md                      ← Cómo opera el mentor
    ├── descubrimiento-problema.md          ← Motor de descubrimiento
    ├── validacion-rapida.md                ← Test Cards, Learning Cards y evidencia
    ├── debate-facilitator.md               ← Facilitación de debates
    ├── faq-situaciones.md                  ← Agente de dudas y situaciones comunes
    ├── etapa1-ideacion.md                  ← Viernes: detalle completo
    ├── etapa2-validacion.md                ← Sábado: detalle completo
    ├── etapa3-presentacion.md              ← Domingo: detalle completo
    ├── vmost-framework.md                  ← Metodología VMOST
    └── herramientas-canvas.md              ← Lean Canvas y BMC
```
