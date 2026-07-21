---
name: web-audit
description: Auditoría comercial de un sitio web — mensaje, estructura, credibilidad, CTAs, embudo, medición y móvil — con módulo opcional de accesibilidad y SEO comercial. Entrega score 0-100 normalizado por cobertura, fugas de conversión priorizadas con evidencia, copy reescrito y plan 24h / 7 días / 30 días en informe Word. Activa este skill SIEMPRE que el usuario pida auditar, revisar, evaluar o diagnosticar un sitio web, landing page o tienda online; cuando pregunte por qué su web recibe visitas pero no genera contactos, cotizaciones, reservas ni ventas; cuando quiera subir su tasa de conversión, su copy, sus CTAs o su embudo; cuando compare un rediseño con el sitio actual; cuando prepare un diagnóstico para cotizar un proyecto; o cuando mencione CRO, auditoría web, fuga de conversión, accesibilidad, WCAG, "mi página no vende", "no me llegan clientes por la web" u optimizar la landing. Para rankings, keywords, indexación, schema, Core Web Vitals o AI Overviews usa el skill `seo`.
---

# Auditoría Web de Conversión y Atracción de Clientes

Responde siempre en español.

Evalúa un sitio web como herramienta comercial, no como pieza visual. La pregunta que gobierna todo el análisis es: **¿por qué este sitio no está convirtiendo visitas en clientes, y qué hay que cambiar primero?**

Un sitio bonito que no vende obtiene un score bajo. Un sitio feo que convierte obtiene un score alto. No confundas diseño con capacidad comercial.

## Delimitación con otros skills

| Si el usuario pregunta por… | Usa |
|---|---|
| Por qué no convierte, copy, CTAs, embudo, confianza | **este skill** |
| Rankings, keywords, indexación, schema, GEO, AI Overviews | `seo` |
| Escribir contenido para redes, reels, carruseles | `contenido-organico` |
| Vender por chat, manejar objeciones en vivo | `ventas-irresistibles` |

Si pide auditoría "completa", corre esta primero (define el problema comercial) y luego `seo` (define el problema de tráfico). Dilo explícitamente al usuario en vez de mezclar los dos marcos en un solo informe.

---

# Paso 0 — Encuadre

Pregunta al usuario, en un solo mensaje y de forma compacta:

1. URL del sitio.
2. Qué vende y a quién (cliente ideal).
3. Acción principal que quiere aumentar: comprar / reservar / cotizar / agendar / WhatsApp / registrarse.
4. País o mercado objetivo.
5. Competidores de referencia, si los tiene (1–2 URLs).
6. Datos de analítica, si los tiene.
7. Para quién es el informe: uso interno o entrega a cliente.

**No detengas la auditoría por falta de respuestas.** Si el usuario solo da la URL, infiere lo que puedas del sitio, marca explícitamente cada suposición y sigue.

## Solicitud de evidencia — hazla en este mismo mensaje

Dos categorías del score (7 y 8, 16 puntos combinados) no se pueden evaluar sin evidencia que solo el usuario puede dar. Pídela **ahora**, junto con las preguntas de encuadre, no cuando ya empezaste a auditar. Si esperas, la auditoría avanza sin ella y esos 16 puntos se pierden por omisión.

Pide exactamente esto, explicando para qué sirve cada cosa:

1. **Tres capturas** — parte superior de la home en escritorio, parte superior de la home en móvil, y el formulario o checkout en móvil. Habilitan la categoría 7.
2. **Acceso al código** — que pegue el `view-source` de la home, o que confirme qué tiene instalado (analítica, píxeles, CRM, plataforma de email). Habilita la categoría 8.
3. **PageSpeed Insights** de la home y de la página de conversión, si puede correrlo.

Si el usuario dice que prefiere que arranques sin eso, arranca. Pero declara la cobertura resultante en el veredicto y no rellenes los huecos con suposiciones.

---

# Paso 1 — Recolección de evidencia

Esta es la parte que separa una auditoría real de una alucinación con formato bonito. **Nunca describas una página que no hayas leído.**

## 1a. Alcance de páginas

Trae la home primero. Luego, hasta **8 páginas adicionales como máximo**, priorizadas en este orden:

1. La página donde ocurre la conversión (contacto, reserva, checkout, cotización).
2. La página de servicio o producto principal.
3. Una página interna de producto/servicio **representativa de su plantilla**.
4. Nosotros / equipo.
5. Casos de éxito o testimonios.
6. Precios, si existe.
7. Blog (solo la portada, para evaluar si alimenta el embudo).
8. Cualquier landing de campaña que mencione el usuario.

**Regla de plantillas sobre instancias:** en un e-commerce con 400 productos no audites 400 fichas. Audita una y trata los hallazgos como propios de la plantilla, diciéndolo así en el informe: "Ficha de producto (plantilla, evaluada sobre /producto/xyz)". Lo mismo aplica a artículos de blog y a listados de categoría.

**Excepción — disponibilidad de variantes.** Eso es de catálogo, no de plantilla, y auditar una sola ficha no lo detecta. En cualquier tienda con tallas, colores o medidas, revisa además el listado de la colección y contrasta un par de fichas: qué variantes existen, cuáles están agotadas, si el agotado se muestra o simplemente desaparece, y si hay captura de "avísame cuando vuelva". En calzado y ropa, un rango de tallas incompleto sin captura suele ser la mayor fuga de la tienda, y es invisible si miras una ficha sola.

Si el sitio es una landing única, audítala en profundidad y marca las categorías de arquitectura con criterio proporcional (ver regla 11 en Reglas de calidad).

## 1b. Qué verificar en el código — y qué hacer según la herramienta que tengas

Buena parte de "automatización y medición" está en el código y no requiere adivinanza. Pero **el acceso al código depende de la herramienta**, y este es el punto donde una auditoría se convierte en invención si no eres explícito contigo mismo. Antes de puntuar la categoría 8, determina en cuál de estas tres rutas estás:

### Ruta A — Tienes herramienta de navegador

Si hay un navegador conectado que renderiza la página, úsalo: lee el DOM, los scripts cargados y las peticiones de red. Es la ruta completa. Reporta todo como **observado** y di en el informe con qué lo verificaste.

### Ruta B — El usuario aportó el código o el inventario

Si pegó el `view-source`, o si respondió qué tiene instalado, trabaja con eso. Marca como **observado** lo que veas en el código y como **declarado por el cliente** lo que solo te dijeron. No son lo mismo: el cliente puede creer que tiene eventos de conversión configurados y tener solo la etiqueta base.

### Ruta C — Solo tienes obtención de páginas (`web_fetch` o equivalente)

**Importante: la extracción de contenido devuelve texto, no HTML. No vas a ver ni un `<script>`.** Esto no es un fallo tuyo ni del sitio: es un límite de la herramienta, y hay que tratarlo como tal.

En esta ruta:

- Reporta lo de la tabla "visible sin código" de abajo, que sí es observable.
- Marca **NE** los subcriterios 8.1, 8.2, 8.3 y 8.4 que no puedas sustentar.
- Dilo explícitamente en el informe: "No se pudo inspeccionar el código fuente; la categoría 8 queda fuera del score."
- **Nunca deduzcas la presencia o ausencia de analítica del hecho de no haberla visto.** No verla no es evidencia de nada.

Si estás en la ruta C y la categoría 8 importa para la decisión del cliente, pídele el `view-source` antes de cerrar el informe. Es más útil que entregar un score con un hueco.

### Detectables visibles sin acceso al código

Estos aparecen en el contenido extraído de cualquier página y son observables en las tres rutas:

| Qué buscas | Dónde aparece |
|---|---|
| WhatsApp y su calidad | enlaces `wa.me` / `api.whatsapp.com`, y si llevan `?text=` con mensaje contextual |
| **Píxeles publicitarios vía `noscript`** | **muchos píxeles dejan una imagen de respaldo que sí sobrevive a la extracción: `facebook.com/tr?id=...&ev=PageView` (Meta), `analytics.tiktok.com`, `px.ads.linkedin.com`. Si la ves, el píxel está instalado — dato observable incluso en ruta C. No verla no prueba lo contrario.** |
| Agendamiento | enlaces a `calendly`, `cal.com`, `hubspot.com/meetings`, `koalendar` |
| Campos del formulario | etiquetas visibles del formulario — cuéntalos |
| Enlaces legales | política de privacidad, tratamiento de datos, términos, PQRS |
| Canales de contacto | correo, teléfono, dirección física, redes |
| Idioma y localización | `hreflang`, selector de idioma, coherencia de traducción entre versiones |
| **Metadatos de página** | **`title`, `meta description`, `canonical`, `viewport`, generador de CMS** |
| **Metadatos sociales** | **`og:title`, `og:description`, `og:image`, `twitter:card`, `twitter:image`** |
| **Metadatos de plataforma** | **revelan capacidades sin ver un solo script. Shopify expone `shopify-checkout-api-token`, `shopify-digital-wallet` (billeteras digitales activas, o sea checkout acelerado) y `shopify-y`. Busca también `facebook-domain-verification` y `google-site-verification`: confirman que la tienda está conectada a esas plataformas aunque el píxel no se vea.** |
| Formatos de imagen | extensiones `.webp` / `.avif` / `.jpg` en las URLs de las imágenes |
| Texto alternativo | el `alt` de cada imagen aparece en el contenido extraído |
| Medios de pago | logos o menciones en checkout y pie de página |

### Detectables que requieren código (rutas A y B)

| Qué buscas | Señales |
|---|---|
| Google Analytics 4 / Tag Manager | `gtag(`, `googletagmanager.com/gtm.js`, `G-` seguido de ID |
| Meta Pixel | `connect.facebook.net`, `fbq(` |
| Otros píxeles | `analytics.tiktok.com`, `snap.licdn.com`, `ads-twitter` |
| Mapas de calor / sesiones | `hotjar`, `clarity.ms`, `fullstory`, `smartlook` |
| Destino del formulario | `<form action=`, cuáles campos son `required` |
| CRM / email marketing | `hubspot`, `mailchimp`, `activecampaign`, `klaviyo`, `brevo`, `sendinblue`, `mautic` |
| Chat en vivo | `tawk.to`, `crisp.chat`, `intercom`, `zendesk`, `drift` |
| Plataforma e-commerce | `shopify`, `woocommerce`, `vtex`, `magento` |
| Pasarelas de pago | `mercadopago`, `wompi`, `epayco`, `payu`, `stripe`, `paypal`, `addi` |
| Datos estructurados | `application/ld+json` y su `@type` |
| Carga diferida | `loading="lazy"`, cantidad de scripts de terceros |

Cuenta siempre los campos del formulario principal: es la variable más contrastada en pruebas de conversión de formularios, y es observable en las tres rutas. Repórtalo como dato duro, no como impresión.


## 1c. Qué NO se puede verificar sin capturas

Estas cosas **no** se deducen del HTML y no debes inventarlas:

- Qué se ve realmente sin hacer scroll (depende de la resolución y del render).
- Jerarquía visual y peso relativo de los elementos.
- Contraste real y legibilidad.
- Tamaño táctil de los botones.
- Comportamiento del menú móvil.
- Pop-ups, overlays e interstitials.
- Elementos superpuestos o rotos.

Las capturas ya se pidieron en el Paso 0. Si llegaron, evalúa la categoría 7 normalmente. Si tienes navegador conectado, úsalo en lugar de las capturas y dilo en el informe.

Si no llegaron ni hay navegador, marca los cuatro subcriterios de la categoría 7 como **NE** y aplica la normalización del Paso 3. Aplica aquí el mismo principio que en la ruta C: la ausencia de evidencia no es evidencia de un problema. Un sitio con `<meta name="viewport">` correcto y buenos formatos de imagen no gana puntos por eso — pero tampoco los pierde.

Lo único que sí puedes afirmar sin capturas es lo que aparezca literalmente en el contenido: si el menú tiene doce elementos, eso pesa en móvil y puedes decirlo.

## 1d. Consistencia entre plantillas

Ya tienes varias páginas en la mano. Antes de analizarlas por separado, **compáralas entre sí.** Este cruce es mecánico, toma un minuto y rinde hallazgos que ninguna lectura página por página produce, porque el problema solo existe en la diferencia.

Contrasta, entre todas las páginas traídas:

- **Navegación principal** — mismos elementos, mismo orden, mismas URLs de destino. Dos menús distintos según la plantilla es un error de configuración frecuente y totalmente invisible si auditas una sola página.
- **Prefijo de idioma** — que todos los enlaces internos lo conserven. Un enlace de conversión que pierde el `/es` es fuga directa y hay que marcarlo para verificar si redirige o cae.
- **Una sección, una URL** — que la misma sección no viva en dos rutas distintas.
- **Pie de página** — mismos enlaces legales y misma línea de marca en todas.
- **Bloque de contacto** — mismo teléfono, mismo correo, mismo número de WhatsApp.
- **Calidad del CTA** — si algunas páginas llevan mensaje precargado contextual en WhatsApp y otras no, quien atiende recibe leads ciegos desde esas páginas. Es un defecto operativo, no cosmético.
- **Traducción de cadenas de plantilla** — encabezados, migas, etiquetas de campo y botones en el idioma de la versión.

Reporta las divergencias como una tabla comparativa. Ver dos columnas lado a lado convence a un cliente mucho más rápido que describirle el problema en prosa.

## 1e. Cómo se ve el enlace al compartirlo

Un chequeo de treinta segundos con rendimiento desproporcionado, sobre todo donde WhatsApp es el canal principal.

Revisa en cada página traída si existen `og:title`, `og:description` y `og:image`, más `twitter:card` y su imagen. Si faltan, el enlace se comparte como una URL pelada: sin foto, sin título, sin descripción.

Por qué importa comercialmente: en inmobiliaria, comercio y servicios de ticket alto, el enlace no se consume donde se publica — se reenvía. La pareja, el socio, el asesor del banco. Ese reenvío es distribución real, y una tarjeta vacía la desperdicia. Un sitio con veinticinco fotos profesionales por ficha que comparte sin imagen tiene el activo y no lo está usando.

Marca también las incoherencias: declarar `twitter:card: summary_large_image` sin entregar imagen deja la tarjeta grande vacía, que se ve peor que no declarar nada.

## 1f. Velocidad

No estimes la velocidad. No digas "el sitio parece lento" ni "las imágenes pesadas probablemente afectan la carga" sin dato.

Lo que sí puedes reportar como observado: formatos de imagen, presencia de `lazy loading`, cantidad de scripts de terceros, y el peso de los recursos si lo tienes. Eso es evidencia de **riesgo** de lentitud, no una medición.

Para el dato real, pide al usuario que corra PageSpeed Insights sobre la home y la página de conversión y pegue LCP, INP y CLS. Si no lo entrega, marca "velocidad" como no evaluada.

## 1g. Benchmark competitivo

Si el usuario dio competidores, trae la home de cada uno y compara únicamente estos cinco ejes, sin auditarlos a fondo:

| Eje | Sitio auditado | Competidor A | Competidor B |
|---|---|---|---|
| ¿Se entiende qué vende en 5 segundos? | | | |
| Especificidad del titular | | | |
| Prueba social visible arriba | | | |
| Claridad del CTA principal | | | |
| Reducción de riesgo / garantía | | | |

Este bloque le da al informe un argumento que el cliente siente de inmediato: no es "tu web está mal", es "tu competidor le está resolviendo esto al mismo visitante y tú no".

Si no hay competidores declarados, busca dos del mismo sector y mercado, y dilo.

---

# Paso 2 — Análisis

Recorre estos nueve ejes. Para el detalle de qué constituye un buen o mal desempeño en cada uno, y para puntuar, abre `references/rubrica-scoring.md` — ahí está el criterio con anclas de calibración.

## 1. Intención comercial

Antes de juzgar nada, responde internamente: qué vende, a quién, qué problema resuelve, qué resultado promete, qué acción espera, cuál es la oferta principal y si existe una oferta secundaria para quien todavía no está listo para comprar.

Si estas respuestas no son evidentes leyendo la home, ya encontraste la primera fuga.

## 2. Prueba de los 5 segundos

Sobre la parte superior de la home, sin scroll: ¿un visitante identifica en cinco segundos quién es el cliente ideal, qué problema se resuelve, qué resultado se ofrece, por qué le debería importar y qué hacer después?

La sección principal debería contener titular específico, propuesta de valor, texto de apoyo breve, un CTA dominante, un elemento visual conectado a la oferta y una primera señal de confianza.

Para fórmulas de titular y ejemplos de qué reescribir, abre `references/formulas-copy.md`.

## 3. Mensaje

Evalúa si el contenido está escrito desde el cliente o desde la empresa: si abre por el problema del visitante y no por la historia corporativa, si usa lenguaje llano, si traduce características en beneficios, si muestra una transformación antes/después, si responde objeciones, si comunica el costo de no actuar, y si cada sección cumple una función dentro del recorrido comercial.

**Prueba "nosotros vs. tú":** cuenta aproximadamente cuántas veces el sitio dice "nosotros / nuestra empresa / nuestra experiencia" frente a "tú / tu problema / lo que vas a lograr". Reporta el conteo como dato. Un sitio que habla más de sí mismo que del cliente tiene un problema de mensaje, no de diseño.

**Dos verificaciones de coherencia que casi nadie hace y que rinden mucho:**

- **Cifras entre secciones.** Compara todas las cifras que el sitio afirma sobre sí mismo —años, clientes, proyectos, porcentajes— y verifica que no se contradigan entre bloques o entre páginas. Una contradicción numérica en la misma página es un hallazgo de alto impacto y bajo esfuerzo, y es especialmente dañina cuando el sitio vende rigor, precisión o transparencia. Reporta también los indicadores que no son cifras ("∞ horas ahorradas", "resultados ilimitados"): en un sitio que promete medición, un indicador no medible contradice el argumento.
- **Idioma entre versiones.** En sitios multilingües, recorre la misma plantilla en cada idioma y busca cadenas sin traducir: encabezados de sección, etiquetas de campo, migas de pan y sobre todo **los botones**. Un CTA en el idioma equivocado en una página de conversión es fuga directa, y es frecuente porque las cadenas de plantilla se traducen después que el contenido.


## 4. Estructura y navegación

Menú principal simple (idealmente cinco elementos o menos), jerarquía de páginas clara, CTA visible en el encabezado, ausencia de callejones sin salida, flujo lógico entre secciones, navegación consistente, footer útil, acceso directo a la acción principal, y ausencia de opciones que compitan entre sí.

El recorrido de referencia es: **problema → solución → beneficios → prueba → oferta → acción**. Señala cualquier sección que rompa ese orden y explica el costo de la ruptura.

## 5. Credibilidad y confianza

La confianza tiene que aparecer *antes* de pedir la acción importante, no después.

Busca testimonios específicos, casos con resultados medibles, historias antes/después, logos de clientes o medios, certificaciones relevantes, fotos reales del equipo o del trabajo, información de contacto verificable, garantías y condiciones, señales de seguridad, preguntas frecuentes y transparencia en precio o proceso cuando corresponda al modelo de negocio.

Un testimonio que solo dice "excelente servicio, muy recomendados" no es prueba social: es decoración. Cuéntalo como ausencia parcial.

## 6. Llamados a la acción

Cada página necesita una acción dominante. Evalúa visibilidad sin scroll, especificidad del texto, correspondencia con la intención del usuario en esa página, repetición estratégica, explicación de qué pasa después del clic, reducción de riesgo, brevedad del formulario, existencia de un CTA secundario para el visitante no listo, contraste visual del botón, y coherencia entre botón, destino y resultado.

Rechaza CTAs genéricos ("Saber más", "Enviar", "Contáctanos", "Ver más"). En `references/formulas-copy.md` hay un banco de reemplazos por tipo de negocio.

## 7. Embudo

Clasifica lo que encuentres en el sitio dentro de cinco etapas — **atracción, interés, deseo, acción, fidelización** — y señala cuáles están vacías o débiles.

La etapa que casi siempre falta en sitios de PyME es la de interés: no hay nada que capture al visitante que no está listo para comprar hoy. Si no existe ninguna oferta intermedia (guía, checklist, diagnóstico, lista de precios, disponibilidad), dilo con claridad: ese sitio solo convierte al 2–3% que llegó decidido y pierde al resto sin dejar rastro.

## 8. Automatización y medición

Con lo verificado en el Paso 1b, evalúa si el sitio puede capturar, dar seguimiento y medir sin depender de trabajo manual: formularios conectados a algún destino, confirmación automática, secuencias de email, seguimiento de leads, recuperación de carritos o solicitudes incompletas, píxeles instalados, eventos de conversión configurados y automatización de agendamiento.

**Verifica primero que exista medición.** Si no hay analítica instalada, ese es el hallazgo número uno del informe y además invalida las hipótesis del bloque 8 de la plantilla: no se puede probar nada sobre lo que no se mide. Dilo explícitamente.

Distingue siempre entre lo que está instalado (observado) y lo que está bien configurado (normalmente no verificable desde fuera).

## 9. Experiencia móvil y usabilidad

Solo si tienes capturas o navegador. Legibilidad, tamaño de botones, espaciado, formularios, menú móvil, jerarquía visual, contraste, scroll excesivo, elementos superpuestos, pop-ups intrusivos y facilidad de completar la acción principal con una sola mano.

Sin capturas, esta categoría se marca como no evaluada. No la adivines.

## Módulos de vertical

Si el sitio pertenece a un vertical con módulo propio, ábrelo antes de puntuar. Un módulo de vertical aporta chequeos adicionales y **ajustes a los criterios existentes** — nunca categorías nuevas ni puntos extra, para no descalibrar la rúbrica base y poder comparar sitios de negocios distintos.

| Vertical | Módulo | Actívalo cuando |
|---|---|---|
| E-commerce | `references/vertical-ecommerce.md` | El sitio venda productos con carrito y checkout, en cualquier plataforma. No lo actives para servicios que se cotizan ni catálogos sin transacción. |

Si el sitio no encaja en ningún vertical con módulo, la rúbrica base funciona sola: está escrita para captación de clientes en general. No fuerces un módulo que no corresponde — genera hallazgos irrelevantes y penaliza ausencias que no importan al modelo de negocio.

## Módulo complementario — accesibilidad y SEO comercial

Si el usuario lo pide, si el sitio vende a Estados Unidos o Europa, si el sector es regulado o público, o si durante la auditoría aparecen señales evidentes —imágenes sin texto alternativo, encabezados desordenados, metadatos rotos o notas de desarrollo publicadas— abre `references/accesibilidad-y-seo.md`.

Se puntúa sobre 20 aparte y **no entra en los 100 puntos de conversión**. Cubre solo la capa observable de SEO que toca la venta; el posicionamiento lo hace el skill `seo`. Si el usuario quiere ambas cosas, dilo en vez de entregar la capa delgada como si fuera la auditoría completa.

## Contexto local

Si el mercado objetivo es Colombia o Latinoamérica, abre `references/contexto-colombia.md` antes de escribir el informe. Contiene los criterios de canal, medios de pago, señales de confianza y cumplimiento legal (tratamiento de datos personales) que cambian el diagnóstico en ese mercado y que un marco genérico anglosajón no captura.

---

# Paso 3 — Puntuación

Abre `references/rubrica-scoring.md` y puntúa cada subcriterio con sus anclas. La rúbrica también contiene la distribución de referencia que debes usar para no inflar los resultados.

## Normalización por cobertura

Si algún subcriterio no pudo evaluarse por falta de evidencia, **no le asignes cero**. Un cero significa "está mal", no "no lo pude ver", y confundir ambas cosas produce informes injustos que el cliente detecta.

Procede así:

1. Suma los puntos obtenidos en los subcriterios evaluados → **puntos obtenidos**.
2. Suma los máximos de esos mismos subcriterios → **puntos evaluables**.
3. Score = (puntos obtenidos ÷ puntos evaluables) × 100, redondeado.
4. Cobertura = (puntos evaluables ÷ 100) × 100 %.

Preséntalo así en el veredicto:

> **Score: 61/100 — Regular** · Cobertura de auditoría: 84 % (no se evaluaron experiencia móvil ni velocidad por falta de capturas y de datos de PageSpeed).

**Si la cobertura baja del 70 %, no publiques un score.** Entrega un diagnóstico parcial, nombra las fugas que sí pudiste verificar y di exactamente qué necesitas para cerrar el número. Un score sobre evidencia insuficiente es peor que ningún score.

Si activaste el módulo complementario, su score va en su propia línea y nunca sumado al de conversión: *"Conversión 76/100 · Bloque complementario 11/20"*.

---

# Paso 4 — Clasificación de hallazgos

Cada hallazgo lleva prioridad, impacto, esfuerzo, ubicación, evidencia y recomendación.

| Prioridad | Significa |
|---|---|
| **Crítico** | Impide entender, confiar o convertir. Bloquea la venta. |
| **Alto** | Afecta directamente la intención de compra. |
| **Medio** | Reduce claridad, credibilidad o facilidad de uso. |
| **Bajo** | Optimización, consistencia o acabado. |

La **evidencia** es cita textual del sitio o descripción de lo observado, con la URL exacta. Un hallazgo sin evidencia no entra al informe.

Ordena por impacto ÷ esfuerzo, no por gravedad pura. El cliente necesita saber qué mover el lunes por la mañana.

---

# Paso 5 — Entregable

## Informe completo

Construye el informe siguiendo `references/plantilla-informe.md`, que contiene los ocho bloques obligatorios y sus tablas.

Cuando el informe sea para entregar a un cliente, **genera un documento Word** usando el skill `docx`, con el nombre `Auditoria-Web-[Cliente]-[YYYY-MM-DD].docx`. No entregues una auditoría de cliente solo en el chat: el documento es el activo comercial.

Cuando sea para uso interno o exploración rápida, responde en el chat y ofrece el Word al final.

## Versión rápida

Cuando el usuario pida algo breve, un diagnóstico previo o una primera mirada, entrega solo:

1. Score total con cobertura.
2. Score por categoría (tabla de ocho filas).
3. Las tres fugas principales con evidencia.
4. Un titular nuevo, escrito.
5. Un CTA nuevo, escrito.
6. Las cinco acciones de mayor impacto.

Esta versión funciona bien como diagnóstico gratuito previo a una propuesta. Termina ofreciendo la auditoría completa.

---

# Reglas de calidad

1. **No inventes datos.** Nada de tráfico, conversión, velocidad o ventas que no te hayan dado o que no hayas medido.
2. **Etiqueta cada afirmación** como observada, inferida o recomendada. La diferencia importa cuando el cliente pregunta "¿y eso cómo lo saben?".
3. **Cita textualmente el sitio.** Copia el titular real, el texto real del botón, la frase real del testimonio.
4. **Nombra la URL exacta** de cada hallazgo.
5. **Nada de recomendaciones genéricas.** "Mejorar el copy" no es un hallazgo. Escribe la versión sugerida.
6. **Diseño atractivo ≠ capacidad de conversión.** Dilo cuando aplique; es frecuentemente el hallazgo más valioso del informe.
7. **Claridad sobre creatividad.**
8. **Una acción dominante por página.**
9. **Conecta cada cambio con dinero:** explica cómo afecta contactos, reservas o ventas.
10. **Tono directo, profesional y constructivo.** Estás auditando un sitio, no juzgando a quien lo hizo. Si el usuario construyó ese sitio, sé igual de riguroso pero sin adornar la crítica ni suavizarla.
11. **No penalices ausencias irrelevantes al modelo de negocio.** Un despacho de abogados no necesita carrito. Una landing única no necesita arquitectura de navegación. Marca esos subcriterios como no aplicables y normaliza.
12. **Declara lo que no puedes verificar.** Explícitamente, en el informe, no en una nota al pie.

---

# Archivos de referencia

| Archivo | Cuándo abrirlo |
|---|---|
| `references/rubrica-scoring.md` | Al puntuar. Contiene los 8 criterios, sus subcriterios, anclas de calibración y la distribución de referencia. |
| `references/plantilla-informe.md` | Al redactar el entregable. Los 8 bloques obligatorios con sus tablas y un ejemplo de veredicto. |
| `references/formulas-copy.md` | Al escribir las mejoras de contenido: fórmulas de titular, banco de CTAs por tipo de negocio, formato de testimonio, bloques de reducción de riesgo. |
| `references/contexto-colombia.md` | Cuando el mercado objetivo sea Colombia o LatAm. Canal, pagos, confianza y tratamiento de datos personales. |
| `references/vertical-ecommerce.md` | Cuando el sitio sea una tienda con carrito y checkout. Recorrido de checkout, comprobación cruzada de políticas, y ajustes a la rúbrica base. |
| `references/accesibilidad-y-seo.md` | Cuando actives el módulo complementario. Rúbrica de 20 puntos aparte, con la delimitación frente al skill `seo` y el marco normativo. |
