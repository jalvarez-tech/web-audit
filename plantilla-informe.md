# Plantilla del informe de auditoría

Usa esta estructura exacta. Los nueve bloques son obligatorios en la versión completa; la versión rápida usa solo los indicados en SKILL.md.

## Contenido

1. [Portada y ficha técnica](#1-portada-y-ficha-técnica)
2. [Veredicto ejecutivo](#2-veredicto-ejecutivo)
3. [Tabla de puntuación](#3-tabla-de-puntuación)
4. [Las 5 fugas principales](#4-las-5-fugas-principales)
5. [Auditoría página por página](#5-auditoría-página-por-página)
6. [Evaluación del embudo](#6-evaluación-del-embudo)
7. [Benchmark competitivo](#7-benchmark-competitivo)
8. [Mejoras de contenido](#8-mejoras-de-contenido)
9. [Plan de acción priorizado](#9-plan-de-acción-priorizado)
10. [Hipótesis de conversión](#10-hipótesis-de-conversión)
11. [Generación del documento Word](#generación-del-documento-word)

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

Si hubo subcriterios NE o NA, agrega una fila debajo:

> Puntos evaluables: 84 de 100. Score normalizado: 61/100. No evaluados: experiencia móvil (sin capturas), velocidad (sin datos de PageSpeed).

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

Cuando propongas un titular, ofrece **dos variantes** con enfoques distintos (por ejemplo, una centrada en el problema y otra en el resultado) para que el cliente elija y para que sirvan como material de prueba A/B.

Las fórmulas están en `formulas-copy.md`.

---

## 9. Plan de acción priorizado

Tres horizontes. Cada tarea en la tabla.

### Primeras 24 horas — cambios de alto impacto y bajo esfuerzo

Normalmente: reescribir el titular, cambiar el texto del CTA, recortar el formulario, activar analítica si falta.

### Próximos 7 días — estructura, contenido y confianza

Normalmente: reordenar la home según el recorrido de referencia, pedir y publicar testimonios con resultado, agregar bloque de proceso y FAQ, corregir la navegación.

### Próximos 30 días — embudo, automatización y medición

Normalmente: crear la oferta intermedia, configurar eventos de conversión, montar la secuencia de seguimiento, iniciar la primera prueba.

| Prioridad | Acción | Página | Impacto | Esfuerzo | Resultado esperado |
|---|---|---|---|---|---|

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

---

## 11. Bloque complementario — accesibilidad y SEO comercial

Solo si el módulo fue activado. Va **después** del plan de acción y con su score en línea propia, nunca sumado al de conversión.

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

1. Portada con nombre del cliente, URL auditada, fecha y autor.
2. Ficha técnica (bloque 1).
3. Veredicto ejecutivo (bloque 2).
4. Tabla de puntuación (bloque 3).
5. Fugas principales (bloque 4).
6. Auditoría página por página (bloque 5).
7. Embudo (bloque 6).
8. Benchmark (bloque 7), si aplica.
9. Mejoras de contenido (bloque 8).
10. Plan de acción (bloque 9).
11. Hipótesis (bloque 10).
12. Bloque complementario de accesibilidad y SEO comercial (bloque 11), si fue activado.
13. Nota de alcance: qué se evaluó, qué no y por qué.

**Criterios de formato:**

- Tabla de contenido al inicio si el documento supera seis páginas.
- Encabezados jerárquicos reales, no texto en negrita.
- Las citas textuales del sitio van entrecomilladas y en cursiva, para que se distingan de la redacción del informe.
- El veredicto ejecutivo debe poder leerse solo. Muchos clientes no pasan de la segunda página.
- La nota de alcance final no es letra pequeña: es lo que hace defendible el informe.
