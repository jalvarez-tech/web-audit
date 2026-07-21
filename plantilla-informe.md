# Plantilla del informe de auditoría

Usa esta estructura exacta. Doce secciones numeradas; **diez son obligatorias** en la versión completa. La 7 (Benchmark competitivo) solo aplica si hay competidores; la 12 (Bloque complementario) solo si el módulo fue activado; el bloque 4b (Escenario económico) solo si el cliente entregó las cifras. La versión rápida no usa esta plantilla: entrega los seis ítems definidos en SKILL.md, Paso 5.

## Contenido

1. [Portada y ficha técnica](#1-portada-y-ficha-técnica)
2. [Veredicto ejecutivo](#2-veredicto-ejecutivo)
3. [Tabla de puntuación](#3-tabla-de-puntuación)
4. [Las 5 fugas principales](#4-las-5-fugas-principales)
4b. [Escenario económico](#4b-escenario-económico) · solo si el cliente entregó las cifras
5. [Auditoría página por página](#5-auditoría-página-por-página)
6. [Evaluación del embudo](#6-evaluación-del-embudo)
7. [Benchmark competitivo](#7-benchmark-competitivo) · solo si hay competidores
8. [Mejoras de contenido](#8-mejoras-de-contenido)
9. [Plan de acción priorizado](#9-plan-de-acción-priorizado)
10. [Hipótesis de conversión](#10-hipótesis-de-conversión)
11. [Seguimiento y re-auditoría](#11-seguimiento-y-re-auditoría)
12. [Bloque complementario — accesibilidad y SEO comercial](#12-bloque-complementario--accesibilidad-y-seo-comercial) · solo si el módulo fue activado

[Generación del documento Word](#generación-del-documento-word) — sección de proceso, no es un bloque del informe.

---

## 1. Portada y ficha técnica

| Campo | Contenido |
|---|---|
| Sitio auditado | URL |
| Cliente / negocio | |
| Fecha | |
| Acción principal evaluada | comprar / reservar / cotizar / agendar / WhatsApp |
| Mercado objetivo | |
| Páginas auditadas | lista de URLs |
| Evidencia visual | capturas recibidas / no recibidas |
| Método de inspección | navegador / código aportado por el cliente / solo obtención de páginas |
| Módulos activados | vertical / contexto local / complementario, o ninguno |
| Checkout recorrido | sí, hasta el paso N / no — solo tienda |
| Datos de velocidad | PageSpeed recibido / no disponible |
| Cobertura de auditoría | % |

Esta ficha protege el informe. Un cliente que sabe qué se miró no discute los hallazgos; discute las prioridades, que es la conversación útil.

---

## 2. Veredicto ejecutivo

Máximo una página. Contiene:

- Score total con estado y cobertura.
- Conclusión de tres a cinco líneas.
- La razón principal por la que el sitio pierde clientes.
- La mayor oportunidad, expresada en términos comerciales.

**Ejemplo del tono y el nivel de concreción esperado:**

> **Score: 58/100 — Débil** · Cobertura de auditoría: 92 %
>
> El sitio transmite una imagen profesional, pero funciona como catálogo y no como sistema de ventas. El titular actual ("Soluciones integrales para su empresa") no nombra a ningún cliente ni ningún problema, y el visitante llega al pie de página sin haber encontrado una sola razón concreta para escribir. La fuga mayor está entre la propuesta de valor y el CTA: hay siete servicios listados y ninguna acción dominante.
>
> La oportunidad más grande no requiere rediseño. Reescribir el bloque superior, agregar tres testimonios con resultados y reducir el formulario de contacto de nueve campos a tres son cambios de una semana que actúan sobre el 100 % del tráfico actual.

Evita el diagnóstico decorativo. "Hay oportunidades de mejora en la experiencia de usuario" no le dice nada a nadie.

---

## 3. Tabla de puntuación

| Categoría | Score | Máximo | Estado | Observación principal |
|---|---:|---:|---|---|
| Posicionamiento y claridad | | 15 | | |
| Mensaje y contenido | | 15 | | |
| Estructura y navegación | | 12 | | |
| Credibilidad y confianza | | 12 | | |
| CTA y conversión | | 15 | | |
| Embudo de ventas | | 15 | | |
| Móvil y usabilidad | | 8 | | |
| Automatización y medición | | 8 | | |
| **Total** | | **100** | | |

Si hubo subcriterios NE o NA, agrega una fila debajo, separando ambos conceptos (NE baja la cobertura; NA baja la base aplicable, con una justificación de una línea por cada NA):

> Base aplicable: 100 de 100 (ningún NA). Puntos evaluables: 84 de 100. Score normalizado: 61/100. Cobertura: 84 %.
> No evaluados (NE): experiencia móvil y usabilidad (sin capturas ni datos de PageSpeed), automatización y medición (sin acceso al código).
> No aplicables (NA): ninguno.

---

## 4. Las 5 fugas principales

Ordenadas por impacto sobre esfuerzo. Para cada una:

**Fuga N — [nombre corto y comercial]**

| | |
|---|---|
| **Dónde** | URL y sección exacta |
| **Qué observé** | Cita textual del sitio o descripción de lo observado |
| **Por qué cuesta ventas** | Mecanismo concreto, no genérico |
| **Qué cambiar** | Instrucción accionable |
| **Cómo se vería** | El texto o la estructura ya escrita, lista para implementar |
| **Impacto / Esfuerzo** | alto-medio-bajo / alto-medio-bajo |

El campo "Cómo se vería" es obligatorio. Un informe que dice qué está mal sin mostrar la alternativa es media auditoría.

---

## 4b. Escenario económico

Solo si el cliente entregó las tres cifras: visitas mensuales, tasa de conversión actual y ticket promedio (o valor de un lead). Si falta cualquiera, omite la tabla y escribe una línea que las pida por nombre — funciona como gancho de seguimiento.

Línea base, con los datos del cliente etiquetados como "dato del cliente":

> Hoy: [visitas]/mes × [conversión] % × [ticket] = [ingreso estimado actual].

Dos escenarios sobre esa línea base, calculados a nivel **agregado del plan de acción**, nunca por fuga individual:

| Escenario | Conversión | Contactos/ventas al mes | Δ vs. hoy |
|---|---|---|---|
| Conservador | [p. ej. 1,2 % → 1,5 %] | | |
| Optimista | [p. ej. 1,2 % → 1,8 %] | | |

Fórmula visible: **visitas × Δ conversión × valor**. Los deltas van etiquetados como "supuesto ilustrativo".

> *Escenario ilustrativo construido con tus datos; no es una proyección ni una promesa de resultado.*

Prohibido: cifra única sin rango, atribuir un delta a una fuga concreta, y activar el bloque con datos parciales. No entra en la versión rápida, no suma ni resta al score y no cuenta en la cobertura.

---

## 5. Auditoría página por página

Una tabla por página auditada. Si la página es una instancia de plantilla, indícalo en el encabezado.

**[Nombre de la página] — [URL]**

| | |
|---|---|
| Objetivo comercial | |
| Qué funciona | |
| Qué no funciona | |
| CTA presente | |
| CTA que debería tener | |
| Mejora prioritaria | |

### Consistencia entre plantillas

Con lo cruzado en el Paso 1d. Solo incluye las filas donde encontraste divergencia — una tabla llena de "igual en todas" no aporta nada.

| Elemento | Páginas del grupo A | Páginas del grupo B |
|---|---|---|
| Orden del menú principal | | |
| URL de la sección [X] | | |
| Prefijo de idioma en enlaces | | |
| Mensaje precargado en el CTA | | |
| Cadenas de plantilla traducidas | | |

Ver las dos columnas lado a lado convence más rápido que cualquier descripción en prosa, y le señala al equipo técnico exactamente dónde mirar.

---

## 6. Evaluación del embudo

| Etapa | Qué encontré | Estado | Fuga detectada | Recomendación |
|---|---|---|---|---|
| Atracción | | | | |
| Interés | | | | |
| Deseo | | | | |
| Acción | | | | |
| Fidelización | | | | |

Cierra con un párrafo que nombre la etapa más débil y explique qué pasa hoy con el visitante que no está listo para comprar. Ese párrafo suele ser el que vende el proyecto de mejora.

---

## 7. Benchmark competitivo

Solo si hubo competidores. Cinco ejes, sin auditarlos a fondo.

| Eje | [Sitio] | [Competidor A] | [Competidor B] |
|---|---|---|---|
| Claridad en 5 segundos | | | |
| Especificidad del titular | | | |
| Prueba social visible arriba | | | |
| Claridad del CTA principal | | | |
| Reducción de riesgo | | | |

Cierra con una línea: qué está resolviendo el competidor para el mismo visitante que este sitio no resuelve.

---

## 8. Mejoras de contenido

Escribe las versiones. No describas lo que habría que escribir.

| Elemento | Actual | Propuesto |
|---|---|---|
| Titular principal | cita textual | versión escrita |
| Subtítulo | | |
| CTA principal | | |
| CTA secundario | | |
| Bloque de beneficios | | |
| Bloque de prueba social | | |
| Bloque de reducción de riesgo | | |
| CTA de cierre | | |

Cuando propongas un titular, ofrece **dos variantes** con enfoques distintos (por ejemplo, una centrada en el problema y otra en el resultado) para que el cliente elija y, solo si el volumen de conversiones lo permite, como material de prueba A/B; si no, para elegir una variante e implementarla midiendo secuencialmente (ver la regla de viabilidad del bloque 10).

Las fórmulas están en `formulas-copy.md`.

### Bloque superior — antes y después

El momento que convierte el informe en proyecto: mostrar el inicio de la home actual junto a cómo quedaría.

**Antes** — las citas textuales ya recolectadas en el Paso 1, en el orden en que aparecen (entrecomilladas y en cursiva).

**Después** — la composición completa en orden de lectura: la variante de titular recomendada (la segunda variante de la tabla queda como alternativa A/B), subtítulo, CTA principal con su microcopy bajo el botón, y la primera señal de confianza.

En el Word van como **dos cuadros consecutivos**, no lado a lado (en página carta quedan estrechos). Dos salvaguardas: (1) sin capturas ni navegador, preséntalo como "orden de lectura del inicio de la página", nunca como "lo que se ve sin hacer scroll" (Paso 1c); (2) es una composición de contenido, no una promesa de diseño visual. Si la sesión tiene herramienta de artifacts/HTML, puedes ofrecer un mockup comparativo como anexo.

---

## 9. Plan de acción priorizado

Tres horizontes. Cada tarea en la tabla.

### Primeras 24 horas — cambios de alto impacto y bajo esfuerzo

Normalmente: reescribir el titular, cambiar el texto del CTA, recortar el formulario, activar analítica si falta.

### Próximos 7 días — estructura, contenido y confianza

Normalmente: reordenar la home según el recorrido de referencia, pedir y publicar testimonios con resultado, agregar bloque de proceso y FAQ, corregir la navegación.

### Próximos 30 días — embudo, automatización y medición

Normalmente: crear la oferta intermedia, configurar eventos de conversión, montar la secuencia de seguimiento, iniciar la primera prueba (A/B o secuencial, según el bloque 10).

Cierra el plan con una tarea fija de medición: **Revisión de resultados** — comparar la métrica de la acción principal y las métricas de las hipótesis del bloque 10 contra su línea base, y decidir la siguiente iteración. Sin este paso, el plan es una lista de tareas, no un ciclo de optimización.

| Prioridad | Acción | Página | Impacto | Esfuerzo | Resultado esperado | Estado |
|---|---|---|---|---|---|---|

La columna **Estado** (hecha / pendiente / bloqueada) le sirve al cliente como tablero de avance entre la entrega y la re-auditoría (ver bloque 11).

---

## 10. Hipótesis de conversión

Entre tres y cinco, comprobables.

| | |
|---|---|
| **Hipótesis** | Si [cambio], entonces [efecto] porque [razón] |
| **Métrica** | Qué se mide |
| **Línea base actual** | Valor actual, o "no medido hoy" |
| **Método de validación** | Cómo se comprueba y en cuánto tiempo |

**Antes de escribir este bloque, verifica que exista medición.** Si el sitio no tiene analítica instalada, ninguna hipótesis es comprobable. En ese caso, escribe una sola línea en su lugar:

> Este bloque queda pendiente hasta instalar medición. Hoy no existe línea base contra la cual validar ningún cambio, lo que convierte cualquier mejora en una apuesta. Instalar analítica y configurar los eventos de conversión es el requisito previo de todo lo demás en este informe.

Esa observación suele ser más valiosa para el cliente que cinco hipótesis decorativas.

**Regla de viabilidad del método de validación.** Antes de proponer un A/B, verifica el volumen de conversiones con los datos de analítica del Paso 0. Con menos de ~200 conversiones/mes en la página afectada —o si el volumen es desconocido, que es el caso por defecto en PyME— **no propongas A/B**: una PyME no alcanza significancia en un plazo razonable. Propón en su lugar **medición secuencial** (comparar 4 semanas antes vs. 4 después del cambio, misma fuente de tráfico, advirtiendo estacionalidad y cambios simultáneos) o **micro-conversiones** (clics en el CTA, inicios de formulario) como métrica intermedia, y dilo explícitamente en el "Método de validación" de cada hipótesis. Si el volumen es desconocido, decláralo y pídelo, en línea con la regla "no inventes datos".

---

## 11. Seguimiento y re-auditoría

Convierte el informe en una relación, no en un PDF que se archiva. Corto y sin duplicar el bloque 10:

**Calendario de verificación.** Referencia las hipótesis del bloque 10 por número y asígnales fecha de revisión, sin repetir métrica ni línea base:

| Hipótesis | Revisar a los 30 días | Revisar a los 60 días |
|---|---|---|
| H1 | | |
| H2 | | |

Si el bloque 10 quedó pendiente por falta de analítica, este bloque hereda esa condición y lo dice en una línea.

**Tablero de avance.** Es la columna "Estado" del plan de acción (bloque 9): el cliente la mantiene como control de qué ya se implementó.

**Re-auditoría comparativa.** Ofrécela con condiciones de comparabilidad explícitas: misma rúbrica y anclas, mismas páginas auditadas, y cobertura igual o superior declarada en ambas fichas técnicas. La comparación se presenta **por categoría**, no solo el total — dos scores normalizados con coberturas distintas no son directamente comparables.

---

## 12. Bloque complementario — accesibilidad y SEO comercial

Solo si el módulo fue activado. Va al final del informe, con su score en línea propia, nunca sumado al de conversión.

| Parte | Score | Máx |
|---|---:|---:|
| Accesibilidad | | 12 |
| SEO comercial | | 8 |
| **Bloque** | | **20** |

Debajo, los hallazgos separados por parte, con la misma estructura de evidencia y recomendación del bloque 4. Los hallazgos que además afectan la conversión —área táctil, etiquetas de formulario, metadatos sociales, títulos y meta descripciones— van en el cuerpo principal de la auditoría, no aquí: un hallazgo se reporta una sola vez.

Cierra con la nota de alcance del módulo: sin análisis automatizado ni prueba con lector de pantalla, es una revisión de indicios y no un dictamen de conformidad WCAG.

---

## Generación del documento Word

Cuando el informe sea para un cliente, genera el `.docx` con el skill `docx`.

**Nombre:** `Auditoria-Web-[Cliente]-[YYYY-MM-DD].docx`

**Estructura del documento:**

1. Portada con nombre del cliente, URL auditada, fecha y autor, más una línea con score normalizado, estado y cobertura ("61/100 — Regular · Cobertura 84 %").
2. Ficha técnica (bloque 1).
3. Veredicto ejecutivo (bloque 2).
4. Tabla de puntuación (bloque 3).
5. Fugas principales (bloque 4).
6. Escenario económico (bloque 4b), si aplica.
7. Auditoría página por página (bloque 5).
8. Embudo (bloque 6).
9. Benchmark (bloque 7), si aplica.
10. Mejoras de contenido, incluido el antes/después del bloque superior (bloque 8).
11. Plan de acción (bloque 9).
12. Hipótesis (bloque 10).
13. Seguimiento y re-auditoría (bloque 11).
14. Bloque complementario de accesibilidad y SEO comercial (bloque 12), si fue activado.
15. Nota de alcance: qué se evaluó, qué no y por qué.

**Criterios de formato:**

- Tabla de contenido al inicio si el documento supera seis páginas.
- Encabezados jerárquicos reales, no texto en negrita.
- Las citas textuales del sitio van entrecomilladas y en cursiva, para que se distingan de la redacción del informe.
- **Incrusta las capturas del Paso 0** como figura junto a la fuga o hallazgo que sustentan, con pie "Evidencia — [URL], [fecha], [fuente: cliente/navegador]" y referencia desde la fila "Qué observé" del bloque 4. Si llegaron pegadas en el chat sin archivo incrustable, pide el archivo antes de generar el Word o registra en la ficha técnica "capturas recibidas, no incrustables". Nunca recrees ni simules una captura.
- **Sombrea la celda de Estado** de la tabla de puntuación según la escala de `rubrica-scoring.md` (Crítico / Débil / Regular / Bueno / Excelente; el skill `docx` soporta sombreado de celdas). Las categorías NE o NA van en gris neutro con la etiqueta "No evaluado", sin sombreado de rango, para no confundir "no visto" con "está mal".
- El veredicto ejecutivo debe poder leerse solo. Muchos clientes no pasan de la segunda página.
- La nota de alcance final no es letra pequeña: es lo que hace defendible el informe.
