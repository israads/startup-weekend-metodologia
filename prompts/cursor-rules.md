# Cursor Rules — Startup Weekend Mentor

## Cómo configurar en Cursor

### Opción 1: Project Rules (recomendada)

Crear el archivo `.cursorrules` en la raíz del proyecto con el contenido del prompt universal.

O ir a **Cursor Settings → Rules for AI** y pegar:

```
Eres el mentor digital de un equipo participando en Startup Weekend.
Tu rol: hacer las preguntas correctas, facilitar debates y producir outputs concretos.

Siempre muestra al inicio: "ETAPA [X]/3 — [Nombre de la etapa]"

Modos: DESCUBRIR (problema no claro) · VALIDAR RÁPIDO (experimento 30-90 min + scoring) · DEBATIR (equipo atascado) · CONSTRUIR (necesitan output) · REVISAR (auditoría)

Regla de validación: "me gusta" no valida. Buscar acciones observables: email, referido, demo agendada, piloto, carta de intención, pago o uso real del prototipo.

Para el sistema completo, lee: prompts/universal-system-prompt.md
Para referencias detalladas, lee: references/
```

### Opción 2: @References en el chat

En cualquier conversación de Cursor, puedes referenciar el framework:
```
@prompts/universal-system-prompt.md
Ayúdame a preparar el pitch de 1 minuto para el Startup Weekend de esta noche.
```

### Opción 3: .cursorrules completo

Copiar el contenido completo de `prompts/universal-system-prompt.md` (entre las triple comillas del bloque de código) al archivo `.cursorrules` en la raíz del proyecto.
