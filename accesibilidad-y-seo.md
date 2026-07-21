# Módulo complementario — Accesibilidad y SEO comercial

## Contenido

1. [Cómo funciona este módulo](#cómo-funciona-este-módulo)
2. [Delimitación con el skill `seo`](#delimitación-con-el-skill-seo)
3. [Parte A — Accesibilidad (12 puntos)](#parte-a--accesibilidad-12-puntos)
4. [Parte B — SEO comercial (8 puntos)](#parte-b--seo-comercial-8-puntos)
5. [Interpretación y reporte](#interpretación-y-reporte)
6. [Marco normativo](#marco-normativo)

---

## Cómo funciona este módulo

Se puntúa sobre 20 y **se reporta aparte del score de conversión**. No entra en los 100 puntos.

Esa separación es deliberada. La rúbrica de conversión está calibrada para responder una pregunta —¿por qué este sitio no convierte?— y meterle accesibilidad y SEO dentro diluiría la respuesta. Además son hallazgos de naturaleza distinta: la conversión se argumenta en ingresos, la accesibilidad en alcance y riesgo. Mezclarlas en un número deja las dos peor explicadas.

**Actívalo cuando:** el usuario lo pida; el sitio sea de un sector regulado, público o de salud; el negocio venda a Estados Unidos o la Unión Europea; el cliente ya invierta en tráfico y no esté revisando qué recibe; o cuando durante la auditoría base aparezcan señales evidentes (imágenes sin texto alternativo, encabezados desordenados, metadatos rotos).

**Aplica la misma lógica de rutas y de NE** que el resto del skill. Lo que no se pueda verificar se marca NE, sale del denominador y se declara. La normalización funciona igual: puntos obtenidos sobre puntos evaluables.

**El argumento comercial correcto no es el miedo.** La accesibilidad se vende sola por solapamiento: área táctil suficiente, etiquetas claras, contraste legible y texto que se entiende suben la conversión de todo el mundo, no solo de quien usa lector de pantalla. Un formulario sin etiquetas asociadas falla para un usuario ciego y también para el autocompletado del navegador de todos los demás. Empieza por ahí y deja el cumplimiento normativo como refuerzo, no como amenaza.

---

## Delimitación con el skill `seo`

La parte B cubre **solo la capa observable que toca la conversión**. No es una auditoría SEO.

| Este módulo cubre | El skill `seo` cubre |
|---|---|
| Títulos y meta descripciones como pieza de venta | Rastreo, indexación, `robots.txt`, sitemaps |
| Encabezados como mapa de contenido | Datos estructurados en profundidad y validación de schema |
| Metadatos sociales y tarjeta de compartido | Core Web Vitals e INP |
| Coherencia de URLs, `canonical` y `hreflang` | E-E-A-T y calidad de contenido competitivo |
| Texto alternativo | Keywords, intención de búsqueda, competencia |
| Enlazado interno hacia páginas de conversión | GEO, AI Overviews, crawlers de IA, `llms.txt` |

Si el usuario quiere posicionamiento, no le entregues esta parte como sustituto: dile explícitamente que esto cubre la higiene visible y que el análisis de posicionamiento lo hace el skill `seo`. Ofrecer una capa delgada como si fuera la auditoría completa es la forma más rápida de perder credibilidad en la siguiente reunión.

---

## Parte A — Accesibilidad (12 puntos)

### Qué se verifica en ruta C

Más de lo que parece. Estos elementos aparecen en el contenido extraído de cualquier página:

- **Texto alternativo** de cada imagen, y su calidad.
- **Enlace de salto al contenido** al inicio del documento.
- **Estructura de encabezados**: cuántos `h1` hay, si el orden salta niveles, si los encabezados describen su sección.
- **Texto de enlaces y botones**: si dicen a dónde llevan.
- **Etiquetas de formulario**: si cada campo tiene una.
- **Idioma declarado** y coherencia de `hreflang`.
- **Aviso de apertura en pestaña nueva**.
- **Títulos de página** únicos y descriptivos.

### Qué requiere capturas o navegador

Contraste de color, indicador de foco visible, navegación por teclado, área táctil de los controles, comportamiento al ampliar al 200 %, orden de lectura y respeto a `prefers-reduced-motion`. Sin evidencia visual, estos van a NE.

### Qué requiere herramienta y queda fuera de alcance

Un análisis automatizado completo (axe, Lighthouse, WAVE), la prueba con lector de pantalla real y cualquier declaración formal de conformidad WCAG. **Nunca afirmes que un sitio "cumple WCAG 2.2 AA" con base en esta revisión.** Puedes decir que no encontraste ciertos fallos; no que el sitio conforma. La diferencia importa, y si el cliente la cita en un pliego te va a citar a ti.

### Rúbrica

#### A1 — Texto alternativo — 0 a 3

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

Con lo verificado en el Paso 1e.

| Nota | Ancla |
|---:|---|
| 0 | Sin `og:image` ni `og:description`: el enlace se comparte pelado. |
| 1 | Parciales, o declarados de forma incoherente — por ejemplo `twitter:card: summary_large_image` sin imagen. |
| 2 | Completos y específicos por página, con imagen propia de esa página y no un genérico de marca. |

### S4 — URLs, `canonical` y `hreflang` — 0 a 1

| Nota | Ancla |
|---:|---|
| 0 | Una sección accesible por dos rutas, `canonical` inconsistente, prefijo de idioma que se pierde en algunos enlaces, o `hreflang` que no corresponde entre versiones. |
| 1 | URLs legibles y únicas por sección, `canonical` correcto y versiones de idioma bien enlazadas entre sí. |

---

## Interpretación y reporte

| Bloque | Estado | Lectura |
|---:|---|---|
| 17–20 | Sólido | Higiene resuelta. Lo que quede es afinación. |
| 13–16 | Aceptable | Base correcta con brechas concretas y baratas de cerrar. |
| 8–12 | Débil | El sitio pierde alcance y excluye usuarios por decisiones que nadie revisó. |
| 0–7 | Crítico | Corregir antes de invertir en tráfico: hoy el tráfico llega a un sitio que no lo aprovecha. |

**Cómo presentarlo en el informe:**

- Una línea propia en el veredicto ejecutivo, nunca sumada al score de conversión: *"Conversión 76/100 · Bloque complementario 11/20"*.
- Su propia sección, después del plan de acción, con los hallazgos separados en accesibilidad y SEO comercial.
- Los hallazgos que además afectan conversión —área táctil, etiquetas de formulario, metadatos sociales, títulos— **repórtalos en el cuerpo principal de la auditoría**, no aquí. Aquí van los que son propios del módulo. Un hallazgo se reporta una vez.
- Cierra recordando qué no se evaluó: sin análisis automatizado ni prueba con lector de pantalla, esto es una revisión de indicios, no un dictamen de conformidad.

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
