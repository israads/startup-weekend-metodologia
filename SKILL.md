---
name: startup-weekend
description: |
  Guía interactiva completa para Startup Weekend (evento de 54 horas). Hace preguntas
  para entender la situación del equipo y genera outputs reales: pitch de 1 minuto,
  script de customer discovery, Lean Canvas completo, definición del MVP, deck de
  presentación final y respuestas preparadas para jueces. Cubre las 3 etapas del evento:
  Etapa 1 (Viernes: ideación, pitch y formación de equipo), Etapa 2 (Sábado: validación
  con usuarios reales, construcción del MVP y mentorías), Etapa 3 (Domingo: refinamiento,
  pitch de 5 minutos ante jueces y Q&A). Integra la metodología VMOST para alineación
  estratégica del equipo durante el fin de semana.
  Úsalo cuando: el usuario participe en un Startup Weekend, necesite preparar un pitch,
  validar una idea, definir un MVP, estructurar su equipo, completar un Lean Canvas,
  preparar una presentación final o responder preguntas de jueces en competencias de startups.
version: 1.0.0
maintainer: israads
tags: [startup, emprendimiento, innovacion, lean-startup, mvp, pitch, canvas, vmost]
user-invocable: true
argument-hint: "[etapa1|etapa2|etapa3|pitch|canvas|mvp|validacion|jueces]"
allowed-tools:
  - Read
  - Write
  - Edit
  - Bash
  - Grep
  - Glob
  - AskUserQuestion
  - WebSearch
  - WebFetch
---

# Startup Weekend — Guía Interactiva de 54 Horas

<!-- Referencias detalladas:
  references/etapa1-ideacion-formacion.md      → Viernes: pitch, votación, equipos
  references/etapa2-validacion-desarrollo.md   → Sábado: validación, MVP, mentorías
  references/etapa3-presentacion-final.md      → Domingo: pitch final, jueces, Q&A
  references/vmost-framework.md               → Metodología VMOST para alineación
  references/herramientas-canvas.md           → Lean Canvas y Business Model Canvas
-->

## Cómo opera este skill

Este skill hace preguntas para entender la situación específica del equipo y genera outputs reales: textos de pitch, Lean Canvas completo, script de entrevistas, especificación del MVP, slides del deck, y respuestas preparadas para jueces. No solo explica — produce.

### Detección automática de etapa

Antes de empezar, identificar en qué momento del evento está el equipo:

```
¿Cuándo está el equipo?
→ "todavía no empezamos / viernes / tengo mi idea / quiero hacer el pitch"
  → ACTIVAR: Modo Etapa 1 — Ideación y Formación

→ "es sábado / estamos validando / necesito entrevistar / qué pregunto a usuarios"
  → ACTIVAR: Modo Etapa 2 — Validación y Desarrollo

→ "es domingo / necesito el pitch / cómo presento / qué preguntan los jueces"
  → ACTIVAR: Modo Etapa 3 — Presentación Final

→ No es claro → Preguntar: "¿Están en el viernes, sábado o domingo del evento?"
```

---

## MODO ETAPA 1 — Viernes: Ideación y Formación

> Referencia completa: `references/etapa1-ideacion-formacion.md`

### Secuencia de preguntas para generar el pitch de 1 minuto

Hacer estas preguntas una por una. Con las respuestas, generar el pitch completo.

**Pregunta 1 — El segmento:**
```
"¿A quién va dirigida tu idea? Descríbeme al cliente más específico posible
(no 'todos' ni 'millennials' — piensa en una persona real con nombre, trabajo y situación)."
```

**Pregunta 2 — El dolor:**
```
"¿Cuál es el problema concreto que tiene esa persona? Descríbelo en sus palabras,
no en las tuyas. ¿Qué les duele hoy? ¿Cuánto les cuesta (tiempo o dinero)?"
```

**Pregunta 3 — La solución:**
```
"¿Cuál es tu idea para resolverlo? Exprésala en una frase que cualquier persona
entienda, sin términos técnicos."
```

**Pregunta 4 — La conexión personal:**
```
"¿Por qué tú? ¿Tienes experiencia personal con este problema o conoces a alguien que lo vive?"
```

**Pregunta 5 — El equipo que necesitas:**
```
"¿Qué tipo de personas necesitas en tu equipo? ¿Developer, designer, alguien de ventas?
¿Con qué habilidad específica?"
```

### Template de pitch generado (rellenar con las respuestas)

```
[GANCHO - 10 seg]
"[DATO SORPRENDENTE O SITUACIÓN CONCRETA relacionada al problema]."

[PROBLEMA - 15 seg]
"[SEGMENTO ESPECÍFICO] enfrenta [DOLOR EN SUS PALABRAS]. Hoy lo resuelven con
[ALTERNATIVA EXISTENTE], pero [POR QUÉ ESA SOLUCIÓN ES INSUFICIENTE]."

[SOLUCIÓN - 15 seg]
"Mi propuesta es [SOLUCIÓN EN UNA FRASE]. Esto permitiría [RESULTADO TANGIBLE]."

[BÚSQUEDA - 20 seg]
"Para hacerlo este fin de semana busco:
• Un/a [ROL 1] con experiencia en [HABILIDAD ESPECÍFICA]
• Un/a [ROL 2] que haya [EXPERIENCIA RELEVANTE]
¿Alguien aquí tiene ese perfil?"
```

### Evaluación rápida de la idea (antes del pitch)

Preguntar y puntuar:

| Criterio | Pregunta | Puntos (1-5) |
|----------|----------|--------------|
| Problema real | ¿Lo has vivido tú o alguien que conoces? | ___ |
| Mercado suficiente | ¿Hay 10,000+ personas con este problema? | ___ |
| Diferenciación | ¿Por qué no existe ya? ¿Por qué es mejor? | ___ |
| Ejecutable en 54h | ¿Se puede demostrar un MVP este fin de semana? | ___ |
| Apalancamiento | ¿Tu equipo tiene las habilidades para hacerlo? | ___ |

**15-20 puntos:** Verde — adelante con confianza  
**10-14 puntos:** Amarillo — refinar el ángulo o el segmento  
**Menos de 10:** Rojo — pivotar o unirse a otro proyecto

### Kick-off del equipo (primeros 30 min del viernes)

Una vez formado el equipo, guiar este proceso:

**1. Hipótesis del problema en una frase (consenso)**
Cada miembro escribe en 1 frase cuál es el problema. Si difieren → discutir hasta acordar una sola versión.

**2. División de trabajo para el fin de semana**
```
DEVELOPERS  → ¿Qué stack van a usar? ¿Qué pueden construir en 24h?
DESIGNER    → ¿Quién hace el prototipo visual? ¿En Figma o otra herramienta?
BUSINESS    → ¿Quién dirige las entrevistas mañana? ¿Cuántas entrevistas haremos?
CEO/VOCERO  → ¿Quién presenta el pitch final? (no tiene que ser quien tuvo la idea)
```

**3. Lista de 10+ personas a entrevistar mañana**
Cada miembro del equipo debe comprometerse con 3-5 contactos del segmento.

---

## MODO ETAPA 2 — Sábado: Validación y Desarrollo

> Referencia completa: `references/etapa2-validacion-desarrollo.md`

### Diagnóstico inicial del sábado

Preguntar al inicio del día:

```
"¿En qué punto está el equipo ahora mismo?
A) Estamos a punto de salir a entrevistar usuarios (customer discovery)
B) Ya hicimos entrevistas — necesitamos analizarlas y decidir si pivotar
C) Ya validamos — estamos construyendo el MVP
D) Tenemos el MVP — necesitamos ayuda con el Canvas o las mentorías"
```

### A) Generación del script de customer discovery

Hacer estas preguntas para personalizar el script:

```
"¿Cuál es exactamente el segmento que van a entrevistar hoy?"
"¿Dónde van a encontrarlos (físicamente o digitalmente)?"
"¿Cuál es la hipótesis del problema que quieren validar?"
```

Con esas respuestas, generar un script personalizado de 10 preguntas siguiendo la estructura de `references/etapa2-validacion-desarrollo.md`.

**Script generado incluye:**
- Apertura no invasiva (no mencionar la solución)
- 5 preguntas de exploración del problema
- 2 preguntas de cuantificación
- 2 preguntas de validación de solución (al final, si aplica)
- Cierre con pedido de referidos

**Tabla de síntesis para llenar post-entrevistas:**
```
| # | Nombre | Confirma problema | Alternativa actual | Dispuesto a pagar | Quote clave |
|---|--------|------------------|--------------------|-------------------|-------------|
| 1 |        |                  |                    |                   |             |
| 2 |        |                  |                    |                   |             |
```

### B) Análisis de entrevistas y decisión de pivot

Preguntar:
```
"¿Cuántas entrevistas completaron? ¿Cuántas confirmaron el problema?
¿Encontraron algo que no esperaban?"
```

Generar análisis con:
- Porcentaje de validación de cada hipótesis
- Recomendación: pivot, perseverar, o ajustar el segmento
- Si pivot: qué tipo de pivot y hacia dónde

### C) Definición y especificación del MVP

Secuencia de preguntas para definir el MVP:

**Pregunta 1:**
```
"¿Cuál es la propuesta de valor central que el MVP debe demostrar?
Exprésala en una frase: 'El usuario puede [HACER X] para lograr [RESULTADO Y]'."
```

**Pregunta 2:**
```
"¿Qué recursos técnicos tiene el equipo? (developers, lenguajes, horas disponibles)"
```

**Pregunta 3:**
```
"¿El MVP necesita funcionar de verdad o puede ser un prototipo clickeable?"
```

Con esas respuestas, generar:

**Especificación del MVP:**
```
TIPO DE MVP RECOMENDADO: [App web / Prototipo Figma / Bot / Concierge / Landing]

FLUJO CORE (obligatorio para la demo):
Paso 1: [Descripción]
Paso 2: [Descripción]
Paso 3: [Descripción]

FUNCIONES IN SCOPE:
✅ [Feature 1] — porque demuestra directamente la propuesta de valor
✅ [Feature 2] — porque es necesario para el flujo core
✅ [Feature 3] — porque los jueces lo esperan en este tipo de producto

FUNCIONES OUT OF SCOPE (para después del evento):
❌ [Feature A] — no es necesario para demostrar la propuesta de valor
❌ [Feature B] — toma más tiempo del que hay disponible

CRITERIO DE "DONE":
El MVP está listo cuando: [DESCRIPCIÓN ESPECÍFICA DE QUÉ DEBE PODER HACER UN USUARIO]

STACK RECOMENDADO (si se solicitó):
Frontend: [Recomendación]
Backend: [Recomendación]
Integraciones: [APIs relevantes]
```

### D) Lean Canvas completo

Preguntar y generar celda por celda:

```
"Dame la información que tienen hasta ahora y generaré el Lean Canvas completo.
¿Ya completaron las entrevistas? ¿Definieron el modelo de negocio?"
```

Generar el Lean Canvas con la información disponible, marcando con ⚠️ las celdas que necesitan más validación y con ✅ las que están confirmadas.

Ver template completo en `references/herramientas-canvas.md`.

### Preparación para mentorías

Generar el brief de mentoría:

```
"¿En qué área necesitan más ayuda de los mentores?
A) Validación y customer discovery
B) Modelo de negocio y monetización
C) Estrategia técnica del MVP
D) Go-to-market y canales de adquisición"
```

Generar brief de mentoría con:
- Resumen de 2 minutos del estado actual
- Hipótesis específica que quieren validar con el mentor
- 3 preguntas concretas para el mentor

---

## MODO ETAPA 3 — Domingo: Presentación Final

> Referencia completa: `references/etapa3-presentacion-final.md`

### Generación del pitch de 5 minutos

Secuencia de preguntas para generar el pitch completo:

**Bloque 1 — Contexto:**
```
"¿Cuántas entrevistas hicieron? ¿Cuál fue el hallazgo más importante?
¿Tienen algún cliente real, pre-registro o compromiso de pago?"
```

**Bloque 2 — El modelo:**
```
"¿Cómo van a ganar dinero? ¿Cuánto cobrarán? ¿A quién exactamente?"
```

**Bloque 3 — El equipo:**
```
"¿Cuántos son en el equipo? ¿Cuál es el nombre y rol de cada uno?
¿Qué hace relevante a cada persona para este proyecto específico?"
```

**Bloque 4 — El MVP:**
```
"¿Qué pueden demostrar en la demo? ¿Funciona de verdad o es prototipo?"
```

Con esas respuestas, generar el script completo del pitch:

```
SCRIPT DEL PITCH — [NOMBRE DEL PROYECTO]
Duración: 5 minutos

[0:00 – 0:30] GANCHO
"[Historia real de un usuario con nombre y situación concreta]..."

[0:30 – 1:15] EL PROBLEMA
"[Dimensión del problema: estadística + por qué importa ahora]..."

[1:15 – 2:00] LA SOLUCIÓN + DEMO
"[Frase de transición a la demo]..."
[DEMO EN VIVO — mostrar el flujo core]
"Como acaban de ver, [lo que acaba de pasar en la demo]..."

[2:00 – 2:30] VALIDACIÓN
"Este fin de semana hablamos con [N] personas del segmento.
El [%] confirmó que [HIPÓTESIS CENTRAL].
[NOMBRE REAL] nos dijo: '[QUOTE LITERAL]'..."

[2:30 – 3:00] MERCADO Y MODELO
"El mercado accesible para nosotros son [SEGMENTO] — [N] en [geografía].
Cobramos $[PRECIO] por [UNIDAD/MES]. Con [N] clientes, eso representa $[MRR]..."

[3:00 – 3:30] EL EQUIPO
"Somos [N] personas: [LISTA CON ROLES Y EXPERTISE RELEVANTE]..."

[3:30 – 4:00] VISIÓN Y CIERRE
"Si tenemos éxito, [VISIÓN DE FUTURO EN 1 FRASE].
[CIERRE CON ENERGÍA]."
```

### Generación del deck de presentación

Con la información del pitch, generar el contenido de cada slide:

```
SLIDE 1 — PORTADA
Texto: [Nombre] | [Tagline de 1 frase]

SLIDE 2 — EL PROBLEMA
Headline: "[Estadística o dato más impactante]"
Subtext: "[2-3 líneas máximo explicando el dolor]"
Visual recomendado: [Descripción del visual o gráfica sugerida]

SLIDE 3 — LA SOLUCIÓN
Headline: "[Propuesta de valor única]"
Subtext: "[Cómo funciona en 1 frase]"
Visual: Captura del MVP o flujo simplificado

[... continuar para cada slide ...]
```

### Preparación de Q&A con jueces

Preguntar:
```
"¿Cuáles son los puntos más débiles de su propuesta que los jueces podrían atacar?
¿Falta algo de validación? ¿El modelo de negocio tiene huecos?"
```

Generar las respuestas preparadas para las preguntas más probables, usando las respuestas del equipo como base.

Ver las 10 preguntas más comunes y cómo responderlas en `references/etapa3-presentacion-final.md`.

### Checklist final antes de presentar

Generar y revisar:

```
CONTENIDO:
□ Script del pitch ensayado 3+ veces con cronómetro
□ Respuestas preparadas para las 5 preguntas más probables
□ Quotes reales de usuarios listos para citar
□ Nombre y rol de cada miembro del equipo listo para presentar

TÉCNICA:
□ MVP probado 5 veces sin errores
□ Demo funciona sin WiFi del evento (hotspot propio)
□ Video de respaldo de 45 segundos descargado
□ Slides en PDF de backup

EQUIPO:
□ Vocero principal del pitch definido
□ Quién maneja preguntas técnicas vs. de negocio, acordado
□ Señal interna si alguien va muy lento o muy rápido
```

---

## VMOST — Alineación Estratégica del Equipo

> Referencia completa: `references/vmost-framework.md`

Cuando el equipo necesite alinearse estratégicamente, hacer estas preguntas y generar el VMOST completo:

```
V: "¿Qué futuro quieren crear? ¿Cómo debería cambiar el mundo si su startup tiene éxito?"
M: "¿Cuál es el propósito concreto de su empresa? ¿A quién sirven y cómo?"
O: "¿Qué métricas específicas quieren alcanzar en 12 meses?"
S: "¿Cuál es su estrategia principal de go-to-market?"
T: "¿Qué van a hacer específicamente hoy, mañana y el domingo?"
```

Generar el documento VMOST completo del equipo y verificar alineación top-down y bottom-up.

---

## Comandos Rápidos

| Comando | Acción |
|---------|--------|
| `/startup-weekend` | Diagnóstico interactivo: ¿en qué etapa están? |
| `/startup-weekend etapa1` | Modo Etapa 1: pitch de 1 minuto + kick-off |
| `/startup-weekend etapa2` | Modo Etapa 2: validación + MVP + Canvas |
| `/startup-weekend etapa3` | Modo Etapa 3: pitch final + jueces + deck |
| `/startup-weekend pitch` | Generador de pitch (1 min o 5 min según etapa) |
| `/startup-weekend canvas` | Generador de Lean Canvas completo |
| `/startup-weekend mvp` | Especificación del MVP con scope y stack |
| `/startup-weekend validacion` | Script personalizado de customer discovery |
| `/startup-weekend jueces` | Q&A preparado para preguntas de jueces |
| `/startup-weekend vmost` | Generador del framework VMOST del equipo |
