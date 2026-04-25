# Motor de Descubrimiento del Problema

El 70% de los equipos de Startup Weekend trabajan en el problema equivocado porque confunden el síntoma con la causa raíz. Este motor guía al equipo para definir el problema REAL antes de hablar de soluciones.

---

## El Pipeline de Descubrimiento

```
SÍNTOMA → PROBLEMA SUPERFICIAL → CAUSA RAÍZ → CLIENTE REAL → SOLUCIONES → HIPÓTESIS
```

Nunca saltar pasos. Cada nivel construye sobre el anterior.

---

## Nivel 1 — El Síntoma vs. El Problema

### Por qué importa esta distinción

Los equipos suelen describir **síntomas** (lo que ven) en lugar de **problemas** (lo que causa lo que ven). Construir una solución para un síntoma sin entender la causa produce productos que no funcionan.

| Síntoma | Problema real |
|---------|---------------|
| "Los restaurantes pierden reservaciones" | Los dueños no tienen forma de confirmar asistencia con tiempo |
| "La gente no estudia idiomas" | Los métodos actuales no encajan con su horario ni ritmo de vida |
| "Las empresas gastan mucho en software" | Pagan por funciones que no usan porque no pueden personalizar |

### Pregunta del mentor para separar síntoma de problema:

```
"Eso que describieron — ¿es lo que pasa (el síntoma) o es por qué pasa (el problema)?
¿Qué tiene que ser verdad para que [síntoma] ocurra?"
```

---

## Nivel 2 — Los 5 Por Qués (Root Cause Analysis)

### Cómo aplicarlo

Empezar con el síntoma que el equipo describe. Preguntar "¿por qué?" hasta llegar a la causa raíz (típicamente 4-5 iteraciones).

### Ejemplo completo

**Síntoma inicial:** "Los estudiantes universitarios no terminan los cursos en línea"

```
¿Por qué no terminan los cursos?
→ Porque los dejan a la mitad cuando el trabajo se acumula

¿Por qué los dejan cuando se acumula el trabajo?
→ Porque los cursos tienen fechas fijas y no pueden seguirles el ritmo

¿Por qué no pueden seguirles el ritmo con fechas fijas?
→ Porque sus horarios cambian semana a semana y no tienen control sobre cuándo estudiar

¿Por qué no tienen control sobre cuándo estudian?
→ Porque las plataformas no se adaptan al ritmo del estudiante — el contenido es lineal y rígido

¿Por qué el contenido es lineal y rígido?
→ CAUSA RAÍZ: Las plataformas están diseñadas para instructores, no para estudiantes.
El modelo es "el instructor dicta el ritmo" en lugar de "el estudiante elige su ritmo"
```

**Problema real:** Las plataformas de aprendizaje son instructor-centric, no student-centric.
**Solución que tiene sentido:** Plataforma donde el contenido se adapta al ritmo y disponibilidad real del estudiante.

### Template para aplicar con el equipo

```
SÍNTOMA: [Lo que el equipo describe como el problema]

Por qué #1: ¿Por qué pasa [síntoma]?
→ [Respuesta del equipo]

Por qué #2: ¿Por qué pasa [respuesta #1]?
→ [Respuesta del equipo]

Por qué #3: ¿Por qué pasa [respuesta #2]?
→ [Respuesta del equipo]

Por qué #4: ¿Por qué pasa [respuesta #3]?
→ [Respuesta del equipo]

Por qué #5: ¿Por qué pasa [respuesta #4]?
→ CAUSA RAÍZ: [El problema real]

REFORMULACIÓN DEL PROBLEMA:
[Nueva definición del problema basada en la causa raíz]
```

---

## Nivel 3 — El Cliente Real

### Por qué importa definir al cliente con precisión

"Todos" no es un cliente. "Millennials" no es un cliente. Un cliente es una persona específica con un problema específico en una situación específica.

### La técnica del Cliente Perfil

Describir al cliente OBJETIVO como una persona real:

```
NOMBRE: [Nombre ficticio pero representativo]
EDAD: [Rango específico]
TRABAJO/SITUACIÓN: [Qué hace en su día a día]
CONTEXTO: [En qué situación tiene el problema]
FRECUENCIA: [¿Cuántas veces por semana/mes tiene este problema?]
COSTO ACTUAL: [¿Cuánto tiempo/dinero le cuesta el problema hoy?]
SOLUCIÓN ACTUAL: [¿Qué usa hoy para resolverlo?]
FRUSTRACIÓN: [¿Qué le molesta de la solución actual?]
```

**Ejemplo:**
```
NOMBRE: Carlos García
EDAD: 42 años
TRABAJO/SITUACIÓN: Dueño de restaurante de comida italiana en Roma, CDMX.
                   Maneja personalmente el WhatsApp del restaurante.
CONTEXTO: Cada viernes-sábado pierde 3-5 mesas por no-shows que no avisaron.
FRECUENCIA: Cada fin de semana, todas las semanas.
COSTO ACTUAL: ~$8,000 MXN/mes en ingresos perdidos + comida desperdiciada.
SOLUCIÓN ACTUAL: Llama a los clientes el día anterior manualmente. Tarda 45 min.
FRUSTRACIÓN: "No tengo tiempo de llamar a todos, y cuando llamo a veces no contestan."
```

### Preguntas del mentor para construir el perfil del cliente

```
"¿Pueden darme el nombre y apellido de una persona real que conocen con este problema?
No un tipo de persona — una persona específica."

"¿Qué hace esa persona en un día típico de trabajo?
¿En qué momento exacto del día tiene el problema que quieren resolver?"

"¿Cuánto dinero o tiempo pierde por mes a causa de este problema?
¿Cómo lo saben — lo vieron, lo calcularon, o lo están suponiendo?"

"¿Qué hace HOY para resolver este problema, aunque sea de forma imperfecta?
¿Qué es lo más frustrante de esa solución actual?"
```

### Identificar al Early Adopter

El early adopter no es el cliente promedio — es el cliente que SIENTE el problema más intensamente y ESTÁ DISPUESTO a probar soluciones imperfectas.

```
Preguntas para identificar al early adopter:

"¿Quién en tu segmento pierde MÁS por este problema?
¿Quién ya intentó resolverlo por su cuenta, aunque sea de forma manual?"

"¿Hay personas que YA pagan por algo similar, aunque sea una solución mala?"

"¿Quién sería el más emocionado de probar un prototipo imperfecto del producto?"
```

**Señales de que encontraron al early adopter:**
- Mencionan el problema sin que preguntes
- Ya tienen una solución casera (Excel, WhatsApp group, proceso manual)
- Están dispuestos a dar su email o pagar antes de que el producto exista
- Conocen exactamente cuánto les cuesta el problema

---

## Nivel 4 — Mapeo del Espacio de Soluciones

### Por qué hacer esto ANTES de comprometerse con una solución

Los equipos suelen enamorarse de su primera idea. El mapeo del espacio de soluciones les muestra que:
1. Pueden haber múltiples soluciones viables
2. La solución obvia puede no ser la mejor
3. La competencia informa qué NO hacer

### Matriz de soluciones posibles

Para cada problema raíz, mapear:

```
PROBLEMA RAÍZ: [El problema identificado en el Nivel 2]

SOLUCIONES EXISTENTES:
| Solución | Quién la ofrece | Precio | Por qué no resuelve completamente |
|----------|----------------|--------|-----------------------------------|
| [A]      | [Empresa/app]  | $[X]   | [Limitación específica]           |
| [B]      | [Empresa/app]  | $[X]   | [Limitación específica]           |
| [C]      | Manual/artesanal | Gratis | [Por qué es tedioso o ineficiente] |

SOLUCIONES POSIBLES (que podrían existir):
| Solución | Enfoque | Factibilidad en 54h | Diferenciador |
|----------|---------|---------------------|---------------|
| [1]      | [Cómo] | Alta/Media/Baja     | [Qué la hace diferente] |
| [2]      | [Cómo] | Alta/Media/Baja     | [Qué la hace diferente] |
| [3]      | [Cómo] | Alta/Media/Baja     | [Qué la hace diferente] |

SOLUCIÓN ELEGIDA: [Número] porque [razón basada en factibilidad + diferenciación]
```

### Preguntas del mentor para el espacio de soluciones

```
"Busquen ahora mismo en Google, App Store y Product Hunt las primeras 5 soluciones existentes.
¿Por qué alguien usaría la suya en vez de esas?"

"Si tuvieran recursos ilimitados, ¿cuál sería la solución ideal para este problema?
¿Qué partes de esa solución ideal pueden construir en 54 horas?"

"¿Cuál de las soluciones posibles es la más fácil de probar con un usuario real HOY?
No la más completa — la más rápida de validar."
```

---

## Nivel 5 — La Hipótesis Central

### Por qué formular hipótesis en lugar de afirmaciones

Una hipótesis es una creencia que puede ser verdadera o falsa y tiene una forma de verificarse. Las afirmaciones ("los usuarios quieren X") no se pueden falsificar.

### Formato de hipótesis del Startup Weekend

```
HIPÓTESIS DE PROBLEMA:
"Creemos que [CLIENTE ESPECÍFICO] tiene el problema de [DOLOR CONCRETO].
Sabremos que esto es cierto cuando [SEÑAL MEDIBLE DE VALIDACIÓN]."

HIPÓTESIS DE SOLUCIÓN:
"Creemos que [SOLUCIÓN] resolverá el problema porque [RAZÓN].
Sabremos que esto es cierto cuando [SEÑAL MEDIBLE DE VALIDACIÓN]."

HIPÓTESIS DE NEGOCIO:
"Creemos que [CLIENTE] pagará $[PRECIO] por [PROPUESTA DE VALOR].
Sabremos que esto es cierto cuando [ACCIÓN DE COMPRA O PRE-COMPRA]."
```

Después de escribir cada hipótesis, convertirla en un Test Card de 30-90 minutos:

```
Supuesto riesgoso: [Qué debe ser verdad]
Test: [Qué haremos hoy]
Métrica: [Acción observable]
Umbral: [N de M antes de hora]
Decisión si falla: [Pivotar / cambiar segmento / cambiar solución / recortar]
```

**Ejemplo completo:**
```
HIPÓTESIS DE PROBLEMA:
"Creemos que los dueños de restaurantes pequeños (<80 mesas) pierden ingresos
por no-shows porque no tienen un sistema de confirmación eficiente.
Sabremos que esto es cierto cuando 7 de 10 dueños entrevistados
describan este problema con un ejemplo concreto de los últimos 30 días."

HIPÓTESIS DE SOLUCIÓN:
"Creemos que un sistema de confirmación automática por WhatsApp
resolverá el problema porque el 80% de sus clientes ya usa WhatsApp.
Sabremos que esto es cierto cuando 5 de 10 dueños entrevistados
digan que usarían el sistema sin que necesite mucha configuración."

HIPÓTESIS DE NEGOCIO:
"Creemos que los dueños pagarán $299 MXN/mes por este sistema.
Sabremos que esto es cierto cuando 3 de 10 dejen su email para registrarse
o digan un número específico de cuánto pagarían."
```

### Preguntas del mentor para formular hipótesis

```
"Completen esta frase: 'Creemos que [X]. ¿Cómo sabremos que tenemos razón?'"

"Si su hipótesis fuera FALSA, ¿qué verían en las entrevistas?
¿Ya encontraron esas señales?"

"¿Cuál es el supuesto más importante que tiene que ser verdad para que su negocio funcione?
¿Cómo pueden probar ese supuesto en las próximas 3 horas?"

"¿Qué acción observable contaría más que una opinión positiva?
¿Email, referido, demo agendada, piloto, carta de intención o pago?"
```

---

## El Test Final: ¿El Problema Vale la Pena Resolver?

Antes de comprometerse con el fin de semana, hacer esta evaluación rápida:

```
CRITERIO 1 — URGENCIA
"¿El cliente necesita resolverlo HOY o puede esperar meses?"
→ Urgente = Alta propensión a pagar
→ Puede esperar = Producto "nice to have"

CRITERIO 2 — FRECUENCIA
"¿El problema pasa diariamente, semanalmente, o una vez al año?"
→ Diario/semanal = Mayor engagement y retención
→ Anual = Difícil de monetizar con SaaS

CRITERIO 3 — MAGNITUD
"¿El problema le cuesta al cliente tiempo, dinero o bienestar de forma significativa?"
→ Alto costo = Mayor willingness to pay
→ Bajo costo = Difícil justificar el precio

CRITERIO 4 — TAMAÑO DEL MERCADO
"¿Cuántas personas/empresas tienen EXACTAMENTE este problema?"
→ >100,000 personas = Mercado viable
→ <10,000 personas = Nicho muy específico (puede funcionar con ticket alto)

CRITERIO 5 — ACCESIBILIDAD
"¿Pueden llegar a esos clientes fácilmente?"
→ Comunidad online, gremio, red de contactos = Alta accesibilidad
→ Dispersos sin forma de agruparlos = Canal de adquisición costoso
```

**Si 4 de 5 criterios son positivos: el problema vale la pena resolver este fin de semana.**
