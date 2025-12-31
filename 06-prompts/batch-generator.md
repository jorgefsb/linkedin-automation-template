# Prompt: Batch Post Generator

**Propósito:** Generar 4-5 variaciones de posts a partir de una sola infografía
**Input:** Infografía (descripción o path)
**Output:** 4-5 posts completos en diferentes formatos
**Uso:** `claude --prompt batch-generator.md --context "infografia: [path]"`

---

## INSTRUCCIONES PARA CLAUDE

Vas a generar **4-5 posts de LinkedIn en español** basados en la infografía proporcionada.

### CONTEXTO:
- **Autor:** Jorge Suárez (GM Amber Studio México, CEO Sparkplug)
- **Audiencia:** Gamedevs, entrepreneurs, marketers, industry professionals
- **Objetivo:** Engagement alto + Thought leadership
- **Distribución:** 80% Marca Personal, 15% Sparkplug, 5% Amber

### INPUTS QUE RECIBIRÁS:
1. **Infografía:** Path al archivo o descripción del contenido
2. **Categoría:** metricas / game-design / retencion / monetizacion / roblox / marketing / career / business
3. **(Opcional) Tema específico:** Si se requiere enfoque particular

---

## FORMATO DE OUTPUT:

Genera **4 posts** usando estos formatos (uno de cada tipo):

### POST 1: EDUCATIVO
**Ver:** `../02-templates/post-templates/educational.md`

**Estructura:**
```
Hook: [Experiencia personal + promesa de valor]

Body:
1. **[Concepto]** - [Explicación 1 línea]
2. **[Concepto]** - [Explicación 1 línea]
...
[5-10 items dependiendo del contenido]

CTA: [Pregunta engagement + insight adicional]

#[5-6 hashtags]

---
📊 [Crédito según creditos.json]
🔗 Análisis por Jorge Suárez
```

**Ejemplo:**
```
Después de 20 años haciendo videojuegos, te puedo decir que no es magia...
son 10 trucos psicológicos que todos los juegos exitosos usan para engancharte. 🎮

Aquí están:

1. **Variable Rewards** - Por qué los loot boxes funcionan
2. **Progress Bars** - El poder de "casi terminar"
...

¿Cuál de estos te ha enganchado más a ti? Comenta 👇

PD: Si estás haciendo un juego y NO usas estos... lo estás haciendo en modo difícil.

#GameDesign #GameDev #Psychology #MobileGames #Gaming

---
📊 Fuente: Multiple industry sources
🔗 Análisis por Jorge Suárez
```

---

### POST 2: DATA-DRIVEN
**Ver:** `../02-templates/post-templates/data-driven.md`

**Estructura:**
```
Hook: [Pregunta + preview de insight]

Body:
**[Métrica/Categoría]:**
- 🔴 Bad: [Rango]
- 🟡 Good: [Rango]
- 🟢 Great: [Rango]

[Repetir 3-5 métricas]

Takeaway: [Regla de oro memorable]

CTA: [Pregunta comparativa]

#[5-6 hashtags]

---
📊 [Crédito]
🔗 Análisis por Jorge Suárez
```

**Ejemplo:**
```
¿Qué tan bueno es tu mobile game... realmente? 📊

Estos son los benchmarks de los TOP titles (datos 2025):

**D1 Retention:**
- 🔴 Bad: <30%
- 🟡 Good: 35-40%
- 🟢 Great: >45%

...

La regla de oro: LTV debe ser 3X tu CAC. Si no... Houston, tenemos un problema.

¿Dónde están tus métricas? (Sé honesto 😅)

#MobileGaming #Metrics #GameDev #Benchmarking

---
📊 Fuente: Industry benchmarks 2025
🔗 Análisis por Jorge Suárez
```

---

### POST 3: HOT TAKE
**Ver:** `../02-templates/post-templates/hot-take.md`

**Estructura:**
```
Hook: [Opinión controversial/insight provocativo]

Setup: [Analogía o contexto]

Reveal:
[Estructura de capas o progresión]

Punch Line: [Statement fuerte que resume todo]

CTA: [Pregunta que invite debate]

#[5-6 hashtags]

---
📊 [Crédito]
🔗 Análisis por Jorge Suárez
```

**Ejemplo:**
```
El 90% del game design NO lo ves cuando juegas. 🧊

Es como un iceberg. La mayoría solo ve la punta.

SUPERFICIE (Lo obvio):
- Gráficos
- Historia
- UI

PROFUNDO (Lo que NUNCA notas):
- Psychology triggers
- Retention mechanics
- Addiction patterns (ethically designed)

La diferencia entre un juego 'bueno' y uno que genera $10M/mes...
está en la profundidad del iceberg.

¿Qué capa dominas tú mejor?

#GameDesign #Psychology #UXDesign

---
📊 Fuente: Game design frameworks
🔗 Análisis por Jorge Suárez
```

---

### POST 4: CASE STUDY
**Ver:** `../02-templates/post-templates/case-study.md`

**Estructura:**
```
Hook: [Marca/Resultado + promesa de breakdown]

Examples:
**1. [Nombre]** - [Métrica]
   - Insight: [Qué hicieron bien]
**2. [Nombre]** - [Métrica]
   - Insight: [Qué hicieron bien]
...

Patterns:
**Los patrones de éxito:**
- ✅ [Patrón 1]
- ✅ [Patrón 2]
...

Why It Matters:
**Por qué importa:**
- [Estadística mercado]
- [Comparación métodos tradicionales]
- [ROI]

CTA: [Soft pitch conectando expertise]

#[5-6 hashtags + #Brandcade si aplica]

---
📊 [Crédito]
🔗 Análisis por Jorge Suárez
```

**Ejemplo:**
```
Marcas como Nike, Gucci, y Walmart están generando millones de interacciones en Roblox. 👟

Aquí está el Top 10 de branded games y qué puedes aprender:

**1. Nike (Nikeland)** - 25M+ visitas
   - Insight: Gamificación de productos físicos
**2. Gucci Town** - 15M+ visitas
   - Insight: Experiencias exclusivas > solo venta

Los patrones de éxito:
- ✅ No es un "anuncio" - es una experiencia
- ✅ Items virtuales exclusivos
- ✅ Events recurrentes

Por qué importa:
- Gen Z pasa 2.5 horas/día en Roblox
- 1 branded experience > 100 anuncios tradicionales

En Brandcade, ayudamos a marcas a crear estas experiencias.
¿Tu marca ya está en Roblox?

#Roblox #BrandedGames #Marketing #Brandcade

---
📊 Fuente: Roblox platform data
🔗 Análisis por Jorge Suárez
```

---

## REGLAS CRÍTICAS:

### ✅ SIEMPRE:
1. **Español mexicano:** Casual pero profesional
2. **Voz de Jorge:** "Después de 20 años...", "La neta...", "Hot take:"
3. **Data específica:** Números concretos, no vagos
4. **CTA engagement:** Invitar a conversación
5. **Créditos:** Usar info de creditos.json
6. **Hashtags:** 5-6 relevantes (no más)
7. **Longitud:** 150-250 palabras por post

### ❌ NUNCA:
1. **Tono corporativo** o formal
2. **Humble bragging** disfrazado
3. **Clickbait** sin sustancia
4. **Atacar** competidores
5. **Mezclar** Amber/Sparkplug sin separación
6. **Inventar** data sin disclaimer

---

## VARIACIÓN ENTRE POSTS:

**Asegúrate de que los 4 posts sean DIFERENTES:**
- Post 1: Formato lista educativo
- Post 2: Benchmarks/ranges
- Post 3: Opinión/insight provocativo
- Post 4: Ejemplos reales/cases

**NO repitas:**
- Mismo hook
- Misma estructura
- Mismo CTA
- Mismos hashtags exactos

---

## ADAPTACIÓN POR CATEGORÍA:

### Si categoría = ROBLOX:
- Mencionar Brandcade si es case study
- Focus en Gen Z/branded games
- Conectar con marketing/marcas

### Si categoría = METRICAS:
- Usar benchmarks y ranges
- Incluir "regla de oro"
- Dirigir a founders/PMs

### Si categoría = GAME-DESIGN:
- Focus en frameworks
- Educar sobre principios
- Audiencia: gamedevs

### Si categoría = RETENTION:
- Psychology angle
- Behavioral economics
- Tips accionables

---

## FORMATO FINAL DE ENTREGA:

Entregar en este formato:

```markdown
# BATCH DE POSTS - [Nombre Infografía]

**Categoría:** [categoria]
**Total posts generados:** 4
**Fecha:** [fecha]

---

## POST 1: Educativo

[Post completo aquí]

**Formato:** Educational
**Plataforma recomendada:** LinkedIn
**Objetivo:** Engagement + Teaching

---

## POST 2: Data-Driven

[Post completo aquí]

**Formato:** Data-driven
**Plataforma recomendada:** LinkedIn
**Objetivo:** Credibility + Leads B2B

---

## POST 3: Hot Take

[Post completo aquí]

**Formato:** Hot take
**Plataforma recomendada:** LinkedIn + Twitter
**Objetivo:** Engagement masivo + Debate

---

## POST 4: Case Study

[Post completo aquí]

**Formato:** Case study
**Plataforma recomendada:** LinkedIn
**Objetivo:** Lead generation + Authority

---

## METADATA:

- **Infografía original:** [filename]
- **Créditos verificados:** [Yes/No - según creditos.json]
- **Categoría:** [categoria]
- **Keywords:** [3-5 keywords principales]
- **Estimated engagement:** [Based on content type]
- **Ready to publish:** [Yes/Needs review]
```

---

## EJEMPLO DE USO:

```bash
# Generar batch de una infografía específica
claude --prompt 06-prompts/batch-generator.md \
       --context "infografia: 01-infografias/catalogadas/metricas/12-key-money-metrics.jpeg, categoria: metricas"

# Output: 4 posts listos para publicar
```

---

**Última actualización:** 2025-12-30
**Versión:** 1.0
