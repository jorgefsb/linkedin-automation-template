# Template: Sistema de Créditos

**Por qué:** Siempre dar crédito a autores originales de infografías
**Cómo:** Append estandarizado al final de cada post
**Formato:** Profesional pero no intrusivo

---

## 📋 Formato Estándar

### Cuando conoces al autor original:

```markdown
[CONTENIDO DEL POST]

#Hashtag1 #Hashtag2 #Hashtag3

---
📊 Infografía original por [Nombre Autor]
🔗 Adaptación y análisis por Jorge Suárez
```

**Ejemplo:**
```
[Tu post sobre 12 métricas mobile gaming]

#GameDev #Metrics #MobileGaming

---
📊 Infografía original por @GameDevInsights
🔗 Adaptación y análisis por Jorge Suárez
```

---

### Cuando NO conoces al autor (fuente genérica):

```markdown
[CONTENIDO DEL POST]

#Hashtag1 #Hashtag2 #Hashtag3

---
📊 Fuente: Multiple industry sources
🔗 Análisis por Jorge Suárez
```

---

### Cuando es contenido agregado/compilado:

```markdown
[CONTENIDO DEL POST]

#Hashtag1 #Hashtag2 #Hashtag3

---
📊 Data compilada de: [Source 1, Source 2, Source 3]
🔗 Análisis por Jorge Suárez
```

---

### Cuando la infografía es tuya/de tu equipo:

```markdown
[CONTENIDO DEL POST]

#Hashtag1 #Hashtag2 #Hashtag3

---
📊 Infografía por Jorge Suárez / Sparkplug
🔗 [Link a recurso completo si aplica]
```

---

## 🎯 Variaciones por Plataforma

### LinkedIn (Formato completo):
```
---
📊 Infografía original por @Author
🔗 Adaptación y análisis por Jorge Suárez
🌐 [Link a source si disponible]
```

### Twitter/X (Compacto):
```
---
📊 Original: @Author
🔗 Análisis: @jorgefsb
```

### Instagram/TikTok (En descripción):
```
Credits:
📊 @OriginalAuthor
🔗 Analysis by @jorgefsb

[Link en bio para más info]
```

---

## 🔍 Cómo Encontrar al Autor Original

### Checklist de investigación:

1. **¿La imagen tiene watermark/logo visible?**
   - Sí → Usar ese nombre/handle
   - No → Continuar investigación

2. **¿Hay firma o attribution en la imagen?**
   - Sí → Verificar ese nombre en redes
   - No → Buscar reverse image search

3. **¿De dónde obtuviste la imagen?**
   - Twitter/LinkedIn post → Ver quién posteó primero
   - Website/blog → Dar crédito al site
   - Compartido por alguien → Pedir source

4. **Google Reverse Image Search:**
   - Upload image a Google Images
   - Ver resultados más antiguos
   - Verificar qué fuente parece original

5. **Si no encuentras nada:**
   - Usar template "Multiple industry sources"
   - Mejor ser genérico que atribuir mal

---

## ⚠️ Reglas Importantes

### ✅ SIEMPRE:
- Dar crédito aunque la imagen sea "viral"
- Incluir handle/tag del autor (engagement para ellos)
- Verificar spelling correcto de nombres
- Agregar link a source cuando disponible
- Ser consistente con formato

### ❌ NUNCA:
- Omitir créditos completamente
- Atribuir a fuente incorrecta sin verificar
- Usar "unknown" si puedes investigar
- Dar crédito a agregadores (buscar source original)
- Saltarte este paso por flojera

### 🤔 CASOS EDGE:

**Imagen viral sin autor claro:**
```
📊 Fuente: Widely shared industry infographic
🔗 Análisis por Jorge Suárez

(Si conoces al autor original, por favor tag them 👇)
```

**Múltiples versiones de misma data:**
```
📊 Data compilada de: [Source 1], [Source 2]
🔗 Visualización y análisis por Jorge Suárez
```

**Infografía editada/traducida por ti:**
```
📊 Infografía original por @Author
✏️ Traducción y adaptación por Jorge Suárez
```

---

## 📝 Metadata en creditos.json

Para cada infografía, trackear:

```json
{
  "filename": "nombre-archivo.jpeg",
  "autor_original": "Nombre del Autor",
  "fuente_url": "https://...",
  "handle_twitter": "@author",
  "handle_linkedin": "linkedin.com/in/author",
  "licencia": "CC BY / All Rights Reserved / Unknown",
  "notas": "Cualquier info adicional",
  "verificado": true/false
}
```

**Ver:** `01-infografias/creditos.json` para lista completa

---

## 🎯 Beneficios de Dar Crédito Correcto

### Para ti:
- ✅ Profesionalismo e integridad
- ✅ Respeto en la comunidad
- ✅ Evita problemas legales
- ✅ Networking con autores originales
- ✅ Good karma

### Para el autor original:
- ✅ Reconocimiento merecido
- ✅ Exposure a tu audiencia
- ✅ Posible collaboration futura

### Para la audiencia:
- ✅ Pueden seguir al autor para más content
- ✅ Verificar source original si quieren
- ✅ Trust en tu contenido

---

## 💡 Pro Tips

1. **Mantén lista de autores frecuentes:**
   - Crea un doc con handles de autores que usas seguido
   - Quick copy-paste para créditos

2. **Tagea al autor en post:**
   - Engagement para ellos
   - Posible reshare (más reach para ti)
   - Networking orgánico

3. **Usa creditos.json religiosamente:**
   - Una vez investigado, nunca repitas trabajo
   - Database crece con el tiempo
   - Compártelo con equipo si escala

4. **Agradece en comments:**
   - Si autor comenta o reshares, agradece
   - "¡Gracias @Autor por el contenido original!"
   - Builds relationships

---

## 🚨 Errores Comunes a Evitar

### ❌ Error 1: "No encontré al autor, no pongo nada"
**Correcto:** Usar template de "Multiple industry sources"

### ❌ Error 2: "Es contenido viejo/viral, no importa"
**Correcto:** Precisamente por ser viral, más importante dar crédito

### ❌ Error 3: "Pongo 'créditos al autor' sin nombre"
**Correcto:** Investigar 5 minutos o ser específico que desconoces

### ❌ Error 4: "Solo taggeo si el autor tiene muchos followers"
**Correcto:** Dar crédito independiente de size de audiencia

### ❌ Error 5: "Pongo crédito en imagen, no en caption"
**Correcto:** Crédito debe estar en text del post (visible sin abrir imagen)

---

## 📋 Quick Checklist

Antes de publicar, verifica:

- [ ] ¿Investigué al autor original? (5 min máx)
- [ ] ¿Formato de crédito es correcto?
- [ ] ¿Handle/tag está correcto? (spelling)
- [ ] ¿Actualicé creditos.json con esta info?
- [ ] ¿Licencia permite uso? (si conocida)

**Si todas ✅ → Publish con confianza**

---

**Última actualización:** 2025-12-30
**Incluir en:** TODOS los posts con infografías de terceros
