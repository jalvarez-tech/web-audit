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
6. Datos de analítica, si los tiene: de los últimos 3 meses, las 10 páginas de aterrizaje con más sesiones, el % móvil vs. escritorio y las conversiones/mes de la acción principal (capturas de GA4 valen); y el ticket promedio o el valor de un cliente/lead (habilitan el bloque 4b, Escenario económico).
7. Para quién es el informe: uso interno o entrega a cliente.
8. ¿De dónde llegan hoy las visitas? (pauta en Meta/Google, Instagram orgánico, buscador, referidos). Si hay pauta activa, pega el texto/creativo del anuncio principal y su URL de destino.

**No detengas la auditoría por falta de respuestas.** Si el usuario solo da la URL, infiere lo que puedas del sitio, marca explícitamente cada suposición y sigue.

## Solicitud de evidencia — hazla en este mismo mensaje

Dos categorías del score (7 y 8, 16 puntos combinados) no se pueden evaluar sin evidencia que solo el usuario puede dar. Pídela **ahora**, junto con las preguntas de encuadre, no cuando ya empezaste a auditar. Si esperas, la auditoría avanza sin ella y esos 16 puntos se pierden por omisión.

Pide exactamente esto, explicando para qué sirve cada cosa:

1. **Tres capturas** — parte superior de la home en escritorio, parte superior de la home en móvil, y el formulario o checkout en móvil. Habilitan la categoría 7.
2. **Acceso al código** — que pegue el `view-source` de la home, o que confirme qué tiene instalado (analítica, píxeles, CRM, plataforma de email). Habilita la categoría 8.
3. **PageSpeed Insights** de la home y de la página de conversión, si puede correrlo.
4. **Objeciones y voz del cliente** (opcional) — las 2–3 objeciones que más le dicen los clientes antes de comprar, y si puede, 3–5 mensajes reales de WhatsApp o chat (sin nombres ni teléfonos). Habilitan la nota alta de 2.4 y el copy con lenguaje real.

Si el usuario dice que prefiere que arranques sin eso, arranca. Pero declara la cobertura resultante en el veredicto y no rellenes los huecos con suposiciones.

## Control de turno

Envía el encuadre y la solicitud de evidencia en un solo mensaje y **termina tu turno ahí**: no inicies el Paso 1 hasta recibir respuesta. Solo salta la espera en dos casos: (a) el mensaje inicial del usuario ya trae las respuestas o la evidencia (capturas, `view-source`), o (b) el usuario pidió expresamente arrancar sin preguntas. "No detengas la auditoría por falta de respuestas" aplica a la respuesta que recibas —si es parcial o dice "arranca así", infiere, marca suposiciones y sigue— **no es licencia para auditar en el mismo turno en que preguntaste.**

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

Si hay un navegador conectado que renderiza la página, úsalo: lee el DOM, los scripts cargados y las peticiones de red. Es la ruta completa. Reporta todo como **observado** y di en el informe con qué lo verificaste. Aprovéchala al máximo — no dejes en NE lo que el navegador sí puede sustentar:

1. Toma tu propia captura de la parte superior de la home en escritorio.
2. Si la herramienta permite redimensionar el viewport, emula móvil (~375 px) y repite la captura de la home y de la página de conversión. Con eso, los subcriterios **7.1–7.3 se evalúan como observados** sin capturas del usuario. Si no permite redimensionar, evalúa solo lo sustentable en escritorio y marca NE lo demás.
3. Durante la navegación, registra pop-ups, overlays e interstitials, y prueba el menú móvil.
4. Para píxeles, prefiere como evidencia el **disparo real** en las peticiones de red (`google-analytics.com/g/collect`, `facebook.com/tr`) sobre la mera presencia del script en el DOM: script presente sin disparo se reporta como "instalado pero sin evento verificado".
5. Obtén LCP/INP/CLS navegando a `pagespeed.web.dev` sobre la home y la página de conversión, y repórtalos como observados con fecha (ver 1f).

### Ruta B — El usuario aportó el código o el inventario

Si pegó el `view-source`, o si respondió qué tiene instalado, trabaja con eso. Marca como **observado** lo que veas en el código y como **declarado por el cliente** lo que solo te dijeron. No son lo mismo: el cliente puede creer que tiene eventos de conversión configurados y tener solo la etiqueta base.

### Ruta C — Solo tienes obtención de páginas (`web_fetch` o equivalente)

**Antes de declarar Ruta C, intenta salir de ella.** Si tienes Bash, `curl -sL <url>` te entrega el código fuente completo — con eso estás en **Ruta B** (código obtenido por ti; repórtalo como observado). La Ruta C aplica solo cuando tu única herramienta devuelve contenido sin markup.

**Importante: si la extracción devuelve texto y no HTML, no vas a ver ni un `<script>`.** Esto no es un fallo tuyo ni del sitio: es un límite de la herramienta, y hay que tratarlo como tal.

**Prueba de alcance del extractor.** Antes de puntuar nada que dependa del `<head>` o del markup, corre dos sondas sobre la home para saber qué te entrega tu herramienta:

- **Sonda de `<head>`** — busca marcadores casi universales: `viewport`, `charset` o cualquier `<meta` literal. No uses `og:title` como sonda: su ausencia es justo lo que vas a evaluar. Si aparecen, estás en **subruta C1** y la tabla de detectables aplica completa. Si no aparecen, los metadatos (`title`, `meta description`, `canonical`, `viewport`, `og:*`, `twitter:*`, tokens de plataforma, verificaciones, `hreflang`, píxel `noscript`) pasan a **NE** con la regla "no verlo no prueba nada" — estás en **subruta C2**.
- **Sonda de imágenes** — si el contenido conserva sintaxis de imagen (`![alt](url)` o equivalente), el `alt` y los formatos de imagen **sí** son evaluables aunque el `<head>` no lo sea, porque los extractores markdown típicos conservan las imágenes y eliminan el `<head>`.

En esta ruta:

- Reporta lo de la tabla "visible sin código" de abajo, respetando qué exige C1 y qué exige la sonda de imágenes.
- Marca **NE** los subcriterios 8.1, 8.2, 8.3 y 8.4 que no puedas sustentar.
- Dilo explícitamente en el informe: "No se pudo inspeccionar el código fuente; la categoría 8 queda fuera del score."
- **Nunca deduzcas la presencia o ausencia de analítica del hecho de no haberla visto.** No verla no es evidencia de nada.

Si estás en la ruta C y la categoría 8 importa para la decisión del cliente, pídele el `view-source` antes de cerrar el informe. Es más útil que entregar un score con un hueco.

### Detectables visibles sin acceso al código

Su observabilidad depende de la ruta. Los de **contenido visible** (WhatsApp, agendamiento, campos del formulario, enlaces legales, canales de contacto, medios de pago) se observan en las tres rutas. Los de **`<head>` o markup** (metadatos de página, sociales y de plataforma, `hreflang`, píxel `noscript`) requieren rutas A, B o **C1**; en **C2** van a NE. El `alt` y los formatos de imagen dependen de la **sonda de imágenes**, no de la del `<head>` (ver la prueba de alcance arriba):

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
| Analítica | GA4 / Tag Manager: `gtag(`, `googletagmanager.com/gtm.js`, `G-` seguido de ID. También `matomo`, `plausible.io`, `usefathom`, `umami`, `posthog` — un sitio con estas **no** está "sin analítica" |
| Meta Pixel | `connect.facebook.net`, `fbq(` |
| Otros píxeles | `analytics.tiktok.com`, `snap.licdn.com`, `ads-twitter`, `AW-` / `googleadservices` (Google Ads), `pintrk` (Pinterest) |
| Gestor de consentimiento (CMP) | `cookiebot`, `onetrust`, `usercentrics`. Con bloqueo previo, los scripts de medición pueden estar presentes pero inertes (`type="text/plain"`, `data-cookieconsent`, `data-usercentrics`) y no disparar red hasta el consentimiento: en ruta A verifica el HTML estático además de la red, reporta el CMP como observado y **nunca concluyas ausencia solo porque el píxel no disparó** |
| Mapas de calor / sesiones | `hotjar`, `clarity.ms`, `fullstory`, `smartlook` |
| Destino del formulario | `<form action=`, cuáles campos son `required` |
| CRM / email marketing | `hubspot`, `mailchimp`, `activecampaign`, `klaviyo`, `brevo`, `sendinblue`, `mautic` |
| Chat en vivo | `tawk.to`, `crisp.chat`, `intercom`, `zendesk`, `drift`, `jivochat`, `cliengo`, `wati`, `callbell` |
| Plataforma e-commerce / CMS | `shopify`, `woocommerce`, `vtex`, `magento`, `tiendanube` / `nuvemshop`, `wix`, `webflow`, `squarespace`, `jumpseller` |
| Pasarelas de pago | `mercadopago`, `wompi`, `epayco`, `payu`, `stripe`, `paypal`, `addi` |
| Datos estructurados | `application/ld+json` y su `@type` |
| Carga diferida | `loading="lazy"`, cantidad de scripts de terceros |

Cuenta siempre los campos del formulario principal: es la variable más contrastada en pruebas de conversión de formularios, y es observable en las tres rutas. Repórtalo como dato duro, no como impresión.

### Qué pasa después de enviar el formulario — protocolo

Tres subcriterios dependen de qué ocurre tras enviar (3.4, 6.5, 8.2), y esa evidencia no se recoge sola. Antes de puntuarlos:

1. **Regla dura** (espejo de la del checkout en `vertical-ecommerce.md`): nunca envíes un formulario real sin permiso explícito del usuario en el chat, y **jamás** en checkouts, pagos o formularios que disparen operaciones (pedidos, reservas con cargo).
2. **Agota los proxies observables sin enviar:** el `action` del formulario o una URL tipo `/gracias` en el sitemap (tráela y evalúa su siguiente paso), mensajes de éxito ya presentes en el DOM, y la plataforma de email/CRM en el código.
3. **Solo con permiso y en ruta A:** llena con datos inequívocamente de prueba (nombre "PRUEBA AUDITORÍA — ignorar", el correo del propio usuario), envía **una sola vez**, y reporta como observado: confirmación inline vs. redirección, contenido del siguiente paso, y pregunta al usuario si llegó correo automático (tú no ves su bandeja). Avísale que el envío generará un registro en el sistema del negocio auditado.
4. **Alternativa preferida** cuando el sitio es de un cliente del usuario: que el usuario haga el envío de prueba y pegue lo que vio — evidencia de ruta B ("declarado por el cliente" si solo lo describe, "observado" si pega captura).
5. **Puntuación:** sin evidencia post-envío, **no** marques 6.5 ni 8.2 completos como NE — puntúalos sobre sus componentes observables (plataforma, agendamiento, recompra/referidos) sin acreditar ni penalizar la confirmación; y nunca apliques el ancla 0 de 3.4 ("formularios que no confirman nada") por inferencia: la ausencia de evidencia no es evidencia de un problema.


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

Si no llegaron ni hay navegador, marca los subcriterios 7.1 a 7.3 como **NE** y aplica la normalización del Paso 3; la velocidad (7.4) se evalúa aparte si el usuario entregó el dato de PageSpeed, aunque no haya capturas. Aplica aquí el mismo principio que en la ruta C: la ausencia de evidencia no es evidencia de un problema. Un sitio con `<meta name="viewport">` correcto y buenos formatos de imagen no gana puntos por eso — pero tampoco los pierde.

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

Para el dato real: **en ruta A, corre PageSpeed tú mismo** navegando a `pagespeed.web.dev` sobre la home y la página de conversión, y reporta LCP, INP y CLS como observados con fecha. Si la navegación falla o estás en rutas B/C, pide al usuario que lo corra y pegue las tres métricas. Sin dato, marca la velocidad (7.4) como NE.

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

## 1h. Seguridad de transporte

La señal de confianza más barata de verificar y observable en las tres rutas. Tres chequeos:

1. **HTTP → HTTPS.** Solicita la home por `http://` y registra qué hace: redirige a `https://` (correcto), falla el certificado, o sirve contenido sin redirigir. En ruta C, si la herramienta sigue redirecciones en silencio, reporta solo la URL final y lo que la herramienta revele, y marca **NE** lo que no muestre — nunca deduzcas.
2. **www vs. no-www.** Solicita la variante contraria y verifica que redirige a una sola canónica. Si ambas sirven contenido duplicado, repórtalo como hallazgo de confianza/consistencia observado y delega la canonicalización e indexación al skill `seo` (o a S4 del módulo complementario si está activo).
3. **Contenido mixto** (solo ruta A): revisa la consola por avisos de recursos cargados por `http` en una página `https`.

`http` sin redirección o certificado inválido/vencido dispara el aviso "No seguro" del navegador: es hallazgo **Crítico** y se refleja en la lectura del subcriterio 4.4 (reducción de riesgo) — sin puntos ni categorías nuevas. Etiqueta la evidencia como observada, con la URL exacta probada y la herramienta usada.

## 1i. Enlaces, redirecciones y página de error

Con tope de esfuerzo y disciplina de rutas:

1. **Enlaces clave.** De las páginas ya traídas, verifica el destino del CTA principal de cada una y de 3–5 enlaces internos de navegación —**máximo 10 URLs**— reportando cada uno como "ok", "redirige a X" o "cae". Todo enlace marcado como sospechoso en 1d (prefijo de idioma perdido) tiene prioridad dentro del cupo.
2. **Ruta declarada.** En ruta A, el estado y la cadena de redirección se leen de las peticiones de red y se reportan como observados. En ruta C, el veredicto se da por el contenido devuelto (¿es la página esperada o una de error?), y la distinción "redirige vs. directo" se marca como no distinguible si la herramienta no la expone — nunca deduzcas que un enlace está roto solo porque la herramienta falló al traerlo.
3. **Página 404.** Solicita una URL deliberadamente inexistente bajo el prefijo de idioma del sitio (p. ej. `/es/auditoria-404-test`) y reporta si la página de error mantiene marca, navegación y un siguiente paso (buscador, enlaces a secciones, CTA), o si es la genérica del servidor o de la plataforma.
4. **Conexión con la rúbrica.** Sin este subpaso ejecutado, la parte de "enlaces rotos" del subcriterio 3.4 no se puntúa por impresión: se sustenta con esta tabla o se trata como no verificada. Un enlace de conversión que cae es hallazgo **Crítico** en el Paso 4.

## 1j. Si el cliente entregó datos de analítica

Con los datos del Paso 0, la auditoría deja de ser a ciegas. Úsalos así:

1. **Prioriza la recolección del 1a por tráfico real:** la página de conversión y la regla de plantillas conservan prioridad; las sesiones reordenan los cupos restantes y pueden incorporar una página de aterrizaje de alto tráfico que la lista fija omitiría.
2. **Cuantifica las fugas:** en el bloque 4, sustenta "Por qué cuesta ventas" con las sesiones que tocan esa página cuando el dato exista ("~N sesiones/mes pasan por aquí").
3. **Llena la línea base:** en las hipótesis del bloque 10, escribe el valor entregado en "Línea base actual" en lugar de "no medido hoy".
4. **Etiqueta el origen:** todo dato del cliente es "declarado por el cliente" (regla de calidad 2), u "observado en captura" si viene en pantallazo.
5. **Dos límites:** los datos declarados priorizan y cuantifican, pero **nunca mueven puntos de la rúbrica** (la calibración no depende de lo que el cliente declare); y las fuentes de tráfico se usan solo como contexto de priorización — el diagnóstico de adquisición pertenece al skill `seo`.

Sin datos, nada cambia: el 1a aplica tal como está.

## 1k. Voz del cliente

Chequeo oportunista, solo sobre fuentes que la herramienta pueda leer de verdad:

- **Reseñas en el propio sitio** (fichas de producto, testimonios) — siempre legibles.
- **Reseñas públicas externas** (Google Business, marketplaces) — solo si hay navegador conectado o el usuario pega el texto. Nunca deduzcas nada de no poder acceder (mismo principio de la Ruta C).
- **Objeciones y mensajes** que el usuario aportó en el Paso 0.

De lo que leas, extrae objeciones y vocabulario textual, citados con su fuente —evidencia observada, o "declarado por el cliente" si el usuario los pegó—. Uso posterior: el subcriterio 2.4 y el bloque de copy (bloque 8) usan estas objeciones y palabras reales cuando existan; si no existe ninguna, 2.4 se evalúa contra las cuatro clases canónicas del ancla (precio, tiempo, riesgo, confianza) marcando el análisis como inferido, y el copy propuesto se marca como "hipótesis a validar con clientes reales".

---

# Paso 2 — Análisis

Recorre estos nueve ejes. Los ejes 1 y 2 alimentan juntos la categoría 1 de la rúbrica; a partir del eje 3 la numeración de ejes **no** coincide con la de categorías — cada encabezado indica su categoría entre paréntesis. Usa siempre el número de categoría de `references/rubrica-scoring.md` al puntuar o marcar NE/NA. Para el detalle de qué constituye un buen o mal desempeño en cada uno, y para puntuar, abre `references/rubrica-scoring.md` — ahí está el criterio con anclas de calibración.

## 1. Intención comercial (→ categoría 1)

Antes de juzgar nada, responde internamente: qué vende, a quién, qué problema resuelve, qué resultado promete, qué acción espera, cuál es la oferta principal y si existe una oferta secundaria para quien todavía no está listo para comprar.

Si estas respuestas no son evidentes leyendo la home, ya encontraste la primera fuga.

## 2. Prueba de los 5 segundos (→ categoría 1)

Sobre la parte superior de la home, sin scroll —sobre el viewport móvil cuando haya evidencia móvil (regla de viewport de la rúbrica)—: ¿un visitante identifica en cinco segundos quién es el cliente ideal, qué problema se resuelve, qué resultado se ofrece, por qué le debería importar y qué hacer después?

La sección principal debería contener titular específico, propuesta de valor, texto de apoyo breve, un CTA dominante, un elemento visual conectado a la oferta y una primera señal de confianza.

**Coherencia anuncio→destino (si hay pauta activa).** Si el usuario declaró pauta y aportó el anuncio, contrasta su promesa, oferta y lenguaje contra el bloque superior de la página de destino, citando ambos lados. Cada divergencia se reporta como fuga en el Paso 4 (anuncio = "declarado por el cliente"; página = "observado"). Si el canal dominante es Instagram orgánico, aplica el mismo contraste entre la bio/publicaciones y la landing. Esto alimenta la evidencia de 1.5 y 5.1; si no hay pauta, se omite sin marcar NE ni penalizar.

Para fórmulas de titular y ejemplos de qué reescribir, abre `references/formulas-copy.md`.

## 3. Mensaje (→ categoría 2)

Evalúa si el contenido está escrito desde el cliente o desde la empresa: si abre por el problema del visitante y no por la historia corporativa, si usa lenguaje llano, si traduce características en beneficios, si muestra una transformación antes/después, si responde objeciones, si comunica el costo de no actuar, y si cada sección cumple una función dentro del recorrido comercial.

**Prueba "nosotros vs. tú":** cuenta aproximadamente cuántas veces el sitio dice "nosotros / nuestra empresa / nuestra experiencia" frente a "tú / tu problema / lo que vas a lograr". Reporta el conteo como dato. Un sitio que habla más de sí mismo que del cliente tiene un problema de mensaje, no de diseño.

**Dos verificaciones de coherencia que casi nadie hace y que rinden mucho:**

- **Cifras entre secciones.** Compara todas las cifras que el sitio afirma sobre sí mismo —años, clientes, proyectos, porcentajes— y verifica que no se contradigan entre bloques o entre páginas. Una contradicción numérica en la misma página es un hallazgo de alto impacto y bajo esfuerzo, y es especialmente dañina cuando el sitio vende rigor, precisión o transparencia. Reporta también los indicadores que no son cifras ("∞ horas ahorradas", "resultados ilimitados"): en un sitio que promete medición, un indicador no medible contradice el argumento.
- **Idioma entre versiones.** En sitios multilingües, recorre la misma plantilla en cada idioma y busca cadenas sin traducir: encabezados de sección, etiquetas de campo, migas de pan y sobre todo **los botones**. Un CTA en el idioma equivocado en una página de conversión es fuga directa, y es frecuente porque las cadenas de plantilla se traducen después que el contenido.


## 4. Estructura y navegación (→ categoría 3)

Menú principal simple (idealmente cinco elementos o menos), jerarquía de páginas clara, CTA visible en el encabezado, ausencia de callejones sin salida, flujo lógico entre secciones, navegación consistente, footer útil, acceso directo a la acción principal, y ausencia de opciones que compitan entre sí.

El recorrido de referencia es: **problema → solución → beneficios → prueba → oferta → acción**. Señala cualquier sección que rompa ese orden y explica el costo de la ruptura.

## 5. Credibilidad y confianza (→ categoría 4)

La confianza tiene que aparecer *antes* de pedir la acción importante, no después.

Busca testimonios específicos, casos con resultados medibles, historias antes/después, logos de clientes o medios, certificaciones relevantes, fotos reales del equipo o del trabajo, información de contacto verificable, garantías y condiciones, señales de seguridad, preguntas frecuentes y transparencia en precio o proceso cuando corresponda al modelo de negocio.

Un testimonio que solo dice "excelente servicio, muy recomendados" no es prueba social: es decoración. Cuéntalo como ausencia parcial.

## 6. Llamados a la acción (→ categoría 5)

Cada página necesita una acción dominante. Evalúa visibilidad sin scroll, especificidad del texto, correspondencia con la intención del usuario en esa página, repetición estratégica, explicación de qué pasa después del clic, reducción de riesgo, brevedad del formulario, existencia de un CTA secundario para el visitante no listo, contraste visual del botón, y coherencia entre botón, destino y resultado.

Rechaza CTAs genéricos ("Saber más", "Enviar", "Contáctanos", "Ver más"). En `references/formulas-copy.md` hay un banco de reemplazos por tipo de negocio.

## 7. Embudo (→ categoría 6)

Clasifica lo que encuentres en el sitio dentro de cinco etapas — **atracción, interés, deseo, acción, fidelización** — y señala cuáles están vacías o débiles.

La etapa que casi siempre falta en sitios de PyME es la de interés: no hay nada que capture al visitante que no está listo para comprar hoy. Si no existe ninguna oferta intermedia (guía, checklist, diagnóstico, lista de precios, disponibilidad), dilo con claridad: ese sitio solo convierte al 2–3% que llegó decidido y pierde al resto sin dejar rastro.

## 8. Automatización y medición (→ categoría 8)

Con lo verificado en el Paso 1b, evalúa si el sitio puede capturar, dar seguimiento y medir sin depender de trabajo manual: formularios conectados a algún destino, confirmación automática, secuencias de email, seguimiento de leads, recuperación de carritos o solicitudes incompletas, píxeles instalados, eventos de conversión configurados y automatización de agendamiento.

**Verifica primero que exista medición.** Si no hay analítica instalada, ese es el hallazgo número uno del informe y además invalida las hipótesis del bloque 10 de la plantilla (Hipótesis de conversión): no se puede probar nada sobre lo que no se mide. Dilo explícitamente.

Distingue siempre entre lo que está instalado (observado) y lo que está bien configurado (normalmente no verificable desde fuera).

## 9. Experiencia móvil y usabilidad (→ categoría 7)

Solo si tienes capturas o navegador. Legibilidad, tamaño de botones, espaciado, formularios, menú móvil, jerarquía visual, contraste, scroll excesivo, elementos superpuestos, pop-ups intrusivos y facilidad de completar la acción principal con una sola mano.

Sin capturas, esta categoría se marca como no evaluada. No la adivines.

## Módulos de vertical

Si el sitio pertenece a un vertical con módulo propio, ábrelo antes de puntuar. Un módulo de vertical aporta chequeos adicionales y **ajustes a los criterios existentes** — nunca categorías nuevas ni puntos extra, para no descalibrar la rúbrica base y poder comparar sitios de negocios distintos.

| Vertical | Módulo | Actívalo cuando |
|---|---|---|
| E-commerce | `references/vertical-ecommerce.md` | El sitio venda productos con carrito y checkout, en cualquier plataforma. No lo actives para servicios que se cotizan ni catálogos sin transacción. |
| Servicios con reserva/agenda | `references/vertical-reservas.md` | La acción principal sea reservar o agendar una cita, mesa, sesión o consulta, con o sin pago. Si la reserva cobra por adelantado, no actives además e-commerce salvo que también venda productos con carrito. |
| B2B de ticket alto | `references/vertical-b2b-ticket-alto.md` | Venta consultiva de ticket alto, con ciclo de semanas o meses y decisión multi-rol (SaaS, consultoría, industrial). No lo actives para B2B de decisión rápida. |

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
3. **Puntos aplicables** = 100 − la suma de los máximos de los subcriterios marcados **NA**.
4. Score = (puntos obtenidos ÷ puntos evaluables) × 100, redondeado.
5. Cobertura = (puntos evaluables ÷ puntos aplicables) × 100 %.

**NA reduce la base del score, no la cobertura:** la cobertura mide lo que no pudiste ver (NE), no lo que no aplica al modelo de negocio. El score no cambia — sigue siendo obtenidos ÷ evaluables. El umbral del 70 % de abajo se aplica sobre esta cobertura.

Preséntalo así en el veredicto cuando solo hubo NE (nada NA):

> **Score: 61/100 — Regular** · Cobertura de auditoría: 84 % (no se evaluaron experiencia móvil y usabilidad —sin capturas ni datos de PageSpeed— ni automatización y medición —sin acceso al código—).

Cuando además hubo subcriterios NA, sepáralos de la cobertura para no presentarlos como huecos de auditoría:

> **Score: 61/100 — Regular** · Base aplicable: 94/100 (navegación no aplica: landing única) · Cobertura: 83 % (no se evaluaron experiencia móvil ni velocidad por falta de capturas y de datos de PageSpeed).

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

Ancla impacto y esfuerzo en vez de puntuarlos por impresión:

| | Impacto | Esfuerzo |
|---|---|---|
| **Alto** | Vive en una superficie de alcance estructural (bloque superior de la home, plantilla que se repite en todo el catálogo, o la página donde ocurre la conversión) **y** obstaculiza directamente la acción principal. | Desarrollo, integración o rediseño (semanas; horizonte de 30 días). |
| **Medio** | Cumple una de las dos condiciones de "alto", o es transversal al sitio sin tocar la acción (medición, footer, navegación). | Cambios de plantilla o secciones nuevas (días; horizonte de 7 días). |
| **Bajo** | Ninguna de las dos. | Texto o configuración, sin desarrollador (horas; horizonte de 24h). |

Sin analítica, el alcance del impacto se juzga por estructura, nunca por tráfico supuesto (regla de calidad 1); con analítica, se sustenta con las sesiones reales de esas páginas. **Desempate:** a igual ratio, primero lo más cercano a la acción de conversión. **Precedencia:** los órdenes ya mandatados por el skill —analítica ausente como hallazgo número uno— prevalecen sobre el ratio.

---

# Paso 5 — Entregable

## Informe completo

Construye el informe siguiendo `references/plantilla-informe.md`, que contiene los diez bloques obligatorios y sus tablas.

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

**Alcance de evidencia — reduce el entregable, no el rigor.** Ejecuta el Paso 0 igual (sin bloquear por falta de respuestas) y el Paso 1 solo sobre la home y la página de conversión, sin benchmark (1g) ni cruce de plantillas (1d). Puntúa con la rúbrica completa aplicando NE y normalización como siempre, y declara la cobertura resultante — será menor, y eso está bien. Si aun así la cobertura queda bajo el 70 %, aplica la regla del Paso 3: entrega las tres fugas, el titular y el CTA sin score, y di exactamente qué evidencia falta para cerrarlo.

**Cierre.** Esta versión funciona bien como diagnóstico previo a una propuesta. Ciérrala así:

1. Declara el total de fugas detectadas y nómbralas en una línea cada una, sin evidencia ni solución — solo las tres principales van desarrolladas con cita textual y URL ("Se detectaron 9 fugas; este diagnóstico desarrolla las 3 de mayor impacto"). No viola la regla de evidencia del Paso 4: las fugas ya se verificaron durante el análisis; la lista es un índice, no hallazgos desarrollados.
2. Cierra con un bloque fijo de lo que agrega la auditoría completa, alineado con los bloques de `plantilla-informe.md`: auditoría página por página, embudo por etapas, benchmark competitivo, mejoras de contenido con dos variantes de titular, plan 24h / 7 días / 30 días, hipótesis de conversión medibles y documento Word.
3. Ajusta el tono según el destinatario declarado en el Paso 0: si es entrega a cliente, el cierre es la oferta comercial; si es uso interno, es el índice de la profundidad disponible — mismo bloque, sin lenguaje de venta.

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
| `references/plantilla-informe.md` | Al redactar el entregable. Las 12 secciones (10 obligatorias) con sus tablas y un ejemplo de veredicto. |
| `references/formulas-copy.md` | Al escribir las mejoras de contenido: fórmulas de titular, banco de CTAs por tipo de negocio, formato de testimonio, bloques de reducción de riesgo. |
| `references/contexto-colombia.md` | Cuando el mercado objetivo sea Colombia o LatAm. Canal, pagos, confianza y tratamiento de datos personales. |
| `references/vertical-ecommerce.md` | Cuando el sitio sea una tienda con carrito y checkout. Recorrido de checkout, comprobación cruzada de políticas, y ajustes a la rúbrica base. |
| `references/vertical-reservas.md` | Cuando la acción principal sea reservar o agendar. Recorrido del flujo de reserva, disponibilidad, recordatorio y ajustes a la rúbrica. |
| `references/vertical-b2b-ticket-alto.md` | Cuando la venta sea consultiva de ticket alto y ciclo largo. Formulario como filtro, contenido para el comité, página reenviable y ajustes a la rúbrica. |
| `references/accesibilidad-y-seo.md` | Cuando actives el módulo complementario. Rúbrica de 20 puntos aparte, con la delimitación frente al skill `seo` y el marco normativo. |
