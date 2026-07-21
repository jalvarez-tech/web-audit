# Contexto Colombia y LatAm

Abre este archivo cuando el mercado objetivo sea Colombia o Latinoamérica. Un marco de conversión anglosajón aplicado tal cual a un sitio colombiano produce hallazgos correctos en lo general y equivocados en lo que decide la venta.

## Contenido

1. [El canal manda](#1-el-canal-manda)
2. [Medios de pago](#2-medios-de-pago)
3. [Señales de confianza locales](#3-señales-de-confianza-locales)
4. [Precio y presentación](#4-precio-y-presentación)
5. [Tratamiento de datos personales](#5-tratamiento-de-datos-personales)
6. [Comercio electrónico y consumidor](#6-comercio-electrónico-y-consumidor)
7. [Ajustes a la puntuación](#7-ajustes-a-la-puntuación)

---

## 1. El canal manda

En Colombia, WhatsApp no es un canal secundario: en muchos sectores **es** el canal de venta. Un sitio que empuja al visitante hacia un formulario de contacto cuando su segmento resuelve todo por WhatsApp está perdiendo conversiones por diseño, aunque el formulario esté impecable.

Qué revisar:

- ¿Existe un enlace a WhatsApp visible sin scroll, en móvil?
- ¿El enlace lleva mensaje prellenado y contexto? (`wa.me/57...?text=Hola,%20vi%20el%20apartamento%20en...`)
- ¿El mensaje prellenado identifica la página de origen? Sin eso, quien atiende empieza a ciegas y la conversación pierde temperatura.
- ¿Hay indicación de horario de atención y tiempo de respuesta?
- ¿Se usa WhatsApp Business con catálogo y respuestas rápidas, o un número personal?

**Y revisa cómo se ve el enlace cuando lo reenvían.** Aquí el contenido no se consume donde se publica: se comparte. La ficha del inmueble llega a la pareja, al socio, al asesor del banco; el producto circula en grupos familiares. Si la página no tiene `og:image` ni `og:description`, ese reenvío aparece como una URL pelada, sin foto ni descripción, y pierde toda su fuerza.

Es el chequeo con mejor relación rendimiento/esfuerzo en un sitio colombiano y casi nadie lo hace. Un catálogo con fotografía profesional que se comparte sin imagen tiene el activo construido y no lo está usando. Ver el Paso 1e y el criterio S3 del módulo complementario.

**Advertencia de diagnóstico:** un número de WhatsApp flotante no compensa la ausencia de propuesta de valor. Muchos sitios colombianos tienen conversión aceptable *a pesar* de la web, porque el vendedor rescata la venta en el chat. Eso no es un sitio que convierte: es un sitio que no estorba demasiado. Dilo así en el informe cuando aplique — y valora si el cuello de botella real está en la web o en el proceso de atención.

Un patrón frecuente: la PyME opera desde Instagram y WhatsApp, y la web cumple un rol de **validación de credibilidad** más que de conversión directa. Si ese es el caso, la categoría 4 (credibilidad) pesa más en la lectura del informe que la 6 (embudo), y conviene decírselo al cliente en el veredicto en lugar de castigar el embudo que nunca quiso construir.

---

## 2. Medios de pago

Para e-commerce, la ausencia de medios locales es una fuga directa. Verifica cuáles aparecen:

| Medio | Qué buscar en el HTML o en el checkout |
|---|---|
| PSE (débito bancario) | Muy usado; su ausencia es una fuga real |
| Nequi / Daviplata | Estándar en compras de ticket bajo y medio |
| Bancolombia a la mano / QR | |
| Tarjetas de crédito y débito | |
| Efectivo (Efecty, Baloto, corresponsales) | Relevante fuera de las capitales |
| Contraentrega | Reduce la barrera de desconfianza en primera compra |
| Financiación (Addi, Sistecrédito, cuotas) | Cambia la conversión en tickets altos |

Pasarelas que verás en el código: `wompi`, `epayco`, `payu`, `mercadopago`, `bold`, `payvalida`.

Si el sitio solo acepta tarjeta internacional o PayPal, márcalo como hallazgo alto: excluye a una porción sustancial del mercado.

---

## 3. Señales de confianza locales

Lo que reduce riesgo percibido aquí no siempre coincide con lo que funciona en un sitio estadounidense:

- **Dirección física visible.** En Colombia pesa más que un sello de seguridad. Un negocio sin dirección se lee como informal.
- **NIT.** Su presencia comunica formalidad.
- **Cámara de Comercio / matrícula mercantil**, cuando aplique.
- **Teléfono fijo o celular real**, no solo formulario.
- **Fotos reales del local, del equipo o del producto**, no banco de imágenes. El uso evidente de stock erosiona confianza más rápido aquí que en mercados anglosajones.
- **Registro sanitario (Invima)** para alimentos, cosméticos, dispositivos.
- **Tarjeta profesional / registro** en servicios regulados: salud, ingeniería, derecho, contaduría.
- **Reseñas de Google del negocio local**, enlazadas o incrustadas.

---

## 4. Precio y presentación

- Precios en **COP** con separador de miles: `$ 1.250.000`. Un precio escrito `$1250000` se lee como error y frena la compra.
- Indica explícitamente si el precio **incluye IVA**. La ambigüedad genera objeción en el momento del pago.
- Para servicios B2B, la transparencia total de precio es menos común que en mercados anglosajones. No penalices su ausencia automáticamente; sí penaliza que no exista **ninguna** señal de rango, criterio de cotización o punto de partida. El visitante que no puede estimar si está en su presupuesto se va sin escribir.
- Si el sitio vende a extranjeros (turismo, rentas, exportación), verifica que exista referencia en USD o conversión visible.
- Horarios de atención en hora Colombia, declarados.

---

## 5. Tratamiento de datos personales

Cualquier formulario que capture datos personales en Colombia está sujeto al régimen de protección de datos: la **Ley 1581 de 2012** y sus decretos reglamentarios, con la Superintendencia de Industria y Comercio como autoridad de vigilancia. El marco exige, entre otras cosas, autorización previa e informada del titular y la existencia de una política de tratamiento de la información.

Qué revisar y reportar:

| Elemento | Qué buscar |
|---|---|
| Política de tratamiento de datos | Página publicada y enlazada, no solo "política de privacidad" genérica copiada |
| Autorización en el formulario | Casilla de aceptación explícita, no premarcada, con enlace a la política |
| Finalidad declarada | Para qué se usan los datos y por cuánto tiempo |
| Canal de derechos del titular | Correo o mecanismo para consultar, actualizar o suprimir datos |
| Aviso de cookies | Presente y funcional si hay analítica o píxeles publicitarios |
| Registro de bases de datos | Aplica según el tipo y tamaño de la organización; verifica con el cliente |

**Cómo reportarlo.** Preséntalo como un hallazgo de cumplimiento con impacto comercial —un formulario sin autorización expone al negocio y además transmite descuido— y recomienda validación con un abogado. No emitas conceptos jurídicos ni afirmes que el sitio "está en infracción": tu papel es señalar la ausencia observable y su riesgo, no dictaminar.

Este hallazgo aparece en la mayoría de sitios de PyME colombiana y casi nunca lo trae una auditoría de conversión estándar. Es una de las cosas que diferencia el informe.

---

## 6. Comercio electrónico y consumidor

Para tiendas en línea, el **Estatuto del Consumidor (Ley 1480 de 2011)** establece obligaciones específicas de información y derechos del comprador en ventas a distancia, incluido el derecho de retracto dentro de un plazo definido y mecanismos de reversión del pago.

Qué revisar en el sitio:

- ¿Están publicadas las condiciones de compra, envío, cambios y devoluciones, en página propia y accesible desde el checkout?
- ¿Se informa el derecho de retracto y cómo ejercerlo?
- ¿Aparecen identificación del vendedor, dirección y canal de reclamaciones (PQRS)?
- ¿Los tiempos y costos de envío se conocen **antes** del último paso? El costo de envío revelado tarde es una de las causas más consistentes de abandono de carrito.
- ¿Existe seguimiento del pedido?

Igual que arriba: repórtalo como ausencia observable con riesgo asociado, y sugiere validación legal.

---

## 7. Ajustes a la puntuación

Aplica estos ajustes al usar `rubrica-scoring.md` en mercado colombiano:

| Criterio | Ajuste |
|---|---|
| 4.4 Transparencia y reducción de riesgo | Incluye dirección física, NIT y política de datos entre las señales evaluadas. Su ausencia impide llegar a 3. |
| 5.5 Formulario sin fricción | Un enlace a WhatsApp con mensaje precargado y contextual cuenta como ruta de conversión de baja fricción y sube la nota, pero con tope de 2 si el formulario sigue siendo largo. Ver el tope del ajuste en `rubrica-scoring.md`. |
| 6.4 Conversión | Evalúa contra el canal que el segmento realmente usa, no contra el formulario ideal. |
| 8.1 Captura y seguimiento | WhatsApp Business sin CRM es captura sin seguimiento: máximo 1 de 2. |
| 2.4 Manejo de objeciones | La objeción de desconfianza ("¿esto es real?") pesa más aquí que la de precio en primera visita. |

Y una regla de encuadre: si el negocio vende principalmente por Instagram y WhatsApp y la web es de respaldo, dilo en el veredicto y ajusta la recomendación. Recomendarle un embudo de cinco etapas a quien necesita tres testimonios y una dirección visible es una auditoría técnicamente correcta y comercialmente inútil.
