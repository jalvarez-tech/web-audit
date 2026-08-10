# Módulo complementario — Accesibilidad, SEO comercial y legibilidad para agentes de IA

## Contenido

1. [Cómo funciona este módulo](#cómo-funciona-este-módulo)
2. [Delimitación con el skill `seo`](#delimitación-con-el-skill-seo)
3. [Parte A — Accesibilidad (12 puntos)](#parte-a--accesibilidad-12-puntos)
4. [Parte B — SEO comercial (8 puntos)](#parte-b--seo-comercial-8-puntos)
5. [Parte C — Legibilidad para agentes de IA (AEO) — 5 puntos](#parte-c--legibilidad-para-agentes-de-ia-aeo--5-puntos)
6. [Herramienta: `agentic-seo`](#herramienta-agentic-seo)
7. [Interpretación y reporte](#interpretación-y-reporte)
8. [Marco normativo](#marco-normativo)

---

## Cómo funciona este módulo

Se puntúa sobre 25 —accesibilidad 12, SEO comercial 8, legibilidad para agentes 5— y **se reporta aparte del score de conversión**. No entra en los 100 puntos.

Esa separación es deliberada. La rúbrica de conversión está calibrada para responder una pregunta —¿por qué este sitio no convierte?— y meterle accesibilidad y SEO dentro diluiría la respuesta. Además son hallazgos de naturaleza distinta: la conversión se argumenta en ingresos, la accesibilidad en alcance y riesgo. Mezclarlas en un número deja las dos peor explicadas.

**Actívalo cuando:** el usuario lo pida; el sitio sea de un sector regulado, público o de salud; el negocio venda a Estados Unidos o la Unión Europea; el cliente ya invierta en tráfico y no esté revisando qué recibe; el usuario pregunte por qué su negocio no aparece cuando le preguntan a ChatGPT, Claude, Perplexity o a las respuestas de IA de Google; o cuando durante la auditoría base aparezcan señales evidentes (imágenes sin texto alternativo, encabezados desordenados, metadatos rotos, o una home que devuelve una cáscara vacía al traerla).

**Aplica la misma lógica de rutas y de NE** que el resto del skill. Lo que no se pueda verificar se marca NE, sale del denominador y se declara. La normalización funciona igual: puntos obtenidos sobre puntos evaluables.

**El argumento comercial correcto no es el miedo.** La accesibilidad se vende sola por solapamiento: área táctil suficiente, etiquetas claras, contraste legible y texto que se entiende suben la conversión de todo el mundo, no solo de quien usa lector de pantalla. Un formulario sin etiquetas asociadas falla para un usuario ciego y también para el autocompletado del navegador de todos los demás. Empieza por ahí y deja el cumplimiento normativo como refuerzo, no como amenaza.

---

## Delimitación con el skill `seo`

Las partes B y C cubren **solo la capa observable que toca la conversión**. No son una auditoría SEO.

| Este módulo cubre | El skill `seo` cubre |
|---|---|
| Títulos y meta descripciones como pieza de venta | Rastreo, indexación, sitemaps |
| Encabezados como mapa de contenido | Datos estructurados en profundidad y validación de schema |
| Metadatos sociales y tarjeta de compartido | Core Web Vitals e INP |
| Coherencia de URLs, `canonical` y `hreflang` | E-E-A-T y calidad de contenido competitivo |
| Texto alternativo | Keywords, intención de búsqueda, competencia |
| Enlazado interno hacia páginas de conversión | Estrategia GEO, medición de citaciones en IA, presencia en AI Overviews |
| **Si el sitio es accesible y legible para un agente de IA** (parte C): acceso de crawlers en `robots.txt`, contenido servido sin JavaScript, datos del negocio citables | **Si el sitio merece ser citado**: autoridad, cobertura temática, entidad de marca, competencia por la respuesta |

**El corte entre parte C y el skill `seo` es mecánico:** aquí se verifica lo que se puede comprobar con una petición HTTP —si el agente entra y si lo que recibe sirve—; allá se trabaja la estrategia de por qué te elegiría entre varios. Puerta abierta y despensa llena son cosas distintas, y la parte C solo responde por la puerta.

Si el usuario quiere posicionamiento, no le entregues esta parte como sustituto: dile explícitamente que esto cubre la higiene visible y que el análisis de posicionamiento lo hace el skill `seo`. Ofrecer una capa delgada como si fuera la auditoría completa es la forma más rápida de perder credibilidad en la siguiente reunión.

---

## Parte A — Accesibilidad (12 puntos)

### Qué se verifica en ruta C

Más de lo que parece, pero **depende de la subruta** — aplica la prueba de alcance del extractor del Paso 1b (SKILL.md).

Observable en toda ruta C, incluida C2 (contenido visible):

- **Enlace de salto al contenido** al inicio del documento.
- **Estructura de encabezados**: cuántos `h1` hay, si el orden salta niveles, si los encabezados describen su sección.
- **Texto de enlaces y botones**: si dicen a dónde llevan.
- **Etiquetas de formulario**: si cada campo tiene una.
- **Aviso de apertura en pestaña nueva**.

Requiere subruta C1 (`<head>` presente) o la sonda de imágenes:

- **Texto alternativo** de cada imagen, y su calidad — depende de la **sonda de imágenes**.
- **Títulos de página** únicos y descriptivos (`<title>`) — subruta C1.
- **Idioma declarado** y coherencia de `hreflang` — subruta C1.

En C2, estos tres van a **NE**, nunca a 0.

### Qué requiere capturas o navegador

Contraste de color, indicador de foco visible, navegación por teclado, área táctil de los controles, comportamiento al ampliar al 200 %, orden de lectura y respeto a `prefers-reduced-motion`. Sin evidencia visual, estos van a NE.

### Qué requiere herramienta y queda fuera de alcance

Un análisis automatizado completo (axe, Lighthouse, WAVE), la prueba con lector de pantalla real y cualquier declaración formal de conformidad WCAG. **Nunca afirmes que un sitio "cumple WCAG 2.2 AA" con base en esta revisión.** Puedes decir que no encontraste ciertos fallos; no que el sitio conforma. La diferencia importa, y si el cliente la cita en un pliego te va a citar a ti.

### Rúbrica

#### A1 — Texto alternativo — 0 a 3 · *en ruta C, sujeto a la sonda de imágenes*

| Nota | Ancla |
|---:|---|
| 0 | Imágenes informativas sin `alt`, o `alt` que repite el nombre del archivo (`IMG_8633`, `foto-1`). |
| 1 | Hay `alt` pero genérico o redundante: "imagen", "foto", el mismo texto en todas. |
| 2 | `alt` descriptivo en la mayoría, con vacíos en imágenes secundarias. |
| 3 | `alt` descriptivo y útil en las informativas, vacío en las decorativas, y sin repetir el texto que ya está al lado. |

#### A2 — Encabezados y regiones — 0 a 2

| Nota | Ancla |
|---:|---|
| 0 | Sin `h1`, con varios `h1`, o encabezados usados por tamaño visual y no por jerarquía. |
| 1 | Jerarquía razonable con saltos de nivel o encabezados vacíos. |
| 2 | Un `h1` por página, jerarquía sin saltos, enlace de salto al contenido presente y regiones identificables. |

#### A3 — Texto de enlaces y botones — 0 a 2

| Nota | Ancla |
|---:|---|
| 0 | Enlaces sin nombre accesible, etiquetas que renderizan la ruta literal, o "clic aquí" / "leer más" repetidos sin contexto. |
| 1 | Mayormente descriptivos, con excepciones en iconos o enlaces de imagen. |
| 2 | Cada enlace y botón se entiende fuera de contexto, incluidos los de solo icono. |

#### A4 — Formularios etiquetados — 0 a 2

| Nota | Ancla |
|---:|---|
| 0 | Campos identificados solo por texto de marcador de posición, o sin etiqueta alguna. |
| 1 | Etiquetas presentes pero sin instrucciones ni manejo visible de error. |
| 2 | Etiqueta por campo, formato esperado indicado, y errores explicados en texto y no solo por color. |

#### A5 — Contraste y legibilidad — 0 a 2 · *requiere evidencia visual*

| Nota | Ancla |
|---:|---|
| 0 | Texto por debajo del contraste mínimo, o texto sobre imagen sin capa de refuerzo. |
| 1 | Cuerpo de texto legible con problemas en textos secundarios, estados o texto sobre fondo variable. |
| 2 | Contraste suficiente en todo el contenido y en los estados de los controles. |

#### A6 — Foco, teclado y área táctil — 0 a 1 · *requiere evidencia visual*

| Nota | Ancla |
|---:|---|
| 0 | Foco invisible, trampas de teclado, o controles con área táctil insuficiente. |
| 1 | Foco visible, recorrido por teclado completo y controles cómodos de accionar. |

---

## Parte B — SEO comercial (8 puntos)

### S1 — Títulos y meta descripciones — 0 a 3

Revísalos en todas las páginas traídas. Este criterio castiga fuerte porque son la primera pieza de venta del sitio y viven fuera de él.

| Nota | Ancla |
|---:|---|
| 0 | Faltan, están duplicadas entre páginas, o contienen notas internas de desarrollo, nombres de máquina o descripciones de contenido que la página no tiene. |
| 1 | Presentes y únicas pero genéricas: repiten el nombre de la página sin ninguna razón para hacer clic. |
| 2 | Descriptivas y únicas, sin argumento comercial ni llamado. |
| 3 | Únicas, con la promesa concreta de la página y una razón para hacer clic, en la longitud que no se corta. |

Una meta descripción con notas de build es un 0 automático, aunque el resto esté bien. Es texto de desarrollo publicado como argumento de venta.

### S2 — Encabezados como mapa de contenido — 0 a 2

Distinto de A2: aquí no importa la jerarquía técnica sino si los encabezados responden lo que el visitante vino a resolver.

| Nota | Ancla |
|---:|---|
| 0 | Encabezados decorativos o de marca que no dicen de qué trata la sección. |
| 1 | Descriptivos pero centrados en la empresa, no en la pregunta del usuario. |
| 2 | El `h1` refleja la intención de la página y los `h2` recorren las preguntas reales del segmento. |

### S3 — Metadatos sociales — 0 a 2

Con lo verificado en el Paso 1e. El ancla 0 solo puede asignarse en rutas A, B o C1; en **C2 el criterio es NE, nunca 0** (no viste el `<head>`, no que falte).

| Nota | Ancla |
|---:|---|
| 0 | Sin `og:image` ni `og:description`: el enlace se comparte pelado. |
| 1 | Parciales, o declarados de forma incoherente — por ejemplo `twitter:card: summary_large_image` sin imagen. |
| 2 | Completos y específicos por página, con imagen propia de esa página y no un genérico de marca. |

### S4 — URLs, `canonical` y `hreflang` — 0 a 1

`canonical` y `hreflang` viven en el `<head>`: el ancla 0 solo puede asignarse en rutas A, B o C1; en **C2 es NE, nunca 0**. La duplicación de rutas y el prefijo de idioma perdido sí se ven en el contenido de cualquier ruta.

| Nota | Ancla |
|---:|---|
| 0 | Una sección accesible por dos rutas, `canonical` inconsistente, prefijo de idioma que se pierde en algunos enlaces, o `hreflang` que no corresponde entre versiones. |
| 1 | URLs legibles y únicas por sección, `canonical` correcto y versiones de idioma bien enlazadas entre sí. |

---

## Parte C — Legibilidad para agentes de IA (AEO) — 5 puntos

Adaptado del marco **Agentic Engine Optimization** de `agentic-seo` (Addy Osmani, MIT — <https://github.com/addyosmani/agentic-seo>), reducido a lo que aplica a un sitio comercial. Ver [Herramienta: `agentic-seo`](#herramienta-agentic-seo) para correrlo y para sus límites.

**El argumento comercial, en una frase:** una parte creciente de las consultas de compra ya no empieza en el buscador sino en un asistente —"¿cuál es la mejor clínica dental en Medellín?", "¿quién instala paneles solares en Bogotá y cuánto cuesta?"—. Ese asistente hace **una sola petición HTTP**, casi nunca ejecuta JavaScript, y descarta lo que no entiende. No hay segunda oportunidad ni sesión de navegación. Si el sitio no responde bien a esa única petición, el negocio no está en la conversación: no aparece mal posicionado, sencillamente no existe.

Eso lo vuelve un criterio de **adquisición**, no de higiene técnica, y por eso se puntúa. Pero se puntúa bajo —5 puntos— por una razón honesta que debes trasladar al cliente: es una práctica emergente, sin datos de atribución maduros. Preséntalo como un canal que se está abriendo y que hoy cuesta poco dejar abierto, nunca como una urgencia con cifras inventadas detrás.

### C1 — Acceso de los crawlers de IA — 0 a 2

Se lee del `robots.txt` (observable en toda ruta: tráelo directamente en `/robots.txt`). Agentes a verificar: `GPTBot` y `ChatGPT-User` (OpenAI), `ClaudeBot` y `Claude-Web` (Anthropic), `PerplexityBot`, `Google-Extended` y `GoogleOther`, `Amazonbot`, `Bytespider`, `cohere-ai`.

| Nota | Ancla |
|---:|---|
| 0 | Los agentes de IA están bloqueados —`Disallow: /` global, o reglas específicas contra ellos— sin que nadie en el negocio lo haya decidido. Suele venir por defecto en la plantilla, en el plugin de SEO o en el WAF, y deja al sitio fuera de las respuestas de IA sin que el dueño lo sepa. |
| 1 | Bloqueo parcial o incoherente —unos agentes sí y otros no, sin criterio— o `robots.txt` ausente, vacío o con errores de sintaxis que lo vuelven impredecible. |
| 2 | Los agentes relevantes pueden rastrear el sitio; o están bloqueados **por decisión deliberada y explicable** del negocio (contenido de pago, catálogo que no se quiere replicar). Ambas cosas puntúan igual: lo que se evalúa es que la puerta esté como el dueño quiere, no que esté abierta. |

**Dos precisiones para no fabricar hallazgos.** Primero: la ausencia de reglas `Allow:` explícitas para agentes de IA **no es un defecto**. `agentic-seo` las premia como refuerzo, pero técnicamente un `robots.txt` sin prohibiciones ya permite el rastreo completo; reportarlo como falla es inventar un problema. Menciónalo como mejora opcional de bajo esfuerzo, jamás como ancla 0. Segundo: `robots.txt` es lo único que puedes verificar por HTTP. Un bloqueo por WAF, por Cloudflare o por reglas de servidor **no aparece ahí** — si lo sospechas, dilo como hipótesis y pide al cliente los registros del servidor. No lo afirmes.

### C2 — Contenido servido sin JavaScript — 0 a 2

El criterio con más consecuencia comercial de esta parte, y el más barato de verificar: trae el HTML crudo de la home y de la página de conversión (`curl -sL <url>`) y comprueba si el contenido que vende —titular, oferta, precios, teléfono, disponibilidad— viene en esa primera respuesta o si llega después por JavaScript.

| Nota | Ancla |
|---:|---|
| 0 | La primera respuesta es una cáscara: `<div id="root">` vacío, o solo menú y pie. Un asistente que traiga la URL no recibe nada que citar. El mismo problema afecta a la tarjeta de compartido en WhatsApp y a cualquier lector que no ejecute JavaScript. |
| 1 | Llega el marco —titular, navegación, texto institucional— pero lo decisivo se carga aparte: precios, fichas de producto, disponibilidad, preguntas frecuentes, testimonios. El agente recibe una descripción genérica del negocio y ningún dato para recomendarlo. |
| 2 | El contenido comercial de cada página está en el HTML de la primera respuesta. |

**Este criterio se conecta con la detección de ruta del Paso 1b.** Si al traer el sitio recibiste una cáscara vacía, eso no es solo una limitación de tu herramienta: es el hallazgo. Repórtalo con la evidencia exacta —la URL, el tamaño del HTML devuelto y qué contenía— y llévalo también al cuerpo principal de la auditoría, porque afecta al compartido en WhatsApp (Paso 1e), que sí es conversión.

### C3 — Datos del negocio citables — 0 a 1

Un asistente solo puede recomendar lo que puede leer y repetir sin ambigüedad. Esto se evalúa sobre el texto, no sobre archivos especiales.

| Nota | Ancla |
|---:|---|
| 0 | Los datos que un asistente necesita para recomendar el negocio —qué vende, dónde opera, a qué precio o rango, cómo se contacta, qué lo diferencia— viven en imágenes, PDFs o carruseles, o se contradicen entre páginas (teléfonos distintos, cobertura distinta, precios distintos). |
| 1 | Datos en texto plano, idénticos entre páginas, con encabezados que aíslan cada respuesta —preguntas frecuentes reales, cobertura, precios o rango, condiciones— y nombre, dirección y teléfono consistentes en todo el sitio. |

Un `llms.txt` bien formado (índice en Markdown con descripciones, según <https://llmstxt.org>) **suma como señal y nunca es requisito**: es un estándar propuesto que hoy ningún motor grande consume de forma confirmada. Si existe y está bien hecho, respáldalo en el ancla 1. Si no existe, no restes — y no lo recomiendes antes que C2, que sí decide si hay algo que indexar.

### Extras de `agentic-seo` que normalmente son NA

`agentic-seo` audita sitios de documentación técnica consumidos por agentes de programación. Estos cinco checks suyos **no aplican a un sitio comercial** y se marcan **NA**, nunca 0 — aplicando la regla de calidad 11 del skill, la misma por la que un despacho de abogados no pierde puntos por no tener carrito:

| Check de `agentic-seo` | Qué evalúa | Cuándo sí evaluarlo |
|---|---|---|
| `skill-md` | `skill.md` describiendo capacidades, entradas y límites | El producto es una API, un SaaS con integraciones o una herramienta para desarrolladores |
| `agents-md` | `AGENTS.md` / `CLAUDE.md` con contexto del proyecto | Igual que el anterior, y solo si el repositorio es público |
| `agent-permissions` | `agent-permissions.json` con reglas de acceso y límites de tasa | Producto con API pública y necesidad real de gobernar clientes automatizados |
| `markdown-availability` | Fuente en Markdown junto al HTML | El sitio es documentación técnica |
| `copy-for-ai` | Botones "copiar para IA" y enlaces a la vista cruda | El sitio es documentación técnica |

Si el sitio auditado **sí** es de producto técnico —SaaS, API, herramienta para desarrolladores—, actívalos como chequeos cualitativos dentro de C3 y repórtalos en prosa. **No añadas puntos por ellos:** la parte C se mantiene en 5 para que dos auditorías de negocios distintos sigan siendo comparables, que es el mismo principio de los módulos de vertical.

El check `token-budget` (peso de página en tokens) tampoco se puntúa aquí: en un sitio comercial las páginas rara vez se acercan al umbral, y cuando el problema existe ya lo captura la velocidad (subcriterio 7.4 de la rúbrica base).

---

## Herramienta: `agentic-seo`

`npx agentic-seo` corre los chequeos AEO sin API key ni instalación previa. Úsalo **solo si tienes Bash y Node ≥ 18**; si no, la parte C se evalúa igual a mano con `curl` sobre `/robots.txt` y sobre la home — los tres criterios están escritos para ser verificables sin la herramienta.

### Regla dura — nunca publiques su score

**Verificado corriéndolo contra un sitio comercial real:** en modo `--url`, cinco de sus diez checks no pueden ejecutarse (necesitan el directorio de archivos del sitio) y **puntúan 0 en lugar de marcarse como no evaluados**. El resultado fue **9/100, grado F** en un sitio sano. Ese número no mide el sitio, mide el modo de ejecución.

Por lo tanto:

- **Nunca lleves su score, su porcentaje ni su letra a un informe de cliente.** Ni siquiera como referencia con nota al pie.
- Usa **solo los hallazgos de los checks que sí corrieron**, y solo como evidencia para C1 y C3.
- Trata sus recomendaciones como directrices, no como veredictos. El propio proyecto lo advierte en su descargo de responsabilidad.

### Qué sirve en cada modo

| Modo | Comando | Qué se puede usar |
|---|---|---|
| **URL en vivo** — el caso normal al auditar el sitio de un cliente | `npx agentic-seo --url https://sitio.com --json` | Únicamente `robots-txt` y `llms-txt` (más `agents-md`, `skill-md` y `agent-permissions`, casi siempre NA). Todo lo demás devuelve "No local directory available" y hay que descartarlo. |
| **Directorio local** — cuando el sitio es tuyo o tienes el build | `npx agentic-seo ./build` | Los diez checks. Aun así, aplica la tabla de NA de arriba antes de reportar nada. |
| **Servidor local** | `npx agentic-seo --serve ./build` | Los diez, con los chequeos por HTTP sobre el sitio servido. |

Para quedarte solo con lo utilizable en modo URL:

```bash
npx --yes agentic-seo --url https://sitio.com --checks robots-txt,llms-txt --json
```

### Cómo reportarlo

Etiqueta la evidencia como **observada con herramienta**, nombrando cuál y con qué fecha —igual que con PageSpeed en el Paso 1f—: *"robots.txt permite ClaudeBot, GPTBot y PerplexityBot (verificado con `agentic-seo v1.0`, 2026-08-09)"*. Si la herramienta falló o no estaba disponible, dilo y reporta la verificación manual con `curl`; nunca dejes ambiguo de dónde salió el dato.

---

## Interpretación y reporte

| Bloque | Estado | Lectura |
|---:|---|---|
| 21–25 | Sólido | Higiene resuelta. Lo que quede es afinación. |
| 16–20 | Aceptable | Base correcta con brechas concretas y baratas de cerrar. |
| 10–15 | Débil | El sitio pierde alcance y excluye usuarios por decisiones que nadie revisó. |
| 0–9 | Crítico | Corregir antes de invertir en tráfico: hoy el tráfico llega a un sitio que no lo aprovecha. |

**Cómo presentarlo en el informe:**

- Una línea propia en el veredicto ejecutivo, nunca sumada al score de conversión: *"Conversión 76/100 · Bloque complementario 14/25"*.
- Su propia sección, después del plan de acción, con los hallazgos separados en accesibilidad, SEO comercial y legibilidad para agentes.
- Los hallazgos que además afectan conversión —área táctil, etiquetas de formulario, metadatos sociales, títulos, y el contenido que no llega sin JavaScript— **repórtalos en el cuerpo principal de la auditoría**, no aquí. Aquí van los que son propios del módulo. Un hallazgo se reporta una vez.
- Cierra recordando qué no se evaluó: sin análisis automatizado ni prueba con lector de pantalla, esto es una revisión de indicios, no un dictamen de conformidad. Para la parte C, añade que mide **si el sitio es legible para un agente**, no si termina siendo citado — eso depende de autoridad y competencia, y corresponde al skill `seo`.

---

## Marco normativo

Orientación general para dimensionar el riesgo, **no concepto jurídico**. Recomienda siempre validación legal antes de que el cliente tome decisiones basadas en esto.

| Ámbito | Referencia | A quién alcanza |
|---|---|---|
| Colombia | Ley 1618 de 2013 y Resolución 1519 de 2020 (MinTIC) | Los criterios de accesibilidad digital de la Resolución 1519 se dirigen a entidades del sector público. Para el sector privado no existe un mandato general equivalente. |
| Estados Unidos | ADA, Título III | El riesgo es principalmente litigioso y afecta a sitios comerciales que atienden público estadounidense. |
| Unión Europea | Directiva (UE) 2019/882 — Acta Europea de Accesibilidad | Alcanza a ciertos productos y servicios del sector privado, incluido el comercio electrónico. |
| Estándar técnico | WCAG 2.2, nivel AA | Es la referencia que citan casi todos los marcos anteriores. |

Encuadre correcto para el cliente: si vende solo en Colombia y es sector privado, el argumento es de alcance de mercado y de conversión, no de obligación. Si vende a Estados Unidos o Europa, la exposición cambia y conviene revisarlo con un abogado. Decirlo así —en lugar de insinuar sanciones genéricas— es más honesto y, en la práctica, más persuasivo.
