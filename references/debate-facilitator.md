# Facilitador de Debates — Decisiones del Equipo

En Startup Weekend, los equipos pierden en promedio 2-3 horas en debates que podrían resolverse en 10 minutos con el framework correcto. Este archivo convierte al mentor en un facilitador de decisiones que respeta el tiempo del equipo.

---

## Principio del Debate Productivo

**La decisión incorrecta ejecutada rápido es mejor que la decisión perfecta ejecutada tarde.**

Un equipo que elige mal pero itera rápido tiene más probabilidad de éxito que un equipo que debate hasta la parálisis. El debate productivo tiene tres propiedades:

1. **Tiempo limitado** — 10 minutos máximo por decisión importante
2. **Basado en evidencia** — Las opiniones ceden ante los datos de las entrevistas
3. **Decisión definitiva** — Una vez decidido, se ejecuta sin reabrir el debate

---

## Las 7 Decisiones Críticas del Fin de Semana

### D1 — ¿Cuál idea elegir? (Viernes, post-votación)

**Cuándo aparece:** Cuando el fundador tiene 2+ ideas o el equipo no está convencido.

**Framework: Evaluación por 5 criterios**

| Criterio | Peso | Idea A | Idea B | Idea C |
|----------|------|--------|--------|--------|
| Problema real y urgente (1-5) | 25% | | | |
| Mercado suficiente (1-5) | 20% | | | |
| Ejecutable en 54h (1-5) | 25% | | | |
| Diferenciación clara (1-5) | 15% | | | |
| Fit del equipo (1-5) | 15% | | | |
| **TOTAL** | 100% | | | |

**Regla:** La idea con mayor puntaje ponderado gana. Si hay empate: elegir la más ejecutable en 54h.

**Preguntas del mentor si el equipo resiste:**
```
"¿Qué información faltaría para estar más seguros?
¿Pueden obtenerla en los próximos 30 minutos?
Si no: elegir y ejecutar."
```

---

### D2 — ¿Pivot o perseverar? (Sábado ~12pm)

**Cuándo aparece:** Post-entrevistas, cuando los datos no son concluyentes.

**Framework: Evidencia vs. Hipótesis**

```
HIPÓTESIS ORIGINAL:
"[El problema que definieron el viernes]"

EVIDENCIA OBTENIDA:
- Entrevistas completadas: ___
- Confirman el problema: ___ / ___  (___%)
- Confirman disposición a pagar: ___ / ___ (___%)
- Señal inesperada encontrada: [Sí/No → qué fue]

DIAGNÓSTICO:
```

| Escenario | Evidencia | Decisión |
|-----------|-----------|----------|
| El problema existe y hay willingness to pay | 7+/10 + 3+/10 emails/pagos | **Perseverar** |
| El problema existe pero nadie pagará | 7+/10 + 0-1/10 pagos | **Pivot de modelo de negocio** |
| El problema no existe como pensaban | <6/10 confirmaciones | **Pivot de problema o segmento** |
| Encontraron un problema más grande | Emergió en las entrevistas | **Pivot a la nueva oportunidad** |
| No hay datos suficientes | <5 entrevistas | **Hacer más entrevistas (2h máx)** |

**Preguntas del mentor para el debate de pivot:**
```
"¿El feedback negativo viene de su segmento target o de personas fuera de él?
[Si es de fuera: no es evidencia de pivot]

¿Cuántas personas describieron el problema con detalles específicos y sin que preguntaran?
[Si nadie: el problema no es urgente]

Si pivotaran ahora, ¿tienen tiempo de construir algo nuevo para el domingo?
[Si no: mejor refinar que abandonar]

¿Hay algún insight de las entrevistas que apunte a un problema MÁS urgente?
[Si sí: ese puede ser el pivot correcto]"
```

---

### D3 — ¿Qué features incluir en el MVP? (Sábado 12-13h)

**Cuándo aparece:** Al definir el scope del MVP y hay más ideas que tiempo.

**Framework: MoSCoW**

```
MUST HAVE (sin esto el MVP no demuestra la propuesta de valor):
→ [Feature] porque [razón directa con propuesta de valor]

SHOULD HAVE (añade valor pero el MVP funciona sin esto):
→ [Feature] porque [razón]

COULD HAVE (sería genial pero no es prioridad):
→ [Feature] — para después del evento

WON'T HAVE (definitivamente fuera del scope):
→ [Feature] — fuera del scope del fin de semana
```

**Criterio de clasificación:**
```
"¿Esta feature demuestra directamente la propuesta de valor?" → MUST
"¿El juez puede ver el valor sin esta feature?" → Si sí: SHOULD o COULD
"¿Esta feature puede simularse manualmente?" → Si sí: COULD o WON'T
"¿Esta feature puede construirse en <4 horas?" → Entonces puede ser MUST si es importante
```

**Pregunta de corte del mentor:**
```
"¿Cuál es la ÚNICA cosa que el usuario debe poder hacer para que los jueces entiendan la propuesta de valor?
Esa va en MUST. Todo lo demás es opcional."
```

---

### D4 — ¿Cuánto cobrar? (Sábado tarde)

**Cuándo aparece:** Al completar el modelo de negocio del Lean Canvas.

**Framework: Evidencia de las entrevistas**

```
DATOS DE LAS ENTREVISTAS:
- Personas que mencionaron precio espontáneamente: ___
- Rango de precios mencionados: $_____ - $_____
- Personas que dijeron "lo pagaría" con número específico: ___
- Alternativa más cara que ya pagan: $_____ / [mes|año|uso]

ANÁLISIS:
- ¿Hay señal de que el precio alto ($___) es aceptable? [Sí/No → evidencia]
- ¿Hay señal de que el precio bajo ($___) parece "muy barato/sospechoso"? [Sí/No]
- ¿El precio alto cubre el CAC estimado en ≤6 meses? [Sí/No → cálculo]
```

**Regla del mentor:**
```
Si no hay datos de entrevistas sobre precio → precio basado en competitor + margen
Si hay datos → usar el percentil 50 de los precios mencionados
Si nadie mencionó precio → el modelo de monetización puede estar equivocado

Pregunta para destrabar:
"¿Cuánto gasta el cliente HOY en resolver esto (aunque sea de forma ineficiente)?
Ese es el techo de precio. ¿El tuyo está por debajo?"
```

---

### D5 — ¿Quién presenta el pitch final? (Domingo mañana)

**Cuándo aparece:** Cuando hay ambigüedad o conflicto sobre quién es el vocero.

**Criterios objetivos (no políticos):**

```
EVALUAR A CADA CANDIDATO EN:
1. Claridad al hablar (¿se entiende sin esfuerzo?) — 1 a 5
2. Energía y convicción (¿creen en el proyecto?) — 1 a 5
3. Conocimiento del negocio (¿puede responder preguntas de jueces?) — 1 a 5
4. Manejo de la presión (¿han presentado antes en público?) — 1 a 5

GANADOR: Quien sume más en los 4 criterios
```

**Si hay empate o conflicto:**
```
"Prueba simple: cada candidato presenta el pitch completo ahora.
El equipo vota de forma anónima en papel.
Se elige al que obtenga más votos. Decisión definitiva."
```

**Regla del mentor:**
```
No tiene que ser quien tuvo la idea original.
No tiene que ser el más senior del equipo.
El presentador es quien hace que los jueces quieran invertir en estas personas.
```

---

### D6 — ¿Cómo llamarse? (En cualquier momento del sábado)

**Esta decisión NO merece más de 10 minutos. Jamás.**

**Proceso rápido:**
```
1. Cada miembro propone 1 nombre (2 minutos)
2. Votar levantando la mano (1 minuto)
3. El que recibe más votos, gana
4. Si hay empate: CEO elige
5. Seguir trabajando
```

**Si el debate se alarga:**
```
Mentor interrumpe:
"El nombre no gana ni pierde un Startup Weekend. ¿Tienen 10 segundos?
→ Eligen el nombre con más votos ahora mismo.
→ Pueden cambiarlo después del evento.
→ Seguimos."
```

---

### D7 — ¿Construir o simular el MVP? (Sábado 12-13h)

**Cuándo aparece:** Los developers quieren construir, el equipo no tiene tiempo.

**Framework de decisión:**

```
¿Cuántas horas de desarrollo tiene el equipo hasta el domingo 13:00?
→ <8 horas: MVP debe ser prototipo (Figma/Concierge)
→ 8-14 horas: App mínima con flujo core
→ >14 horas: App con flujo core + 1-2 features secundarias

¿La propuesta de valor requiere que FUNCIONE de verdad o puede simularse?
→ Requiere funcionar (ej: procesamiento de pagos real): construir
→ Puede simularse (ej: "el sistema envía un WhatsApp"): prototipo es suficiente

¿Los jueces de ESTE evento valoran más la tecnología o la validación de negocio?
→ Más tecnología: construir
→ Más negocio: prototipo + validación fuerte
```

**Preguntas del mentor:**
```
"Si demuestran esto con un prototipo en Figma bien diseñado,
¿los jueces podrán ver la propuesta de valor?"

"¿Cuántas horas de desarrollo van a usar para features que los jueces no van a ver en la demo?"

"¿Cuál es el riesgo mayor: que el MVP no funcione el domingo, o que no tengan validación suficiente?"
```

---

## Protocolo General de Debate (10 minutos)

Para cualquier decisión no listada arriba:

```
[0:00 - 0:30]  MENTOR enuncia la decisión exacta
               "La decisión que toman ahora es: [DECISIÓN EN UNA FRASE]"

[0:30 - 2:00]  POSICIÓN A presenta sin interrupciones
               "¿Quién defiende la opción [A]? Tienes 90 segundos."

[2:00 - 3:30]  POSICIÓN B presenta sin interrupciones
               "¿Quién defiende la opción [B]? Tienes 90 segundos."

[3:30 - 5:30]  MENTOR hace 2-3 preguntas neutrales
               Preguntas que ninguno consideró. Basadas en evidencia o consecuencias.

[5:30 - 7:00]  REVISIÓN DE EVIDENCIA
               "¿Qué datos de sus entrevistas apoyan A vs. B?"
               Si no hay datos: "¿Cuál opción es más reversible?"

[7:00 - 9:00]  RONDA FINAL
               Cada posición tiene 60 segundos para su argumento definitivo.

[9:00 - 10:00] DECISIÓN
               Votación de mano o decisión del CEO.
               Anunciar en voz alta.
               El debate está cerrado.
```

**Regla de oro del mentor:**
```
Si a los 10 minutos el debate no terminó:
"Esta decisión se puede revertir con [COSTO]. ¿Ese costo es aceptable?
Si sí → elegir la opción más fácil de ejecutar y seguir.
Si no → [DECISIÓN DEL CEO] y seguimos."
```

---

## Señales de que el Debate No Está Siendo Productivo

El mentor interviene cuando detecta:

```
🔴 El mismo argumento se repite en diferentes palabras
   → "Ya escuché ese punto. ¿Tienen algo nuevo?"

🔴 El debate es sobre preferencias personales, no sobre el usuario
   → "¿Qué dicen los usuarios que entrevistaron sobre esto?"

🔴 Se está debatiendo un detalle que no impacta al usuario final
   → "¿El usuario final notaría la diferencia entre A y B?
      Si no: elegir la más fácil de implementar y seguir."

🔴 El debate bloquea trabajo que podría estar en progreso
   → "¿Pueden seguir trabajando mientras esto se decide?
      → Sí: asignar la decisión al CEO y que los demás continúen."

🔴 Nadie tiene datos para sustentar su posición
   → "Ninguna de las dos posiciones tiene evidencia.
      Entonces: eligamos la más rápida de probar y la probamos."
```

---

## Después del Debate: Execution Agreement

Una vez tomada la decisión, el mentor genera un acuerdo de ejecución:

```
DECISIÓN TOMADA: [Decisión en 1 frase]
FECHA/HORA: [Cuando se tomó]
RESPONSABLE DE EJECUTAR: [Nombre]
PRÓXIMO HITO: [Qué debe estar listo y cuándo]
SEÑAL DE ÉXITO: [Cómo sabremos que fue la decisión correcta]
CONDICIÓN DE REVISIÓN: [Si [X] pasa, revisamos esta decisión]
```

Este acuerdo se escribe (en el chat del equipo, en Notion, en un papel) para que nadie lo reabra sin nueva evidencia.
