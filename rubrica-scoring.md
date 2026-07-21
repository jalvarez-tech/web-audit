# Rúbrica de puntuación con anclas de calibración

## Contenido

1. [Cómo usar esta rúbrica](#cómo-usar-esta-rúbrica)
2. [Distribución de referencia](#distribución-de-referencia)
3. [Categoría 1 — Posicionamiento y claridad (15)](#categoría-1--posicionamiento-y-claridad-15-puntos)
4. [Categoría 2 — Mensaje y contenido persuasivo (15)](#categoría-2--mensaje-y-contenido-persuasivo-15-puntos)
5. [Categoría 3 — Estructura y navegación (12)](#categoría-3--estructura-y-navegación-12-puntos)
6. [Categoría 4 — Credibilidad y confianza (12)](#categoría-4--credibilidad-y-confianza-12-puntos)
7. [Categoría 5 — CTA y capacidad de conversión (15)](#categoría-5--cta-y-capacidad-de-conversión-15-puntos)
8. [Categoría 6 — Embudo de ventas (15)](#categoría-6--embudo-de-ventas-15-puntos)
9. [Categoría 7 — Experiencia móvil y usabilidad (8)](#categoría-7--experiencia-móvil-y-usabilidad-8-puntos)
10. [Categoría 8 — Automatización y medición (8)](#categoría-8--automatización-y-medición-8-puntos)
11. [Interpretación del score](#interpretación-del-score)

---

## Cómo usar esta rúbrica

Puntúa cada subcriterio contra su ancla, no contra tu impresión general del sitio. La impresión general es exactamente el sesgo que estas anclas existen para corregir: un sitio con buen diseño arrastra hacia arriba todas las notas si no te obligas a mirar cada criterio por separado.

Para cada subcriterio, **escribe la evidencia antes que el número**. Si no puedes citar algo concreto del sitio que justifique la nota, la nota está mal.

**Desempate en anclas 1–2:** varias anclas colapsan las notas 1 y 2 en una sola fila. Asigna **2** solo si tu línea de evidencia cita algo concreto del sitio que apunte parcialmente al ancla del nivel 3 de ese subcriterio; si la evidencia solo confirma el ancla 1–2, asigna **1**. Así el desempate queda sujeto al mismo mecanismo de evidencia escrita que el resto de la rúbrica.

**Regla de viewport.** Todo subcriterio que dependa del fold o del peso visual (1.5, 5.1, 5.2) se evalúa por defecto sobre el **viewport móvil** cuando exista evidencia móvil —la captura de la parte superior en móvil del Paso 0, o navegador redimensionado a ~375 px—. La versión de escritorio es secundaria: si ambos folds divergen (CTA visible en escritorio pero no en móvil, propuesta de valor empujada bajo el fold móvil), la nota la fija la versión móvil y la divergencia se reporta como hallazgo con prioridad propia. Sin evidencia visual móvil, evalúa sobre la evidencia disponible (captura de escritorio u orden del contenido extraído) y decláralo en el campo "Evidencia visual" de la ficha técnica y en la nota de alcance. En 5.1, la regla aplica solo a su dimensión visual (dominancia del CTA en pantalla), no a la textual.

Tres marcas posibles además del número:

- **NE (no evaluado)** — falta evidencia. No cuenta ni en obtenidos ni en evaluables.
- **NA (no aplica)** — irrelevante para el modelo de negocio. Tampoco cuenta.
- **0** — se pudo evaluar y está mal. Esto sí cuenta.

Confundir NE con 0 es el error más común y el más caro: produce informes que castigan al cliente por límites de tu propia auditoría.

**NE descuenta de la cobertura; NA descuenta de la base aplicable. No los mezcles al reportar** (ver la normalización del Paso 3 en SKILL.md): la cobertura mide lo que no pudiste ver, no lo que no aplica al modelo de negocio.

---

## Distribución de referencia

Los modelos de lenguaje tienden a agrupar puntuaciones entre 60 y 75 porque promediar hacia el centro se siente prudente. No es prudente: es inútil. Un informe donde todos los sitios sacan 68 no orienta ninguna decisión.

De cada diez sitios de PyME o profesional independiente auditados con esta rúbrica, la distribución esperada se acerca a:

| Rango | Sitios esperados de cada 10 |
|---|---|
| 90–100 | 0 |
| 75–89 | 1 |
| 60–74 | 3 |
| 40–59 | 4 |
| 0–39 | 2 |

**El caso típico está entre 40 y 59.** Un sitio corporativo estándar —hecho por una agencia, visualmente correcto, con titular genérico, sin prueba social específica, con formulario de contacto de siete campos y sin oferta intermedia— es un 45–55. No un 70.

Distribución calibrada sobre PyME y profesional independiente. Con un módulo de vertical activo, los tres controles anti-inflación de abajo siguen aplicando; justifica cada nota contra las anclas **ajustadas por el módulo**, no contra las de la rúbrica base.

Antes de cerrar el score, aplica estos tres controles:

1. ¿Le pusiste más de 3 sobre 4 a algún criterio? Justifica con evidencia citada o baja la nota.
2. ¿Tu total quedó entre 65 y 75? Revisa si estás promediando por comodidad.
3. ¿El sitio tiene titular genérico y sin prueba social específica? Entonces las categorías 1, 2 y 4 no pueden sumar más del 55 % de sus máximos.

---

## Categoría 1 — Posicionamiento y claridad (15 puntos)

### 1.1 Cliente ideal claramente identificado — 0 a 4

| Nota | Ancla |
|---:|---|
| 0 | No se identifica a nadie. "Soluciones para empresas y personas." |
| 1–2 | Segmento amplio e implícito, deducible solo tras leer varias secciones. |
| 3 | Segmento nombrado pero genérico: "pequeñas empresas", "profesionales". |
| 4 | Segmento específico y nombrado arriba: "constructoras en Antioquia con obras de 3 a 20 unidades". |

### 1.2 Problema claramente expresado — 0 a 3

| Nota | Ancla |
|---:|---|
| 0 | No hay problema. El sitio arranca describiendo la empresa o el producto. |
| 1–2 | El problema se insinúa o aparece enterrado abajo. |
| 3 | El problema del cliente aparece arriba, en su lenguaje, antes de la solución. |

### 1.3 Resultado o transformación — 0 a 4

| Nota | Ancla |
|---:|---|
| 0 | No se promete ningún resultado. |
| 1–2 | Resultado vago: "mejores resultados", "crece tu negocio". |
| 3 | Resultado concreto pero sin magnitud ni plazo. |
| 4 | Resultado concreto con magnitud, plazo o ambos, y respaldado en algún punto del sitio. |

### 1.4 Diferenciador — 0 a 2

| Nota | Ancla |
|---:|---|
| 0 | Nada distingue a este negocio de cualquier competidor. Podrías cambiar el logo y el texto seguiría funcionando. |
| 1 | Hay diferenciador pero es un lugar común: "calidad", "experiencia", "atención personalizada". |
| 2 | Diferenciador específico y defendible, que un competidor no podría copiar en su web mañana. |

### 1.5 Comprensión en 5 segundos — 0 a 2

| Nota | Ancla |
|---:|---|
| 0 | Tras leer solo la parte superior no sabes qué vende el negocio. |
| 1 | Sabes el rubro pero no la oferta ni para quién es. |
| 2 | Qué vende, para quién y qué hacer después quedan claros sin scroll. |

---

## Categoría 2 — Mensaje y contenido persuasivo (15 puntos)

### 2.1 Lenguaje centrado en el cliente — 0 a 4

Usa el conteo de la prueba "nosotros vs. tú".

| Nota | Ancla |
|---:|---|
| 0 | El sitio habla casi exclusivamente de la empresa, su historia y su trayectoria. |
| 1–2 | Predomina la empresa; el cliente aparece de forma incidental. |
| 3 | Equilibrio, con algunas secciones autorreferenciales. |
| 4 | El cliente es el sujeto del texto; la empresa aparece como medio, no como protagonista. |

### 2.2 Beneficios y transformación — 0 a 4

| Nota | Ancla |
|---:|---|
| 0 | Solo características, especificaciones o listados de servicios. |
| 1–2 | Beneficios enunciados pero abstractos. |
| 3 | Beneficios concretos, sin contraste antes/después. |
| 4 | Beneficios concretos con contraste explícito entre la situación actual y la deseada. |

### 2.3 Claridad y ausencia de jerga — 0 a 3

| Nota | Ancla |
|---:|---|
| 0 | Texto denso, corporativo o técnico; un cliente no experto no lo entiende. |
| 1–2 | Legible pero con frases de relleno y tecnicismos innecesarios. |
| 3 | Lenguaje llano, frases cortas, cero relleno. Se entiende de una sola lectura. |

### 2.4 Manejo de objeciones — 0 a 2

| Nota | Ancla |
|---:|---|
| 0 | Ninguna objeción anticipada. Ni FAQ, ni sección de proceso, ni referencia a precio o plazos. |
| 1 | Algunas objeciones atendidas, típicamente en un FAQ genérico. |
| 2 | Las objeciones reales del segmento —precio, tiempo, riesgo, confianza— se abordan donde surgen en el recorrido. |

Cuando el Paso 0 o el subpaso 1k (voz del cliente) aporten objeciones **declaradas u observadas**, evalúa contra ellas — es el caso ideal. Si no existe ninguna, evalúa contra las cuatro clases canónicas de arriba y **marca el análisis como inferido**: no las inventes como si fueran las del negocio.

### 2.5 Consistencia del mensaje y acabado público — 0 a 2

Este subcriterio cubre dos cosas que el visitante experimenta como una sola: que el sitio diga lo mismo en todas partes, y que no deje ver por dónde se construyó.

**Artefactos de construcción visibles.** Cuentan aquí, y hay que buscarlos activamente porque el equipo que hizo el sitio ya no los ve:

- Meta descripciones con notas internas de desarrollo, nombres de máquina de formularios o vistas, o descripciones de contenido que la página no tiene.
- Nombres de producto o de marca equivocados en metadatos o plantillas.
- Nombres de usuario crudos del CMS en lugar del nombre real de la persona.
- Etiquetas de enlace que renderizan la ruta literal en vez de un texto.
- Texto de plantilla sin traducir en versiones de otro idioma.
- Contadores o copy que contradicen lo que hay en pantalla — "llena los 4 datos" sobre un formulario de tres campos.
- Contradicciones internas de contenido: publicar el dato exacto y decir en otro bloque que se entrega después.
- Secciones de plantilla configuradas y nunca pobladas: un encabezado que promete algo —productos relacionados, reseñas, galería— seguido de nada. Frecuente en tiendas y constructores visuales, y peor que no tener la sección, porque el visitante lee la promesa y recibe el vacío.

| Nota | Ancla |
|---:|---|
| 0 | Cada página promete algo distinto, o hay artefactos de construcción visibles en la mayoría de las páginas auditadas. |
| 1 | Promesa consistente en general, con desviaciones de tono o con artefactos de construcción en algunas páginas. |
| 2 | Una sola promesa sostenida en todo el sitio, sin artefactos visibles ni contradicciones internas. |

Estos hallazgos valen poco en puntos y mucho en el informe: son evidencia citable, se arreglan en minutos y le demuestran al cliente que la auditoría miró de verdad. Repórtalos siempre, aunque muevan poco el score — y con más razón cuando el sitio vende rigor, precisión o transparencia, porque ahí contradicen el argumento de venta.

---

## Categoría 3 — Estructura y navegación (12 puntos)

### 3.1 Menú simple — 0 a 3

| Nota | Ancla |
|---:|---|
| 0 | Más de 8 elementos, o menús desplegables anidados que compiten entre sí. |
| 1–2 | 6 a 8 elementos, o etiquetas ambiguas ("Soluciones", "Recursos"). |
| 3 | 5 o menos, etiquetas literales, y el CTA visible en el encabezado. |

### 3.2 Flujo lógico — 0 a 4

Contra el recorrido de referencia: problema → solución → beneficios → prueba → oferta → acción.

| Nota | Ancla |
|---:|---|
| 0 | Secciones sin orden aparente; la home es un collage. |
| 1–2 | Hay orden pero faltan dos o más etapas del recorrido. |
| 3 | Recorrido completo con una etapa débil o fuera de lugar. |
| 4 | Recorrido completo y en orden; cada sección hace avanzar al visitante. |

### 3.3 Jerarquía de páginas — 0 a 3

| Nota | Ancla |
|---:|---|
| 0 | Páginas huérfanas, duplicadas o inalcanzables desde la navegación. |
| 1–2 | Jerarquía funcional pero con solapamientos o profundidad excesiva. |
| 3 | Cada página tiene un lugar claro y la conversión está a un clic desde cualquier punto. |

### 3.4 Ausencia de fricción y callejones sin salida — 0 a 2

| Nota | Ancla |
|---:|---|
| 0 | Páginas que terminan sin siguiente paso; enlaces rotos; formularios que no confirman nada. |
| 1 | Algunas páginas sin salida clara. |
| 2 | Ninguna página termina sin ofrecer el siguiente movimiento. |

---

## Categoría 4 — Credibilidad y confianza (12 puntos)

### 4.1 Testimonios o casos de éxito — 0 a 4

| Nota | Ancla |
|---:|---|
| 0 | Ninguno, o solo logos sin contexto. |
| 1–2 | Testimonios anónimos o genéricos: "Excelente servicio, muy recomendados." |
| 3 | Testimonios con nombre, cargo y empresa, pero sin resultado. |
| 4 | Testimonios o casos atribuidos con problema, acción y resultado verificable. |

### 4.2 Resultados específicos — 0 a 3

| Nota | Ancla |
|---:|---|
| 0 | Cero cifras en todo el sitio. |
| 1–2 | Cifras de vanidad: años de experiencia, número de clientes, "+500 proyectos". |
| 3 | Cifras del resultado del cliente: cuánto mejoró, en cuánto tiempo, en qué. |

### 4.3 Señales de autoridad — 0 a 2

| Nota | Ancla |
|---:|---|
| 0 | Ninguna. Ni certificaciones, ni medios, ni alianzas, ni equipo visible. |
| 1 | Presentes pero irrelevantes para la decisión de compra. |
| 2 | Señales que el segmento reconoce y que reducen riesgo percibido. |

### 4.4 Transparencia y reducción de riesgo — 0 a 3

| Nota | Ancla |
|---:|---|
| 0 | Sin garantía, sin política, sin proceso explicado, sin dirección física ni datos verificables. |
| 1–2 | Información legal presente pero sin garantía ni explicación del proceso. |
| 3 | Proceso explicado paso a paso, garantía o condiciones claras, y datos de la empresa verificables. |

---

## Categoría 5 — CTA y capacidad de conversión (15 puntos)

### 5.1 CTA principal claro — 0 a 4

| Nota | Ancla |
|---:|---|
| 0 | No hay CTA, o hay tantos que ninguno domina. |
| 1–2 | Existe pero compite con otros de peso visual similar. |
| 3 | Hay una acción dominante identificable. |
| 4 | Una sola acción dominante, visualmente inequívoca y repetida coherentemente. |

### 5.2 CTA visible y repetido — 0 a 3

| Nota | Ancla |
|---:|---|
| 0 | Solo aparece en el pie de página o dentro del menú. |
| 1–2 | Visible arriba pero no reaparece durante el scroll. |
| 3 | Visible sin scroll y repetido en los puntos naturales de decisión. |

### 5.3 Lenguaje específico — 0 a 3

| Nota | Ancla |
|---:|---|
| 0 | "Enviar", "Saber más", "Contáctanos", "Ver más". |
| 1–2 | Algo más concreto pero sin nombrar el valor o el esfuerzo: "Contactar ahora". |
| 3 | Nombra la acción y lo que recibe: "Solicita tu cotización en 2 minutos". |

### 5.4 Explicación del siguiente paso — 0 a 2

| Nota | Ancla |
|---:|---|
| 0 | Nada indica qué pasa tras el clic. |
| 1 | Se insinúa. |
| 2 | Se declara: qué recibe, en cuánto tiempo, quién lo contacta y si hay costo. |

### 5.5 Formulario o proceso sin fricción — 0 a 3

Usa el conteo real de campos del Paso 1b.

| Nota | Ancla |
|---:|---|
| 0 | Más de 8 campos, o pide datos sensibles antes de dar valor, o el checkout obliga a crear cuenta. |
| 1–2 | 5 a 8 campos, o pasos innecesarios. |
| 3 | 3 o menos campos obligatorios, o checkout como invitado disponible. |

**Tope del ajuste por canal alterno.** Un canal de baja fricción bien construido —WhatsApp con mensaje precargado y contextual, chat atendido, teléfono visible— mejora la nota, pero **no puede llevarla más allá de 2 si el formulario sigue siendo largo**. La razón: el canal alterno rescata al visitante que ya decidió escribir; no arregla la fricción para quien prefiere no hablar con nadie todavía, que suele ser el prospecto de ciclo largo y ticket alto. Para llegar a 3 tiene que ser corta *también* la ruta del formulario.


---

## Categoría 6 — Embudo de ventas (15 puntos)

Cada etapa se puntúa de 0 a 3 con el mismo criterio:

| Nota | Ancla |
|---:|---|
| 0 | La etapa no existe en el sitio. |
| 1 | Existe algo pero es incidental y sin intención comercial. |
| 2 | Existe y funciona, con vacíos evidentes. |
| 3 | Existe, es deliberada y conecta con la etapa siguiente. |

### 6.1 Atracción — 0 a 3
Contenido, blog activo, landings de campaña, motivo para que alguien llegue sin conocer la marca.

### 6.2 Captura de interés — 0 a 3
Oferta intermedia para quien no está listo hoy: guía, checklist, diagnóstico, lista de precios, consulta de disponibilidad, newsletter con propósito. **Esta es la etapa que más frecuentemente vale 0.**

### 6.3 Generación de deseo — 0 a 3
Casos, demostraciones, explicación del proceso, comparativas, manejo de objeciones.

### 6.4 Conversión — 0 a 3
Que la acción se pueda completar sin fricción y por el canal que el segmento prefiere.

### 6.5 Seguimiento y fidelización — 0 a 3
Página de confirmación con siguiente paso, email automático, onboarding, recompra, referidos.

---

## Categoría 7 — Experiencia móvil y usabilidad (8 puntos)

Evaluable con capturas del usuario o con navegador que permita **emulación móvil** (ver la ruta A del Paso 1b). Sin evidencia visual, marca **7.1–7.3** como NE y normaliza. **7.4 (velocidad) no depende de capturas:** se evalúa únicamente con el dato de PageSpeed, y sin ese dato es NE.

### 7.1 Diseño móvil — 0 a 3

| Nota | Ancla |
|---:|---|
| 0 | Requiere zoom o scroll horizontal; elementos superpuestos o cortados. |
| 1–2 | Adaptado pero con problemas: texto pequeño, botones apretados, menú confuso. |
| 3 | Diseñado para móvil, no solo reducido. |

### 7.2 Legibilidad y jerarquía — 0 a 2

| Nota | Ancla |
|---:|---|
| 0 | Texto ilegible o contraste insuficiente. |
| 1 | Legible con jerarquía plana; todo pesa igual. |
| 2 | Legible con jerarquía que guía la lectura hacia la acción. |

### 7.3 Facilidad de interacción — 0 a 2

| Nota | Ancla |
|---:|---|
| 0 | La acción principal no se puede completar cómodamente con una mano. |
| 1 | Posible pero incómodo. |
| 2 | Botones con área táctil suficiente, formularios con teclado adecuado, sin pop-ups que bloqueen. |

### 7.4 Velocidad — 0 a 1

Solo con dato de PageSpeed Insights. Sin dato, NE.

| Nota | Ancla |
|---:|---|
| 0 | LCP superior a 4 s, INP superior a 500 ms **o** CLS superior a 0,25 (rango "deficiente" de PageSpeed). |
| 1 | LCP ≤ 4 s, INP ≤ 500 ms **y** CLS ≤ 0,25. |

El rango "a mejorar" de PageSpeed (p. ej. LCP entre 2,5 y 4 s) puntúa 1; solo el rango "deficiente" puntúa 0. Usa las tres métricas que el Paso 1f pide (LCP, INP, CLS); si no tienes alguna, evalúa con las que tengas y no penalices la ausente.

---

## Categoría 8 — Automatización y medición (8 puntos)

Basado en la evidencia del Paso 1b. Distingue instalado de bien configurado, y evidencia **observada** (código o navegador — rutas A y B) de evidencia **solo declarada por el cliente**. Lo solo declarado puntúa con **tope 1** en cada subcriterio y se etiqueta "declarado por el cliente" en la columna de evidencia; la nota 2 exige evidencia observada, porque el cliente puede creer que tiene eventos de conversión configurados y tener solo la etiqueta base. Sin código, sin navegador y sin declaración, el subcriterio va a **NE**.

### 8.1 Captura y seguimiento — 0 a 2

| Nota | Ancla |
|---:|---|
| 0 | Formulario que envía a un correo genérico, o solo un `mailto:`. |
| 1 | Formulario conectado a algún destino, sin evidencia de seguimiento estructurado. |
| 2 | Integración visible con CRM o plataforma de gestión de leads. |

### 8.2 Emails o automatización — 0 a 2

| Nota | Ancla |
|---:|---|
| 0 | Sin plataforma de email ni confirmación automática detectable. |
| 1 | Plataforma presente pero sin evidencia de secuencia. |
| 2 | Evidencia de automatización real: confirmación, secuencia, agendamiento automático. |

### 8.3 Analítica y eventos — 0 a 2

| Nota | Ancla |
|---:|---|
| 0 | Sin analítica instalada. **Este cero es el hallazgo número uno del informe.** |
| 1 | Analítica instalada sin evidencia de eventos de conversión. |
| 2 | Analítica más píxeles publicitarios, con eventos de conversión aparentes. |

**Antes de asignar 0**, contrasta con lo que el usuario declaró en el Paso 0 y con las señales de plataforma del 1b (`google-site-verification`, `facebook-domain-verification`, CMP presente). Si hay señales de conexión sin script visible, o sospecha de medición server-side (un cargador `gtag(` sirviéndose desde subdominio propio en vez de `googletagmanager.com`, o ningún script pero verificaciones activas), trátalo como duda y **pregunta al usuario en lugar de asignar 0**. Recuerda que la lista de analítica del 1b incluye Matomo, Plausible, Fathom, Umami y PostHog: no verlas por buscar solo GA no es ausencia.

### 8.4 Optimización, pruebas o recuperación — 0 a 2

| Nota | Ancla |
|---:|---|
| 0 | Nada. |
| 1 | Un elemento: mapas de calor, o recuperación de carrito, o herramienta de pruebas. |
| 2 | Varios, con evidencia de uso deliberado. |

---

## Interpretación del score

| Score | Estado | Lectura para el cliente |
|---:|---|---|
| 90–100 | Excelente | Comunica, genera confianza y conduce a la conversión con muy poca fricción. El trabajo pendiente es de optimización fina. |
| 75–89 | Bueno | Base sólida con oportunidades claras de aumentar contactos o ventas sin tocar el tráfico. |
| 60–74 | Regular | Puede verse bien, pero tiene fugas de conversión importantes. Cada peso invertido en tráfico rinde por debajo de su potencial. |
| 40–59 | Débil | El mensaje, la estructura o el CTA le dificultan al visitante tomar acción. Invertir en publicidad antes de corregir esto es quemar presupuesto. |
| 0–39 | Crítico | El sitio no opera como sistema comercial. Requiere reestructuración antes que optimización. |

Acompaña siempre el score con la cobertura de auditoría. Sin cobertura, el número no es interpretable.
