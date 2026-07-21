# Vertical — Servicios con reserva o agenda

Módulo de vertical. Aporta chequeos adicionales y **ajustes a los criterios existentes**, no una categoría nueva. Los 100 puntos de conversión no se tocan: eso preserva la calibración de la rúbrica base y permite comparar un negocio de reservas con cualquier otro sitio auditado.

## Contenido

1. [Cuándo activarlo](#cuándo-activarlo)
2. [Qué agregar a la recolección](#qué-agregar-a-la-recolección)
3. [Chequeos propios de reserva](#chequeos-propios-de-reserva)
4. [Ajustes a la rúbrica](#ajustes-a-la-rúbrica)
5. [Fugas típicas](#fugas-típicas)

---

## Cuándo activarlo

Cuando la acción principal sea **reservar o agendar** una cita, mesa, sesión o consulta, con o sin pago en línea: clínicas y consultorios, restaurantes, salones y estéticas, asesorías, talleres, tours, canchas y coworking.

**Si la reserva cobra por adelantado**, el flujo de reserva cumple el rol del checkout y **no** actives además el módulo de e-commerce, salvo que el sitio también venda productos con carrito (misma exclusión que `vertical-ecommerce.md`).

**No lo actives** para servicios que solo se cotizan por formulario sin agenda, ni para catálogos informativos. Ahí la rúbrica base ya funciona.

Un negocio de reservas tiene una particularidad que cambia el encuadre: **el visitante ya decidió el tipo de servicio; lo que negocia es cuándo, con quién y con qué certeza.** Por eso la disponibilidad visible, la fricción del flujo de reserva y la reducción de la incertidumbre (precio, política de cancelación, recordatorio) pesan más que el copy de la home.

---

## Qué agregar a la recolección

A las páginas del Paso 1a, suma:

1. **La página de servicios o de precios** — para contrastar qué se ofrece y a cuánto.
2. **La política de cancelación y reprogramación.**
3. **El flujo de reserva**, hasta donde puedas llegar.

### Recorrido del flujo de reserva

Es donde se gana o se pierde la cita, y es lo más difícil de auditar desde fuera. Sé explícito sobre cuál de las tres rutas del Paso 1b estás usando.

Con navegador: inicia una reserva, avanza por el calendario y **detente antes de confirmar**. Nunca completes una reserva real ni ingreses datos reales —misma salvaguarda que el checkout de e-commerce—. Observa y anota:

- ¿Se ve la disponibilidad real en el calendario, o hay que llamar/escribir para saber si hay cupo?
- ¿Cuántos pasos hay hasta confirmar? ¿Pide crear cuenta?
- ¿Aparece el precio del servicio antes de reservar?
- ¿Se declara la política de cancelación en el punto de la reserva, no solo en una página aparte?
- ¿La confirmación dice qué pasa después: dónde, cómo llegar, qué llevar?

Sin navegador: marca el flujo como **NE** y dilo. No infieras la experiencia de reserva a partir de que el sitio tenga Calendly o un plugin — dos negocios con la misma herramienta configuran flujos distintos.

### Regla de evidencia del recordatorio

El recordatorio automático (correo/SMS/WhatsApp antes de la cita) casi nunca es observable desde fuera. Cuéntalo como:

- **Observado** solo si el copy del flujo o de la confirmación lo declara ("te enviaremos un recordatorio").
- **Declarado por el cliente** si el usuario lo confirma.
- **NE** en cualquier otro caso.

Nunca lo infieras de la mera presencia de Calendly, `cal.com` o similar: tener la herramienta no prueba que el recordatorio esté activado.

---

## Chequeos propios de reserva

### Disponibilidad

La señal que más reduce fricción. Un calendario que muestra huecos reales convierte; un "escríbenos para agendar" traslada al visitante el trabajo de averiguar si hay cupo, y en móvil eso se pierde.

- ¿La disponibilidad está publicada y actualizada, o es un formulario ciego?
- ¿Se puede elegir profesional/mesa/recurso, o es genérico?
- ¿Los horarios y servicios están vigentes, o hay rastros de temporadas pasadas?

### Certeza antes de reservar

El visitante entrega una franja de su tiempo y, a veces, un anticipo. Reduce su riesgo antes de pedirlo:

- **Precio del servicio** visible antes de reservar, no "consultar".
- **Política de cancelación y reprogramación** en el punto de decisión.
- **Qué incluye** la sesión y cuánto dura.

### Después de reservar

Casi siempre vacío y casi siempre barato de llenar:

- Confirmación con fecha, lugar, cómo llegar y qué llevar.
- Recordatorio automático antes de la cita (la mayor defensa contra el no-show).
- Recaptura de la cita cancelada o no asistida: un enlace para reprogramar en vez de perder al cliente.

---

## Ajustes a la rúbrica

Aplica estos ajustes al puntuar con `rubrica-scoring.md`. Los topes son topes: no se superan aunque el resto del criterio esté bien.

| Criterio | Ajuste |
|---|---|
| **4.4** Transparencia | Requiere **precio del servicio y política de cancelación visibles antes de reservar**. Sin ambas, tope 2. Con contradicción entre lo que dice el flujo y la política, tope 1. |
| **5.4** Siguiente paso | La confirmación debe declarar **qué pasa después**: dónde es, cómo llegar, qué llevar, con quién. Sin eso, tope 1. |
| **5.5** Fricción | Se evalúa sobre el **flujo de reserva**, no sobre el formulario de contacto. Reserva completable en línea con disponibilidad visible → 3. Botón que solo abre WhatsApp sin fecha/hora ni mensaje contextual → tope 1. Flujo no recorrido → NE, no lo estimes. |
| **6.2** Captura de interés | La **disponibilidad publicada** cuenta como captura de interés: convierte al que está listo hoy. Su ausencia (formulario ciego) es una fuga de interés, no solo de acción. |
| **6.5** Fidelización | Se evalúa sobre el **recordatorio** y la **recaptura** de la cita cancelada o no asistida, no sobre recompra ni referidos. |
| **8.2** Emails o automatización | Solo con herramienta de agendamiento instalada → 1. Sube a 2 únicamente con evidencia (observada o declarada) de **confirmación más recordatorio** automatizados. |

---

## Fugas típicas

Ordenadas por frecuencia y por lo barato que es cerrarlas. Úsalas como lista de contraste al final, no como sustituto del análisis.

1. **Calendario sin disponibilidad publicada**: obliga a llamar o escribir para saber si hay cupo. Pierde a todo el que reservaría solo si pudiera verlo.
2. **Precio oculto hasta la reserva** o "consultar valores": el visitante no agenda sin saber cuánto cuesta.
3. **Sin recordatorio automático**: el no-show que se podía evitar con un mensaje.
4. **Horarios o servicios desactualizados**: precios viejos, servicios que ya no se prestan, franjas de una temporada pasada.
5. **WhatsApp como único canal de reserva** sin contexto precargado: quien atiende empieza a ciegas y la agenda se lleva a mano.
6. **Cita cancelada que no se recaptura**: se pierde al cliente en vez de ofrecerle reprogramar.
7. **Política de cancelación enterrada** o contradictoria entre el flujo y la página aparte.
