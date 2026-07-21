# Vertical — B2B de ticket alto

Módulo de vertical. Aporta chequeos adicionales y **ajustes a los criterios existentes**, no una categoría nueva. Los 100 puntos de conversión no se tocan: eso preserva la calibración de la rúbrica base y permite comparar una venta consultiva con cualquier otro sitio auditado.

## Contenido

1. [Cuándo activarlo](#cuándo-activarlo)
2. [Qué agregar a la recolección](#qué-agregar-a-la-recolección)
3. [Chequeos propios de B2B](#chequeos-propios-de-b2b)
4. [Ajustes a la rúbrica](#ajustes-a-la-rúbrica)
5. [Fugas típicas](#fugas-típicas)

---

## Cuándo activarlo

Cuando el sitio venda de forma **consultiva y de ticket alto**, con un ciclo de decisión de semanas o meses y una decisión **multi-rol**: SaaS de contrato anual, consultoría, servicios profesionales de proyecto, maquinaria o insumos industriales de alto valor.

**No lo actives** para B2B de decisión rápida —servicios locales, insumos recurrentes, compra transaccional—, donde la rúbrica base funciona sin ajustes.

Un B2B de ticket alto tiene una particularidad que cambia el encuadre y que la rúbrica base, calibrada para PyME B2C, malinterpreta: **lo que en B2C es fricción, aquí suele ser calificación deliberada.** Un formulario de siete campos que en una landing de servicios locales es una fuga, en una venta con costo comercial alto es un filtro que protege el tiempo del equipo. Además, la decisión no la toma una persona: el sitio debe equipar a un **campeón interno** para que reenvíe el caso y lo defienda ante un comité. La transparencia total de precio no es la norma, y la "fidelización" es *nurture* del lead no listo, no recompra.

---

## Qué agregar a la recolección

A las páginas del Paso 1a, suma:

1. **La página de producto/solución dirigida al comprador técnico** (funcionalidad, integración, seguridad).
2. **La página de casos o clientes**, para verificar si hay resultados con cifra, no solo logos.
3. **Cualquier activo descargable** que aparezca: caso en PDF, one-pager, calculadora de ROI, comparativa.

Si no lo sabes ya por el encuadre, confírmalo con el usuario: **¿ticket aproximado y cuánto dura típicamente la venta?** — decide si este módulo aplica y calibra qué campos del formulario son calificación legítima.

---

## Chequeos propios de B2B

### El formulario como filtro, no como barrera

Cuenta los campos, pero **júzgalos por lo que califican**, no por su número. Un campo que segmenta de verdad (cargo, tamaño de empresa, plazo del proyecto) gana el derecho a existir; pedir el teléfono para descargar un PDF no. La pregunta correcta no es "¿cuántos campos?" sino "¿este campo protege el costo comercial o solo estorba?".

### El CTA nombra lo que se recibe

En ticket alto, "Contáctanos" no dice nada. El CTA fuerte nombra el entregable y su forma: "Agenda una demo personalizada de 30 min", "Solicita el análisis de tu caso". Y debe existir una **ruta paralela de baja fricción** para el que aún no está listo para hablar con ventas: un recurso que se lleva sin agendar nada.

### Contenido para el comité

La decisión pasa por varios roles con preguntas distintas: el **usuario** ("¿me facilita el trabajo?"), el **comprador económico** ("¿qué retorno y a qué costo?"), el **evaluador técnico** ("¿integra, es seguro, cumple?"). Un sitio que solo le habla a uno deja a los otros dos sin munición.

### La página reenviable al comité (chequeo sin puntos)

El campeón interno rara vez decide; **reenvía**. Verifica que la página clave sobreviva al reenvío:

- Metadatos sociales que no la dejen llegar como URL pelada (ver Paso 1e).
- Un one-pager o caso descargable que circule por correo.
- Un criterio de precio citable —rango, "desde", modelo— para que quien no habló con ventas pueda defender el número.

Se reporta como hallazgo de **prioridad alta** cuando falta, sin tocar los pesos del score.

---

## Ajustes a la rúbrica

Aplica estos ajustes al puntuar con `rubrica-scoring.md`, **solo donde el ancla base entra en conflicto real** con la dinámica B2B. Los topes son topes.

| Criterio | Ajuste |
|---|---|
| **2.4** Objeciones | Para 2 se exige contenido para los **roles del comité** (usuario, comprador económico, evaluador técnico). Un FAQ genérico que solo atiende a uno → tope 1. |
| **4.2** Resultados específicos | Para 3, al menos un caso con **cifra de resultado y cliente identificable** del segmento. Solo logos, sin resultado → tope 1. |
| **5.5** Fricción | Se evalúa el **balance calificación/valor**, no el conteo bruto: 4–7 campos son aceptables para 3 si cada campo califica de verdad (cargo, tamaño de empresa, plazo) **y** el CTA nombra lo que se recibe. Pedir teléfono para descargar un PDF → tope 1. Sin ruta paralela de baja fricción para el no-listo → tope 2 (coherente con el tope ya existente en 5.5). |
| **6.2** Captura de interés | La oferta intermedia esperada es de **ciclo largo**: caso descargable, calculadora de ROI, comparativa contra alternativas. Un checklist genérico → tope 2. |
| **6.5** Fidelización | Se evalúa sobre el **nurture del lead no listo** (secuencia post-descarga, contenido de decisión), no sobre recompra ni referidos. |

---

## Fugas típicas

Ordenadas por frecuencia. Úsalas como lista de contraste al final, no como sustituto del análisis.

1. **CTA único de alta fricción** ("Contáctanos") sin ruta para el que aún investiga: se pierde a todo el mercado que no está listo para hablar con ventas hoy.
2. **Casos que son solo logos**, sin una cifra de resultado ni un cliente reconocible del segmento.
3. **Página que solo le habla al usuario final**, sin munición para el comprador económico ni el evaluador técnico.
4. **Precio totalmente opaco**, sin rango ni "desde", que deja al campeón interno sin cómo defender el número.
5. **Página clave no reenviable**: sin metadatos, sin one-pager, llega al comité como una URL pelada.
6. **Formulario que filtra por barrera y no por calificación**: pide datos que no segmentan y ahuyenta al lead bueno.
7. **Sin oferta intermedia de ciclo largo**: nada que capture al que está a meses de decidir.
