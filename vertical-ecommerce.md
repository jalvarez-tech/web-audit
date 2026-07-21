# Vertical — E-commerce

Módulo de vertical. Aporta chequeos adicionales y **ajustes a los criterios existentes**, no una categoría nueva. Los 100 puntos de conversión no se tocan: eso preserva la calibración de la rúbrica base y permite comparar una tienda con cualquier otro sitio auditado.

## Contenido

1. [Cuándo activarlo](#cuándo-activarlo)
2. [Qué agregar a la recolección](#qué-agregar-a-la-recolección)
3. [Chequeos propios de tienda](#chequeos-propios-de-tienda)
4. [Ajustes a la rúbrica](#ajustes-a-la-rúbrica)
5. [Fugas típicas](#fugas-típicas)

---

## Cuándo activarlo

Cuando el sitio venda productos con carrito y checkout, sea la plataforma que sea. Los metadatos de plataforma del Paso 1b suelen delatarla sin necesidad de preguntar.

**No lo actives** para servicios que se cotizan, reservas sin pago en línea, o catálogos sin transacción. Ahí la rúbrica base ya funciona: el checkout no existe y forzar estos criterios genera hallazgos irrelevantes.

Una tienda tiene una particularidad que cambia el encuadre entero: **el visitante no viene a informarse, viene a comprar.** Eso reordena las prioridades. Un sitio de servicios puede permitirse construir confianza a lo largo de varias visitas; una tienda tiene que resolver ajuste, precio total, riesgo y entrega en la misma sesión, casi siempre en la ficha de producto. Por eso la ficha pesa más que la home en el diagnóstico, y por eso las objeciones no resueltas se castigan más fuerte.

---

## Qué agregar a la recolección

A las páginas del Paso 1a, suma:

1. **Listado de la colección principal** — para el barrido de variantes.
2. **Dos fichas de producto**, no una: una del producto más caro y otra del más barato. Las tiendas suelen tener la ficha estrella cuidada y el resto sin terminar.
3. **Páginas de política**: envío, devoluciones y cambios, privacidad, términos.
4. **Carrito y checkout**, hasta donde puedas llegar.

### Recorrido de carrito y checkout

Es donde se pierde el dinero y es lo más difícil de auditar desde fuera. Sé explícito sobre cuál de las tres rutas del Paso 1b estás usando.

Con navegador: agrega un producto, ve al carrito, entra al checkout y **detente antes de cualquier pago**. Nunca completes una compra ni ingreses datos reales. Observa y anota:

- ¿Se puede comprar sin crear cuenta?
- ¿Cuántos pasos hay hasta el pago?
- ¿En qué momento aparece el costo de envío? ¿Y los impuestos? ¿Y los aranceles?
- ¿Hay billeteras digitales o checkout acelerado?
- ¿Se puede editar el carrito sin perder el avance?
- ¿Qué señales de seguridad y qué medios de pago se muestran?

Sin navegador: marca el checkout como **NE** y dilo. No infieras la experiencia de compra a partir de la plataforma — dos tiendas en el mismo Shopify tienen checkouts distintos. Lo que sí puedes observar en ruta C: presencia de billeteras digitales en los metadatos de plataforma, el mensaje del carrito vacío, y si la tienda invita a iniciar sesión antes de comprar.

### Comprobación cruzada de políticas

Lee las páginas de política y **contrástalas contra lo que promete la ficha de producto y el pie**. Envío gratis, ventana de devolución, quién paga el retorno, plazo de entrega.

Esta comprobación existe porque la contradicción es sistemática: la ficha, la barra de confianza, el pie y la página de política se editan en momentos distintos y por personas distintas. Cuando la ventana de devolución dice una cosa junto al botón de compra y otra doscientos píxeles más abajo, no es un descuido de copy — es una promesa comercial poco confiable en el punto exacto donde se decide una compra, y expone al negocio si un cliente reclama dentro de la ventana más larga.

---

## Chequeos propios de tienda

### Ficha de producto

Es la página que vende. Audítala con más rigor que la home.

| Qué revisar | Qué buscas |
|---|---|
| Fotografía | Tomas **únicas** —cuenta duplicados subidos en dos formatos— con las vistas que la categoría exige: frontal, lateral, detalle de material y el producto en uso |
| Escala real | Cómo sabe el comprador el tamaño verdadero: medidas, referencia junto a un objeto conocido, producto sobre persona con su talla indicada |
| Guía de tallas o ajuste | Que exista, sea accesible desde la ficha sin salir de ella, y sea específica del producto y no una tabla genérica |
| Disponibilidad de variantes | Ver el barrido del Paso 1a |
| Precio total | Si el impuesto está incluido, si hay financiación, si el precio mostrado es el que se cobra |
| Envío | Costo y plazo visibles **antes** del carrito |
| Devolución | Ventana, quién paga el retorno, cómo se inicia, si hay cambio de talla |
| Reseñas | Cantidad, recencia, distribución de estrellas, si la marca responde |
| Preguntas | Sección de preguntas, FAQ del producto o chat |
| Urgencia | Si hay contadores o alertas de stock, que correspondan a existencias reales |

### Confianza de tienda

Distinta de la confianza de un sitio de servicios. Aquí el comprador entrega dinero a un desconocido antes de recibir nada.

- **Reseñas de producto** con volumen y fechas recientes. Es la señal dominante; casi nada la sustituye.
- **Identidad verificable**: razón social, dirección física, teléfono o canal de atención con horario.
- **Medios de pago** visibles antes del checkout.
- **Contenido real de clientes**, no solo producción de marca.
- **Política de cambios** explicada, no solo enlazada.

### Venta transfronteriza

Si la tienda ofrece varias divisas o envía fuera de su país, revisa:

- Quién paga los **aranceles e impuestos de importación**, y si se dice antes de pagar. El cargo sorpresa en la entrega es una de las peores experiencias de compra que existen y genera contracargos.
- **Plazos por destino**, no un plazo único.
- **Devoluciones internacionales**: quién paga el retorno y a qué dirección.
- Que la divisa mostrada corresponda al país seleccionado. Un país configurado con la divisa equivocada es un error observable y frecuente.

### Post-compra

Casi siempre vacío y casi siempre barato de llenar:

- Confirmación con lo que sigue y cuándo.
- Seguimiento del envío.
- Contenido de uso o cuidado. Si la ficha ya tiene instrucciones de cuidado, ese contenido es un correo post-compra listo y nadie lo está usando.
- Solicitud de reseña — que además alimenta el punto más débil de casi toda tienda nueva.
- Reposición o recompra.

---

## Ajustes a la rúbrica

Aplica estos ajustes al puntuar con `rubrica-scoring.md`. Los topes son topes: no se superan aunque el resto del criterio esté bien.

| Criterio | Ajuste |
|---|---|
| **1.3** Resultado | En tienda el resultado es el producto en uso. Sin mostrarlo en contexto y a escala real, tope 2. |
| **2.2** Beneficios | Ficha técnica completa —material, medida, origen, cuidado— es requisito para 3 o más. |
| **2.4** Objeciones | Las tres objeciones de tienda son **ajuste, devolución y entrega**. Si alguna queda sin resolver en la ficha, tope 1. |
| **4.1** Testimonios | Se reemplaza por **reseñas de producto**. Sin reseñas en la ficha, tope 1 — aunque haya testimonios de marca en otra página. La reseña de producto y el testimonio de marca no son intercambiables: la compradora quiere saber si *ese* producto cumplió, no si la empresa cae bien. |
| **4.2** Resultados específicos | Aquí son volumen, recencia y distribución de reseñas, no cifras de caso. Sin ninguna reseña, 0. |
| **4.4** Transparencia | Requiere ventana de devolución clara, quién paga el retorno, y tratamiento de aranceles si vende al exterior. Sin las tres, tope 2. Con contradicción entre ficha y política, tope 1. |
| **5.4** Siguiente paso | Costo y plazo de envío visibles antes del carrito. Sin eso, tope 1. |
| **5.5** Fricción | Se evalúa sobre el **checkout**, no sobre el formulario de contacto. Compra como invitado más billeteras digitales → 3. Cuenta obligatoria para comprar → tope 1. Checkout no recorrido → NE, no lo estimes. |
| **6.2** Captura de interés | "Avísame cuando vuelva" cuenta como captura, y en una tienda con agotados es la más valiosa que existe: llega justo cuando la intención está en su punto más alto y hoy se pierde entera. |
| **6.4** Conversión | La cobertura de variantes entra aquí. Rango de tallas o medidas incompleto sin captura de reingreso → tope 1, sin importar qué tan bueno sea el resto del checkout. |
| **6.5** Fidelización | Se evalúa sobre el post-compra: confirmación, seguimiento, contenido de uso, solicitud de reseña, recompra. |

---

## Fugas típicas

Ordenadas por frecuencia con la que aparecen y por lo barato que es cerrarlas. Úsalas como lista de contraste al final, no como sustituto del análisis.

1. **Costo de envío revelado en el último paso.** La causa más consistente de abandono de carrito que existe.
2. **Cuenta obligatoria para comprar.**
3. **Agotados que desaparecen del listado** en lugar de mostrarse con captura de reingreso. La tienda se vuelve invisible para su propia demanda.
4. **Ficha sin escala real**: fotos hermosas de las que no se deduce el tamaño.
5. **Sin reseñas, o solo cinco estrellas sin volumen** — que se lee como reseñas filtradas y resta más de lo que suma.
6. **Aranceles sorpresa** en la entrega internacional.
7. **Devolución contradictoria** entre ficha, barra de confianza, pie y página de política.
8. **Secciones de plantilla vacías**: "productos relacionados", "también te puede gustar", "opiniones", con encabezado y sin contenido.
9. **Urgencia falsa**: contadores que se reinician, "últimas unidades" permanente.
10. **Bloques por defecto de la plataforma sin personalizar** — el texto genérico de newsletter en una marca de lujo delata que nadie revisó esa sección, y aparece justo donde la intención de compra es más alta.
