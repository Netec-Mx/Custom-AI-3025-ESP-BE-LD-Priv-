# Demo: Caso de uso contextualizado para BancoEstado de Chile — el instructor demuestra cómo utilizar Copilot Chat para transformar información laboral en una presentación de PowerPoint, organizando el contenido y generando una primera versión de las diapositivas.

## Metadatos

| Elemento | Valor |
|---|---|
| Duración | 15 minutos |
| Complejidad | Fácil |
| Nivel de Bloom | Aplicar |
| Modalidad | Demostración guiada por el instructor |
| Tecnologías | Microsoft Copilot Chat, Microsoft Word, Microsoft PowerPoint, Microsoft 365 |
| Escenario | Programa de Educación Financiera Digital BancoEstado (ficticio) |

## Descripción General

> ℹ️ **Nota:** Esta práctica es una **Demostración realizada por el instructor**. El instructor ejecutará los pasos y comandos mientras los alumnos observan, toman notas y analizan el procedimiento, en lugar de realizarla individualmente.

En esta demostración, el instructor utiliza Copilot Chat para transformar un documento de contexto laboral ficticio en una propuesta estructurada de presentación ejecutiva. El proceso muestra cómo entregar contexto, definir audiencia y propósito, solicitar un índice de diapositivas, revisar afirmaciones generadas por IA y convertir un esquema validado en una primera versión de PowerPoint.

El resultado será el archivo `Presentacion_Educacion_Financiera_BancoEstado_v1.pptx`, que se conservará como antecedente narrativo para una demostración posterior de análisis de indicadores en Excel.

## Objetivos de aprendizaje

Al finalizar la demostración, los alumnos podrán:

- [ ] Identificar los componentes de un prompt efectivo para crear una presentación con Copilot Chat.
- [ ] Observar cómo se proporciona contexto laboral ficticio y autorizado a Copilot Chat.
- [ ] Reconocer la importancia de revisar afirmaciones, cifras y mensajes antes de utilizarlos en una presentación.
- [ ] Distinguir entre un borrador generado por IA y una presentación validada para uso profesional.
- [ ] Comprender cómo trasladar un esquema validado a una primera versión de diapositivas en PowerPoint.

## Requisitos previos

### Conocimientos

- Familiaridad básica con la navegación de Microsoft 365.
- Conocimientos básicos de Microsoft Word y PowerPoint.
- Comprensión de los conceptos de audiencia, propósito, mensaje clave y estructura de presentación.
- Comprensión de que Copilot puede generar contenido incompleto, impreciso o no respaldado por las fuentes proporcionadas.

### Acceso y archivos requeridos

Antes de iniciar la demostración, el instructor debe confirmar lo siguiente:

- Inicio de sesión con la cuenta de demostración:

  ```text
  instructor.copilotdemo@contoso-bancoestado-demo.onmicrosoft.com
  ```

- Tenant utilizado exclusivamente para la sesión:

  ```text
  contoso-bancoestado-demo.onmicrosoft.com
  ```

- Licencia Básica de Copilot M365 activa y acceso funcional a Copilot Chat.
- Archivo de contexto disponible:

  ```text
  Contexto_Programa_Educacion_Financiera_BancoEstado.docx
  ```

- Directorio local de trabajo:

  ```text
  C:\CopilotM365Labs\BancoEstadoDemo\
  ```

- Biblioteca de documentos de SharePoint:

  ```text
  /sites/CopilotM365Demo/Documentos compartidos/Labs/01_Contexto_BancoEstado/
  ```

- Confirmación de que todo el contenido usado corresponde a un escenario ficticio, anonimizado y apto para demostración.

## Entorno de laboratorio

### Hardware de referencia

| Componente | Requisito de referencia |
|---|---|
| Equipo | Windows 11 Pro, 24H2 |
| Procesador | 2 núcleos o superior |
| Memoria RAM | 8 GB o superior |
| Espacio disponible | 5 GB o superior |
| Resolución de pantalla | Mínimo 1920 x 1080 |
| Conectividad | Internet estable de al menos 10 Mbps de descarga y 5 Mbps de subida |
| Visualización | Proyector o pantalla compartida para los alumnos |

### Software y configuración

| Elemento | Configuración requerida |
|---|---|
| Sistema operativo | Windows 11 Pro 24H2, compilación 10.0.26100.4652 |
| Microsoft 365 Apps | Versión 2502, compilación 16.0.18526.20168 |
| Navegador | Microsoft Edge 140.0.3485.81 o versión compatible |
| Copilot Chat | Microsoft Copilot Chat para Microsoft 365 |
| Fecha de referencia del servicio | 14-09-2026 |
| Idioma de interfaz | Español (Chile) |
| Idioma de revisión | Español (Chile) |
| Zona horaria | America/Santiago |
| Formato de fecha | `dd-MM-aaaa` |

### Preparación local opcional

Si la carpeta local no existe, el instructor puede crearla antes de la demostración. Ejecutar PowerShell como usuario de la sesión:

```powershell
New-Item -ItemType Directory -Force -Path "C:\CopilotM365Labs\BancoEstadoDemo"
```

El archivo fuente puede abrirse desde SharePoint o desde una copia sincronizada/local autorizada. No se deben usar archivos de producción, cuentas personales ni información real de clientes.

## Procedimiento paso a paso

### Paso 1: Confirmar el entorno de demostración y abrir el documento de contexto

**Objetivo:** Mostrar a los alumnos que la preparación, el contexto autorizado y la identidad de la cuenta son controles previos al uso de IA.

**Instrucciones:**

1. El instructor inicia sesión en Microsoft 365 con la cuenta de demostración:

   ```text
   instructor.copilotdemo@contoso-bancoestado-demo.onmicrosoft.com
   ```

2. El instructor confirma visualmente que la sesión pertenece al tenant de demostración `contoso-bancoestado-demo.onmicrosoft.com`.

3. El instructor abre el documento fuente desde la biblioteca de SharePoint:

   ```text
   /sites/CopilotM365Demo/Documentos compartidos/Labs/01_Contexto_BancoEstado/Contexto_Programa_Educacion_Financiera_BancoEstado.docx
   ```

4. El instructor muestra a los alumnos la información disponible en el documento, identificando de forma general:
   - Nombre de la iniciativa ficticia.
   - Propósito del programa.
   - Público objetivo.
   - Avances descritos.
   - Próximos hitos.
   - Mensajes o restricciones relevantes.

5. El instructor explica que el documento es la fuente de verdad para la demostración y que Copilot no debe complementar cifras, resultados, fechas ni compromisos que no aparezcan en el archivo.

6. El instructor recalca que no se copiarán ni pegarán datos reales de clientes, información bancaria confidencial, credenciales, información comercial reservada ni datos personales.

**Resultado esperado:**

- El documento `Contexto_Programa_Educacion_Financiera_BancoEstado.docx` está abierto.
- Los alumnos pueden reconocer que el escenario y la información utilizados son ficticios.
- Se han identificado los elementos que alimentarán el prompt.

**Verificación:**

El instructor pregunta al grupo:

- ¿Cuál es la fuente que respalda el contenido de la presentación?
- ¿Qué tipo de información no se debe entregar a Copilot durante una demostración?
- ¿Qué ocurriría si Copilot genera una cifra que no aparece en el documento fuente?

La respuesta esperada es que el documento fuente respalda el contenido, que se deben excluir datos reales o sensibles, y que cualquier cifra no respaldada debe eliminarse, corregirse o marcarse para validación.

---

### Paso 2: Formular un prompt contextualizado para generar el índice de la presentación

**Objetivo:** Demostrar cómo incluir contexto, audiencia, propósito, estructura, tono, extensión, formato y restricciones en una solicitud a Copilot Chat.

**Instrucciones:**

1. El instructor abre Microsoft Copilot Chat con la cuenta corporativa de demostración.

2. El instructor proporciona a Copilot el contexto del documento. Según las opciones disponibles en la interfaz, puede adjuntar el archivo autorizado desde SharePoint o incorporar un resumen controlado del contenido ficticio.

3. El instructor explica que el prompt no debe limitarse a pedir “crear una presentación”, sino que debe indicar para quién se crea, qué decisión o comprensión se busca y qué formato se necesita.

4. El instructor ingresa un prompt similar al siguiente. Si el contenido del documento difiere, debe adaptar las referencias sin inventar información.

   ```text
   Utiliza exclusivamente la información del documento
   "Contexto_Programa_Educacion_Financiera_BancoEstado.docx", correspondiente a un
   escenario ficticio y de demostración.

   Actúa como apoyo para preparar una presentación ejecutiva interna sobre el
   Programa de Educación Financiera Digital BancoEstado.

   Audiencia: equipo directivo y responsables de seguimiento de una iniciativa
   ficticia. Su tiempo es limitado y requieren una visión clara del propósito,
   avances, riesgos o dependencias descritas y próximos hitos.

   Propósito: informar el estado de la iniciativa y facilitar una conversación
   de seguimiento; no solicitar aprobación de presupuesto ni presentar datos no
   incluidos en la fuente.

   Genera un índice para una presentación de 6 a 8 diapositivas. Para cada
   diapositiva incluye:
   1. Número de diapositiva.
   2. Título ejecutivo.
   3. Objetivo de la diapositiva.
   4. Tres mensajes clave como máximo.
   5. Referencia a la sección o dato del documento que respalda cada mensaje.

   Usa tono institucional, claro, sobrio y orientado a gestión.
   No inventes cifras, fechas, resultados, productos, compromisos ni nombres.
   Cuando una afirmación no esté explícitamente respaldada por el documento,
   escribe: [VALIDAR CON FUENTE].
   Devuelve el resultado en una tabla Markdown.
   ```

5. El instructor espera la respuesta y muestra el índice generado a los alumnos.

6. El instructor destaca los elementos del prompt:
   - **Contexto:** documento fuente y escenario ficticio.
   - **Audiencia:** equipo directivo y responsables de seguimiento.
   - **Propósito:** informar y facilitar seguimiento.
   - **Estructura:** 6 a 8 diapositivas.
   - **Tono:** institucional, claro y sobrio.
   - **Restricciones:** no inventar información.
   - **Formato de salida:** tabla Markdown con referencias.

**Resultado esperado:**

Copilot Chat propone un índice organizado para una presentación, normalmente con temas similares a:

1. Portada y propósito de la actualización.
2. Contexto o desafío abordado.
3. Objetivos del programa.
4. Público objetivo o alcance.
5. Avances informados.
6. Próximos hitos.
7. Riesgos, dependencias o aspectos por validar, si están presentes en la fuente.
8. Cierre y conversación de seguimiento.

La estructura exacta debe depender del documento fuente.

**Verificación:**

El instructor revisa junto con los alumnos:

- Que la propuesta tenga entre 6 y 8 diapositivas.
- Que cada diapositiva responda al propósito de informar a una audiencia ejecutiva.
- Que no existan afirmaciones que aparenten ser hechos sin respaldo visible.
- Que los mensajes sean breves y no reproduzcan párrafos extensos del documento.

---

### Paso 3: Solicitar contenido resumido por diapositiva

**Objetivo:** Mostrar cómo transformar un índice en contenido inicial breve, reutilizable y apropiado para diapositivas.

**Instrucciones:**

1. Sin perder el contexto de la conversación, el instructor solicita desarrollar el índice aprobado como borrador de contenido para diapositivas.

2. El instructor ingresa el siguiente prompt:

   ```text
   A partir del índice anterior y utilizando únicamente el documento fuente,
   desarrolla el contenido inicial de cada diapositiva.

   Para cada diapositiva entrega:
   - Título de máximo 10 palabras.
   - Una frase de mensaje principal.
   - Entre 2 y 4 viñetas breves.
   - Una sugerencia de recurso visual genérico, por ejemplo: línea de tiempo,
     diagrama de proceso, iconos o gráfico, solo si está respaldado por la
     información disponible.
   - Una marca [VALIDAR CON FUENTE] junto a cualquier elemento que no tenga
     evidencia explícita en el documento.

   Mantén un tono institucional para BancoEstado de Chile, evitando lenguaje
   promocional, promesas de impacto, cifras inventadas o términos técnicos
   innecesarios. No incluyas datos personales, información de clientes ni
   información de producción.
   ```

3. El instructor muestra el resultado generado y lee una o dos diapositivas en voz alta.

4. El instructor explica que el contenido es un borrador y que una recomendación visual no equivale a evidencia. Por ejemplo, si Copilot sugiere un gráfico, el instructor debe verificar que existan datos apropiados para construirlo.

5. El instructor pide a los alumnos identificar una diferencia entre:
   - Un mensaje respaldado por el documento.
   - Una interpretación razonable, pero que requiere confirmación.
   - Una afirmación no respaldada que debe eliminarse.

**Resultado esperado:**

- Copilot entrega títulos, mensajes principales y viñetas breves por diapositiva.
- El contenido mantiene una estructura ejecutiva y legible.
- Los elementos sin respaldo se identifican mediante `[VALIDAR CON FUENTE]` o se omiten.

**Verificación:**

El instructor comprueba que:

- Ninguna diapositiva contiene párrafos extensos.
- Las viñetas describen solamente información existente en el documento.
- Los títulos expresan un mensaje y no solo un tema genérico, cuando la fuente lo permite.
- Las sugerencias visuales no inducen a representar datos inexistentes.

---

### Paso 4: Revisar y corregir afirmaciones no respaldadas

**Objetivo:** Demostrar la revisión humana obligatoria antes de utilizar contenido generado por IA en una comunicación de trabajo.

**Instrucciones:**

1. El instructor coloca Word y Copilot Chat en pantalla dividida, o alterna entre ambas aplicaciones para comparar el contenido generado con el documento fuente.

2. El instructor selecciona al menos tres elementos del borrador para revisar:
   - Una cifra, porcentaje, fecha o hito, si aparece.
   - Una afirmación sobre avance, alcance o resultado.
   - Un mensaje de cierre o una conclusión ejecutiva.

3. Para cada elemento, el instructor busca la evidencia directamente en el documento de contexto.

4. Si Copilot incluyó contenido no respaldado, ambiguo o más concluyente que la fuente, el instructor explica la acción correspondiente:
   - Eliminar la afirmación.
   - Reformularla como antecedente pendiente de validación.
   - Reemplazarla por texto respaldado.
   - Pedir a Copilot una versión más conservadora.

5. El instructor demuestra una solicitud de corrección como la siguiente:

   ```text
   Revisa el borrador anterior con un criterio estricto de trazabilidad.
   Elimina o reformula toda afirmación que no pueda respaldarse explícitamente
   en el documento fuente.

   Para cada diapositiva, presenta:
   - Contenido corregido.
   - Lista breve de cambios realizados.
   - Texto que se debe validar manualmente antes de usarlo.

   No agregues información nueva ni completes vacíos con supuestos.
   ```

6. El instructor explica que la validación no consiste únicamente en detectar errores numéricos. También incluye revisar tono, interpretación, omisiones, contexto, destinatarios y posibles implicancias de una afirmación.

**Resultado esperado:**

- Se obtiene una versión más prudente y trazable del contenido.
- Las afirmaciones no respaldadas se eliminan, se reformulan o se marcan para validación.
- Los alumnos observan que la IA acelera el borrador, pero no reemplaza el juicio profesional.

**Verificación:**

El instructor confirma que cada diapositiva responde positivamente a estas preguntas:

| Pregunta de control | Criterio esperado |
|---|---|
| ¿Está respaldada por la fuente? | Sí, o está marcada para validación. |
| ¿Es adecuada para audiencia ejecutiva? | Sí; es breve, relevante y comprensible. |
| ¿Mantiene el tono institucional? | Sí; evita promesas, exageraciones y lenguaje promocional. |
| ¿Protege información sensible? | Sí; usa solo información ficticia y autorizada. |
| ¿Se entiende sin leer el documento completo? | Sí; comunica un mensaje central claro. |

---

### Paso 5: Ajustar el tono institucional y definir el esquema final

**Objetivo:** Mostrar cómo refinar el contenido para una audiencia ejecutiva antes de llevarlo a PowerPoint.

**Instrucciones:**

1. El instructor solicita una última versión del esquema, orientada a ser trasladada a diapositivas.

2. El instructor utiliza un prompt similar al siguiente:

   ```text
   Genera la versión final del esquema para PowerPoint a partir del contenido
   corregido y validado.

   Requisitos:
   - Máximo 7 diapositivas, incluida la portada.
   - Un solo mensaje principal por diapositiva.
   - Títulos ejecutivos, claros y sobrios.
   - Máximo 4 viñetas por diapositiva.
   - Máximo 12 palabras por viñeta cuando sea posible.
   - No incluir cifras, fechas o resultados que no estén explícitamente
     respaldados por el documento.
   - No incluir notas marcadas como [VALIDAR CON FUENTE]; en su lugar,
     proponlas como preguntas para revisión interna al final de la respuesta.

   Devuelve:
   1. Esquema de diapositivas listo para copiar a PowerPoint.
   2. Lista separada de preguntas de validación pendientes.
   ```

3. El instructor revisa la estructura final con el grupo y confirma que existe una narrativa lógica:
   - Contexto y propósito.
   - Objetivos y alcance.
   - Avances.
   - Próximos hitos.
   - Cierre o próximos pasos de seguimiento.

4. El instructor explica que el número de diapositivas puede ajustarse según la información real del documento, pero no se deben agregar secciones solo para “llenar” una presentación.

5. El instructor conserva las preguntas de validación pendientes como notas para revisión posterior, sin incluirlas como afirmaciones en la presentación.

**Resultado esperado:**

- Existe un esquema final de hasta siete diapositivas.
- El lenguaje es institucional y está adaptado a una audiencia con tiempo limitado.
- Las dudas o vacíos de información se separan del contenido que se presentará como hecho.

**Verificación:**

El instructor solicita a los alumnos que indiquen:

- El mensaje principal de la presentación.
- Qué diapositiva comunica los avances.
- Qué información requeriría validación antes de exponerla.
- Si el orden de las diapositivas apoya una conversación ejecutiva.

---

### Paso 6: Crear la primera versión en PowerPoint

**Objetivo:** Demostrar cómo trasladar un esquema validado a una presentación inicial de PowerPoint sin confundir el borrador con un entregable final aprobado.

**Instrucciones:**

1. El instructor abre Microsoft PowerPoint.

2. El instructor crea una presentación en blanco o utiliza una plantilla institucional autorizada para demostración, si está disponible.

3. El instructor crea las diapositivas según el esquema validado en el paso anterior:
   - Una diapositiva de portada.
   - Una diapositiva por cada sección validada.
   - Una diapositiva final de próximos pasos o cierre, según corresponda.

4. Para cada diapositiva, el instructor:
   - Copia el título validado.
   - Incorpora el mensaje principal y las viñetas resumidas.
   - Mantiene texto breve y legible.
   - Usa diseños simples y consistentes.
   - Evita gráficos o visualizaciones si no existen datos fuente apropiados.

5. Si se incorporan elementos visuales, el instructor utiliza recursos genéricos, tales como iconos autorizados, una línea de tiempo sin cifras no validadas o un diagrama de proceso basado en la fuente.

6. El instructor agrega, cuando corresponda, una nota del presentador con preguntas pendientes de validación. Estas notas no deben presentar información no confirmada como un hecho.

7. El instructor guarda el archivo con el nombre requerido:

   ```text
   C:\CopilotM365Labs\BancoEstadoDemo\Presentacion_Educacion_Financiera_BancoEstado_v1.pptx
   ```

   Si la demostración se realiza directamente desde SharePoint, el instructor guarda también una copia en la biblioteca autorizada, manteniendo el mismo nombre de archivo.

**Resultado esperado:**

Se crea una presentación inicial titulada:

```text
Presentacion_Educacion_Financiera_BancoEstado_v1.pptx
```

La presentación contiene una narrativa breve, ordenada y basada en el documento fuente ficticio.

**Verificación:**

El instructor revisa en modo clasificador de diapositivas que:

- La presentación tenga un máximo de siete diapositivas, salvo que el documento fuente justifique otro número.
- Los títulos sean claros y coherentes entre sí.
- Las diapositivas no estén saturadas de texto.
- No existan marcadores `[VALIDAR CON FUENTE]` visibles en el contenido de las diapositivas.
- No se presenten cifras, promesas o resultados sin respaldo.
- El archivo se haya guardado correctamente con el nombre solicitado.

## Validación y pruebas

El instructor realiza una validación final antes de cerrar la demostración. Esta revisión representa el comportamiento esperado antes de compartir una presentación en un contexto laboral.

| Área de validación | Prueba realizada | Resultado esperado |
|---|---|---|
| Trazabilidad | Comparar títulos, viñetas, cifras y fechas con el documento Word. | Todo contenido está respaldado o fue eliminado. |
| Audiencia | Revisar si una persona directiva comprendería la situación en pocos minutos. | Narrativa clara, breve y orientada a seguimiento. |
| Propósito | Confirmar que la presentación informa y facilita conversación de gestión. | No se introducen decisiones, compromisos o solicitudes no definidas. |
| Tono | Revisar expresiones absolutas, promocionales o ambiguas. | Lenguaje institucional, sobrio y preciso. |
| Protección de datos | Verificar que se usaron solo datos ficticios y autorizados. | No hay datos personales, de clientes ni información productiva. |
| Presentación | Revisar ortografía, consistencia visual y densidad de texto. | Diapositivas legibles y listas para una revisión de contenido final. |
| Archivo | Confirmar ubicación y nombre del archivo. | Existe `Presentacion_Educacion_Financiera_BancoEstado_v1.pptx`. |

Como cierre de la validación, el instructor enfatiza que el archivo creado es una **versión 1**. Antes de una distribución formal, debe contar con revisión del responsable funcional, validación de cifras y fechas, y aplicación de las políticas internas correspondientes.

## Solución de problemas

| Problema | Síntomas | Causa probable | Corrección |
|---|---|---|---|
| Copilot Chat no permite acceder o adjuntar el documento de contexto | El archivo no aparece en el selector, Copilot no puede usarlo o la respuesta indica que no tiene acceso al contenido. | El archivo no está en la biblioteca autorizada, la sesión se inició con una cuenta distinta de la demostración o los permisos aún no se han aplicado. | Confirmar que la sesión corresponde a `instructor.copilotdemo@contoso-bancoestado-demo.onmicrosoft.com`, abrir el archivo desde la biblioteca de SharePoint definida y comprobar permisos. Como alternativa controlada para la demo, copiar al prompt solo un resumen ficticio autorizado del documento; no usar archivos de producción ni cuentas personales. |
| El borrador contiene cifras, resultados o afirmaciones que no aparecen en el documento | Copilot propone porcentajes, fechas, impactos o compromisos sin referencia clara a la fuente. | El modelo completó vacíos mediante inferencia o el prompt no estableció restricciones de trazabilidad suficientemente explícitas. | No copiar el contenido directamente a PowerPoint. Comparar cada afirmación con el documento, eliminar o reformular lo no respaldado y reenviar un prompt que exija usar exclusivamente la fuente, marcar vacíos y no completar supuestos. |

## Limpieza

1. El instructor confirma que el archivo generado se conserva como antecedente para la demostración posterior:

   ```text
   C:\CopilotM365Labs\BancoEstadoDemo\Presentacion_Educacion_Financiera_BancoEstado_v1.pptx
   ```

2. El instructor cierra Word, PowerPoint y las pestañas de Copilot Chat que ya no sean necesarias.

3. El instructor verifica que no se hayan descargado, compartido ni copiado archivos fuera del tenant de demostración.

4. El instructor no elimina el archivo de presentación ni el documento fuente, ya que ambos forman parte de la continuidad pedagógica del curso.

5. Al finalizar la sesión, el instructor cierra sesión de Microsoft 365 si el equipo es compartido.

## Resumen

En esta demostración, los alumnos observaron cómo el instructor transformó un documento laboral ficticio en una primera versión de presentación con apoyo de Copilot Chat. El proceso siguió una secuencia controlada: revisar la fuente, formular un prompt con contexto y restricciones, generar un índice, resumir contenido, validar afirmaciones, ajustar el tono y trasladar el esquema validado a PowerPoint.

La idea central es que Copilot acelera la elaboración de un borrador, pero la responsabilidad sobre la exactitud, pertinencia, confidencialidad y calidad del material sigue siendo humana. Una presentación generada con apoyo de IA debe revisarse antes de comunicarla o utilizarla para respaldar decisiones de trabajo.

### Recursos opcionales

- [Copilot en PowerPoint: ayuda y aprendizaje de Microsoft](https://support.microsoft.com/es-es/copilot-powerpoint)
- [Uso de Copilot en Microsoft 365](https://support.microsoft.com/es-es/copilot)
- [IA responsable de Microsoft](https://www.microsoft.com/es-es/ai/responsible-ai)

---

# Demo: Caso de uso contextualizado para BancoEstado de Chile — el instructor demuestra cómo proporcionar a Copilot Chat un archivo de Excel como fuente de información para realizar consultas, identificar datos relevantes y obtener conclusiones a partir de su contenido.

## Metadatos

| Elemento | Valor |
|---|---|
| Duración | 15 minutos |
| Complejidad | Media |
| Nivel de Bloom | Aplicar |
| Modalidad | Demostración dirigida por el instructor |
| Tecnologías | Microsoft Copilot Chat, Microsoft Excel, Microsoft PowerPoint, Microsoft 365 |
| Escenario | Programa ficticio de Educación Financiera Digital BancoEstado |

## Descripción general

> ℹ️ **Nota:** Esta práctica es una **Demostración realizada por el instructor**. El instructor ejecutará los pasos y comandos mientras los alumnos observan, toman notas y analizan el procedimiento, en lugar de realizarla individualmente.

En esta demostración, el instructor utiliza un archivo de Excel ficticio como fuente de información para Copilot Chat. Se realizan consultas progresivas para comprender la estructura del libro, identificar indicadores, comparar los resultados de Q1 y Q2 de 2026, detectar variaciones y preparar mensajes ejecutivos verificables.

El foco no es aceptar automáticamente el texto generado por Copilot, sino mostrar cómo formular solicitudes con contexto y cómo contrastar cada hallazgo contra los datos de origen en Excel antes de incorporarlo a una presentación o a una decisión de trabajo.

## Objetivos de aprendizaje

Al finalizar la demostración, los alumnos podrán:

- [ ] Reconocer cómo el instructor adjunta o referencia un archivo de Excel permitido en Copilot Chat.
- [ ] Identificar preguntas útiles para explorar hojas, columnas, indicadores, tendencias y comparaciones entre períodos.
- [ ] Distinguir entre un dato presente en el archivo, una inferencia razonable y una recomendación generada por IA.
- [ ] Observar la validación de cálculos y conclusiones directamente en Excel antes de reutilizar los resultados.
- [ ] Relacionar los hallazgos de datos con las diapositivas de resultados de `Presentacion_Educacion_Financiera_BancoEstado_v1.pptx`.

## Requisitos previos

### Conocimientos previos

Los alumnos deben haber observado la demostración 01-06-01 y conocer el escenario ficticio del Programa de Educación Financiera Digital BancoEstado. También deben comprender, a nivel básico:

- Hojas, filas, columnas, encabezados y rangos de datos en Excel.
- Filtros, ordenación y lectura de gráficos simples.
- Diferencia entre valores absolutos, porcentajes y variaciones porcentuales.
- Principio de uso responsable: validar toda salida de IA antes de usarla en comunicaciones, decisiones o documentos de trabajo.
- Prohibición de usar datos reales de clientes, colaboradores, productos, transacciones o información regulada durante la demostración.

### Accesos y archivos requeridos

Antes de iniciar, el instructor debe confirmar los siguientes elementos:

- Cuenta de demostración iniciada: `instructor.copilotdemo@contoso-bancoestado-demo.onmicrosoft.com`.
- Tenant exclusivo de demostración: `contoso-bancoestado-demo.onmicrosoft.com`.
- Licencia Básica de Copilot M365 activa y acceso confirmado a Microsoft Copilot Chat.
- Capacidad habilitada por el tenant para adjuntar o referenciar archivos de trabajo autorizados.
- Archivo fuente disponible:

  ```text
  C:\CopilotM365Labs\BancoEstadoDemo\Indicadores_Programa_Educacion_Financiera_Q1_Q2_2026.xlsx
  ```

- Archivo de contexto de la demostración anterior disponible si corresponde:

  ```text
  C:\CopilotM365Labs\BancoEstadoDemo\Contexto_Programa_Educacion_Financiera_BancoEstado.docx
  ```

- Presentación creada o utilizada en la demostración anterior disponible para consulta:

  ```text
  C:\CopilotM365Labs\BancoEstadoDemo\Presentacion_Educacion_Financiera_BancoEstado_v1.pptx
  ```

- Ubicación autorizada en SharePoint, si el flujo de demostración utiliza archivos en línea:

  ```text
  /sites/CopilotM365Demo/Documentos compartidos/Labs/01_Contexto_BancoEstado/
  ```

## Entorno de laboratorio

### Configuración de hardware

| Componente | Configuración mínima para la demostración |
|---|---|
| Equipo del instructor | Windows 11 Pro 24H2, versión 10.0.26100.4652 |
| Procesador | 2 núcleos o superior |
| Memoria | 8 GB de RAM o superior |
| Disco disponible | 5 GB o superior |
| Pantalla | Resolución mínima de 1920 × 1080 |
| Conectividad | 10 Mbps de descarga y 5 Mbps de subida como mínimo |
| Visualización | Proyector o pantalla compartida para que los alumnos observen Copilot Chat y Excel simultáneamente |

### Configuración de software

| Componente | Configuración requerida |
|---|---|
| Sistema operativo | Windows 11 Pro 24H2 |
| Microsoft 365 Apps | Version 2502, Build 16.0.18526.20168 |
| Navegador | Microsoft Edge 140.0.3485.81 o versión aprobada equivalente |
| Copilot | Microsoft Copilot Chat para Microsoft 365, entorno de demostración fijado al 14-09-2026 |
| Idioma de Microsoft 365 | Español (Chile) |
| Idioma de revisión | Español (Chile) |
| Zona horaria | `America/Santiago` |
| Formato de fecha | `dd-MM-aaaa` |

### Preparación técnica del instructor

Antes de proyectar la sesión, el instructor debe abrir el libro de Excel y comprobar que no contiene datos personales, cuentas reales, RUT, correos reales, números de tarjeta, información transaccional ni información interna no autorizada.

El instructor puede ejecutar el siguiente comando en PowerShell para confirmar la existencia del directorio y del archivo fuente:

```powershell
$labPath = "C:\CopilotM365Labs\BancoEstadoDemo"
$excelFile = Join-Path $labPath "Indicadores_Programa_Educacion_Financiera_Q1_Q2_2026.xlsx"

Test-Path $labPath
Test-Path $excelFile
Get-Item $excelFile | Select-Object Name, Length, LastWriteTime
```

El resultado esperado para los dos primeros comandos es `True`. El último comando debe mostrar el nombre del archivo, su tamaño y la fecha de modificación.

> **Recordatorio de seguridad:** use únicamente la cuenta, tenant, archivos y ubicaciones de demostración indicados. No inicie sesión con cuentas personales ni de producción. No copie datos de esta demostración a chats, repositorios, unidades o cuentas no autorizadas.

## Procedimiento paso a paso

### Paso 1. Presentar el propósito, los límites y el criterio de validación

**Objetivo:** Establecer el escenario de negocio ficticio y explicar que Copilot se utiliza como apoyo para explorar datos, no como sustituto de la validación profesional.

**Instrucciones:**

1. El instructor proyecta una diapositiva o explica verbalmente el contexto del Programa de Educación Financiera Digital BancoEstado utilizado en la demostración 01-06-01.
2. El instructor indica que el archivo `Indicadores_Programa_Educacion_Financiera_Q1_Q2_2026.xlsx` contiene indicadores ficticios o anonimizados correspondientes a Q1 y Q2 de 2026.
3. El instructor explica que durante la demostración se responderán cinco tipos de preguntas:
   1. ¿Qué contiene el libro?
   2. ¿Cuáles son los indicadores principales?
   3. ¿Qué cambió entre Q1 y Q2?
   4. ¿Qué segmentos requieren atención?
   5. ¿Qué mensaje ejecutivo puede incorporarse a una presentación?
4. El instructor comunica explícitamente el criterio de calidad que se aplicará a toda respuesta de Copilot:
   - Los **datos presentes** deben poder localizarse en una hoja, tabla, fila, columna o gráfico del libro.
   - Las **inferencias** deben declararse como interpretación y no como hecho absoluto.
   - Las **recomendaciones** deben estar separadas de los datos y requerir revisión humana.
5. El instructor solicita a los alumnos tomar nota de cualquier afirmación que deba verificarse posteriormente en Excel.

**Resultado esperado:**

Los alumnos comprenden que el objetivo es demostrar un proceso de consulta, interpretación y validación. No se espera que los alumnos introduzcan prompts ni modifiquen archivos.

**Verificación:**

El instructor formula una pregunta breve al grupo:

> “Si Copilot afirma que un segmento tiene baja participación, ¿qué debemos revisar antes de comunicarlo como conclusión?”

La respuesta esperada debe mencionar la revisión de la columna, la hoja, el período, el valor y, cuando corresponda, el cálculo utilizado.

---

### Paso 2. Inspeccionar el libro de Excel antes de consultar a Copilot

**Objetivo:** Mostrar que la calidad del análisis depende de una fuente estructurada, comprensible y revisada antes de utilizar IA.

**Instrucciones:**

1. El instructor abre en Excel el archivo:

   ```text
   C:\CopilotM365Labs\BancoEstadoDemo\Indicadores_Programa_Educacion_Financiera_Q1_Q2_2026.xlsx
   ```

2. El instructor muestra las pestañas de las hojas sin asumir que su contenido puede ser interpretado solo por el nombre.
3. Para cada hoja relevante, el instructor revisa visualmente:
   - El nombre de la hoja.
   - Los encabezados de columna.
   - La presencia de valores numéricos y porcentajes.
   - La existencia de períodos comparables, en particular Q1 y Q2 de 2026.
   - La presencia de categorías o segmentos que permitan comparar participación, cobertura, finalización u otros indicadores.
4. El instructor confirma que los encabezados son claros y que no existen filas de título dentro del rango que puedan confundir un análisis.
5. Si los datos están organizados como tabla de Excel, el instructor selecciona una celda de la tabla y señala que las tablas facilitan filtros, referencias y revisión. Si no están organizados como tabla, el instructor no modifica la estructura durante esta demo, pero destaca que una tabla bien definida mejora la confiabilidad del análisis posterior.
6. El instructor identifica, sin todavía calcular conclusiones, las columnas que probablemente serán relevantes para la comparación, por ejemplo:
   - Período o trimestre.
   - Segmento, región, canal o público objetivo.
   - Participantes, inscripciones, sesiones o alcance.
   - Tasa de finalización, satisfacción, adopción u otro indicador porcentual.
   - Metas o resultados esperados, si existen.
7. El instructor explica que una solicitud ambigua como “analiza los datos” genera resultados difíciles de validar. En cambio, una solicitud con período, indicador, dimensión de comparación y formato de salida permite una revisión objetiva.

**Resultado esperado:**

El libro queda abierto en Excel y los alumnos visualizan una fuente de datos con hojas y encabezados identificables. Se han reconocido posibles campos para comparar Q1 con Q2 sin emitir aún conclusiones.

**Verificación:**

El instructor pide a los alumnos identificar, mirando el libro proyectado:

- Una columna que represente un indicador.
- Una columna que permita segmentar o comparar.
- Una columna o valor que permita diferenciar Q1 y Q2.

El instructor confirma las respuestas directamente en el archivo, no mediante una respuesta de Copilot.

---

### Paso 3. Adjuntar el libro en Copilot Chat y solicitar una descripción verificable

**Objetivo:** Demostrar cómo proporcionar el archivo autorizado a Copilot Chat y solicitar una descripción estructurada de su contenido.

**Instrucciones:**

1. El instructor abre Microsoft Copilot Chat desde Microsoft 365 o desde el acceso corporativo autorizado.
2. El instructor verifica visualmente que ha iniciado sesión con:

   ```text
   instructor.copilotdemo@contoso-bancoestado-demo.onmicrosoft.com
   ```

3. El instructor confirma que el contexto corresponde al tenant de demostración `contoso-bancoestado-demo.onmicrosoft.com`.
4. En un chat nuevo, el instructor usa la opción de adjuntar archivo o la opción autorizada para referenciar el archivo desde OneDrive o SharePoint.
5. El instructor adjunta o selecciona el archivo:

   ```text
   Indicadores_Programa_Educacion_Financiera_Q1_Q2_2026.xlsx
   ```

6. El instructor espera a que la interfaz confirme que el archivo está adjunto antes de enviar la consulta.
7. El instructor introduce el siguiente prompt, adaptándolo solo si la interfaz solicita una referencia explícita al archivo adjunto:

   ```text
   Actúa como analista de datos para un programa ficticio de educación financiera digital de BancoEstado de Chile.

   Usa exclusivamente el archivo Excel adjunto como fuente. No inventes cifras, hojas, columnas ni definiciones.

   1. Enumera las hojas disponibles.
   2. Para cada hoja, describe brevemente su propósito según sus encabezados y datos.
   3. Identifica las columnas principales, incluyendo período, indicadores y dimensiones de segmentación.
   4. Indica qué hojas y columnas parecen útiles para comparar Q1 y Q2 de 2026.

   Devuelve el resultado en una tabla con las columnas: Hoja, propósito observado, columnas relevantes y posible uso analítico.
   Si algo no está disponible o no es claro, indícalo explícitamente como "No identificado en el archivo".
   ```

8. El instructor lee la respuesta en voz alta y destaca si Copilot:
   - Identifica hojas existentes.
   - Utiliza nombres de columnas coherentes con el libro.
   - Distingue observaciones verificables de supuestos.
   - Declara limitaciones cuando no puede identificar un elemento.
9. Si Copilot menciona una hoja o columna inesperada, el instructor no la acepta de inmediato: vuelve a Excel y confirma si realmente existe.

**Resultado esperado:**

Copilot genera una descripción tabular de las hojas y columnas relevantes del archivo adjunto. La respuesta debe servir como mapa inicial del libro, no como conclusión de negocio.

**Verificación:**

El instructor compara al menos dos elementos de la respuesta de Copilot contra Excel:

1. Un nombre de hoja.
2. Un encabezado de columna relevante.

Si ambos elementos coinciden, el instructor explica que la respuesta es parcialmente validada. Si hay discrepancias, el instructor señala que debe corregirse o descartarse antes de continuar.

---

### Paso 4. Identificar indicadores principales y comparar Q1 con Q2

**Objetivo:** Demostrar una consulta específica que solicite comparaciones verificables, diferencias absolutas y variaciones porcentuales sin confundir los conceptos.

**Instrucciones:**

1. El instructor conserva el mismo chat para mantener el contexto del archivo adjunto.
2. El instructor explica la diferencia entre:
   - **Diferencia absoluta:** resta entre dos valores, por ejemplo, `Q2 - Q1`.
   - **Variación porcentual:** cambio relativo respecto de Q1, calculado como `(Q2 - Q1) / Q1`.
   - **Puntos porcentuales:** diferencia entre dos tasas expresadas en porcentaje, por ejemplo, pasar de 60 % a 65 % equivale a 5 puntos porcentuales.
3. El instructor envía el siguiente prompt:

   ```text
   A partir del archivo Excel adjunto, identifica los indicadores principales disponibles para evaluar el Programa de Educación Financiera Digital.

   Compara Q1 y Q2 de 2026 para cada indicador que tenga datos comparables.

   Para cada comparación, entrega:
   - nombre exacto del indicador;
   - valor de Q1;
   - valor de Q2;
   - diferencia absoluta;
   - variación porcentual, cuando sea matemáticamente aplicable;
   - hoja, tabla o sección de origen;
   - una interpretación breve y prudente.

   Separa con claridad los datos observados de la interpretación. No completes valores faltantes ni infieras datos que no estén en el archivo.
   Ordena las comparaciones desde la mayor variación negativa a la mayor variación positiva.
   ```

4. El instructor revisa la salida y selecciona uno o dos indicadores relevantes para validación manual.
5. El instructor vuelve a Excel y localiza los valores de Q1 y Q2 informados por Copilot.
6. En una celda vacía, hoja auxiliar autorizada o cálculo temporal, el instructor demuestra la fórmula de variación porcentual. Como ejemplo genérico, si Q1 está en `B2` y Q2 en `C2`, utiliza:

   ```excel
   =(C2-B2)/B2
   ```

7. El instructor aplica formato de porcentaje a la celda si corresponde.
8. Cuando el indicador sea una tasa porcentual, el instructor demuestra el cálculo de puntos porcentuales:

   ```excel
   =C2-B2
   ```

9. El instructor aclara al grupo que no se deben etiquetar automáticamente todos los cambios de tasas como “variación porcentual”; en comunicaciones ejecutivas suele ser más claro reportar puntos porcentuales cuando se comparan porcentajes.

**Resultado esperado:**

Copilot presenta una comparación estructurada entre Q1 y Q2 usando los indicadores disponibles. El instructor valida uno o dos cálculos directamente en Excel y determina si la interpretación de Copilot es consistente con los datos.

**Verificación:**

La verificación se considera satisfactoria cuando:

- Los valores de Q1 y Q2 indicados por Copilot coinciden con el libro.
- La diferencia absoluta coincide con la resta realizada en Excel.
- La variación porcentual o los puntos porcentuales están correctamente calculados y etiquetados.
- La fuente indicada por Copilot puede asociarse a una hoja, tabla o sección existente.

> **Punto de enseñanza:** un cálculo correcto no garantiza una conclusión correcta. El instructor debe revisar si se están comparando períodos equivalentes, segmentos equivalentes y unidades compatibles.

---

### Paso 5. Detectar variaciones relevantes y segmentos con menor participación

**Objetivo:** Mostrar cómo formular una consulta analítica con criterios explícitos y cómo evitar que Copilot transforme una correlación o diferencia numérica en una causa no demostrada.

**Instrucciones:**

1. El instructor explica que expresiones como “variación relevante” o “baja participación” necesitan una definición en el prompt.
2. El instructor pide a Copilot revisar las variaciones y los segmentos, usando una solicitud que obligue a explicitar criterios y fuentes:

   ```text
   Analiza el archivo Excel adjunto para identificar variaciones relevantes entre Q1 y Q2 de 2026 y segmentos con menor participación.

   Aplica estos criterios:
   - considera una variación relevante cuando exista una disminución o aumento destacado respecto de los demás registros comparables del mismo indicador;
   - identifica los segmentos ubicados en el nivel más bajo de participación, alcance, inscripción o finalización, según las métricas disponibles;
   - compara solo registros equivalentes en período, métrica y unidad de medida.

   Entrega tres secciones:

   1. Datos observados:
      - indicador o segmento;
      - valor Q1;
      - valor Q2;
      - cambio calculado;
      - fuente en el archivo.

   2. Inferencias prudentes:
      - posibles interpretaciones limitadas a lo que los datos permiten observar;
      - usa lenguaje como "podría indicar", "requiere revisión" o "se observa una asociación".

   3. Preguntas de validación:
      - información adicional necesaria antes de atribuir causas o tomar decisiones.

   No atribuyas causas, como problemas de comunicación, conectividad, contenido o canal, a menos que el archivo contenga evidencia explícita.
   ```

3. El instructor lee una o dos observaciones de la sección “Datos observados”.
4. El instructor lee una inferencia y destaca el uso de lenguaje prudente. Si Copilot presenta una causa como certeza sin evidencia, el instructor señala que esa afirmación no debe usarse.
5. El instructor vuelve a Excel y utiliza filtros para revisar el segmento identificado con menor participación:
   - Selecciona la columna de segmento, región, canal o grupo disponible.
   - Aplica filtro u ordenación ascendente sobre la métrica de participación pertinente.
   - Confirma que el registro señalado por Copilot está efectivamente entre los valores más bajos bajo los criterios comparables.
6. El instructor revisa que la comparación no mezcle indicadores distintos, por ejemplo, participantes con porcentajes de finalización, ni períodos no equivalentes.
7. Si el archivo incluye gráficos, el instructor muestra cómo utilizar el gráfico solo como apoyo visual y no como sustituto de la lectura de los valores subyacentes.

**Resultado esperado:**

Copilot diferencia datos, inferencias y preguntas de validación. Se identifica al menos un segmento o indicador que merece seguimiento, sin declarar una causa no respaldada por la fuente.

**Verificación:**

El instructor debe poder responder “sí” a estas preguntas:

- ¿El segmento señalado existe en el archivo?
- ¿La métrica usada para calificarlo como de baja participación está claramente identificada?
- ¿Se comparó con registros equivalentes?
- ¿La afirmación de causa fue evitada o respaldada por evidencia explícita?
- ¿La observación puede localizarse mediante un filtro o una ordenación en Excel?

---

### Paso 6. Generar una síntesis ejecutiva para la presentación y validarla

**Objetivo:** Transformar hallazgos validados en contenido breve para diapositivas, manteniendo trazabilidad hacia los datos y separando recomendaciones de resultados.

**Instrucciones:**

1. El instructor abre o deja visible la presentación creada en la demostración anterior:

   ```text
   Presentacion_Educacion_Financiera_BancoEstado_v1.pptx
   ```

2. El instructor identifica la diapositiva de resultados, avances, indicadores o próximos pasos donde podría incorporarse una síntesis.
3. El instructor indica que no copiará automáticamente el contenido generado por Copilot. Primero solicitará un borrador con restricciones específicas.
4. El instructor envía el siguiente prompt en Copilot Chat:

   ```text
   Con base exclusivamente en los hallazgos del archivo Excel adjunto que hayan sido identificados y validados, redacta una síntesis para incorporar en una diapositiva de resultados de Presentacion_Educacion_Financiera_BancoEstado_v1.pptx.

   Audiencia: equipo ejecutivo interno del escenario ficticio BancoEstado.
   Objetivo: comunicar resultados de Q1 y Q2 de 2026 de forma clara, prudente y accionable.
   Formato:
   - título de máximo 10 palabras;
   - 3 viñetas de resultados observados, cada una de máximo 20 palabras;
   - 1 viñeta separada de "Implicancia a revisar", redactada como recomendación y no como hecho;
   - nota de fuente al final: "Fuente: Indicadores_Programa_Educacion_Financiera_Q1_Q2_2026.xlsx".

   Reglas:
   - conserva las cifras y unidades verificadas;
   - no inventes metas, causas ni impactos;
   - distingue resultados observados de la recomendación;
   - si un dato no fue validado, reemplázalo por "[Validar en Excel]".
   ```

5. El instructor revisa el texto generado y compara las cifras con las anotaciones o cálculos validados en los pasos anteriores.
6. El instructor ajusta manualmente el lenguaje de ser necesario para:
   - Eliminar afirmaciones absolutas no respaldadas.
   - Corregir unidades, porcentajes o períodos.
   - Hacer explícita la fuente.
   - Mantener el carácter ficticio del escenario.
7. El instructor muestra cómo el contenido podría incorporarse en la diapositiva como borrador, sin necesidad de modificar la presentación durante la demostración si el tiempo es limitado.
8. El instructor explica que, antes de distribuir una presentación real, el responsable del documento debe aplicar los controles internos, de marca, de calidad, de privacidad y de aprobación correspondientes.

**Resultado esperado:**

Se obtiene un borrador de contenido ejecutivo breve, trazable al archivo Excel y adecuado para revisión humana antes de usarlo en la presentación.

**Verificación:**

El instructor verifica que el borrador cumple las siguientes condiciones:

| Criterio | Resultado esperado |
|---|---|
| Título | Tiene un máximo de 10 palabras y describe el contenido sin exagerar conclusiones. |
| Viñetas de resultados | Contienen cifras o hallazgos que pueden validarse en Excel. |
| Recomendación | Está separada de los resultados y usa un lenguaje de revisión o acción propuesta. |
| Fuente | Menciona el archivo Excel exacto. |
| Riesgo de invención | No incluye metas, causas, segmentos o valores inexistentes. |

## Validación y pruebas

El instructor debe completar las siguientes pruebas durante o inmediatamente después de la demostración. Estas pruebas sirven para demostrar que la salida de Copilot fue evaluada y no utilizada de manera automática.

### Prueba 1. Validación de estructura del archivo

1. Compare los nombres de hojas mencionados por Copilot con las pestañas visibles en Excel.
2. Compare al menos dos nombres de columnas mencionados por Copilot con los encabezados reales.
3. Confirme que Copilot no haya atribuido al archivo una hoja, métrica o dimensión inexistente.

**Criterio de aprobación:** todos los elementos comprobados coinciden con el libro o han sido corregidos explícitamente.

### Prueba 2. Validación de un cálculo comparativo

1. Seleccione un indicador comparado entre Q1 y Q2.
2. Identifique los valores fuente en Excel.
3. Calcule la diferencia absoluta.
4. Calcule la variación porcentual o la diferencia en puntos porcentuales según la naturaleza del indicador.
5. Compare el resultado con el valor entregado por Copilot.

**Criterio de aprobación:** el cálculo de Copilot coincide con Excel o se corrige antes de usarlo.

### Prueba 3. Validación de segmento de menor participación

1. Aplique un filtro u ordenación a la métrica utilizada.
2. Compruebe que el segmento señalado por Copilot se encuentre efectivamente entre los registros de menor valor comparables.
3. Verifique que no existan filtros ocultos, categorías excluidas o períodos mezclados que invaliden la comparación.

**Criterio de aprobación:** el hallazgo puede reproducirse directamente desde el archivo.

### Prueba 4. Validación del lenguaje ejecutivo

Revise la síntesis propuesta por Copilot y clasifique cada afirmación:

| Tipo de afirmación | Tratamiento requerido |
|---|---|
| Dato presente | Confirmar valor, período, unidad y fuente. |
| Inferencia | Mantener lenguaje prudente y confirmar que se deriva razonablemente de los datos. |
| Recomendación | Presentarla como propuesta sujeta a revisión, no como conclusión factual. |
| Causa atribuida | Eliminarla o exigir evidencia explícita en el archivo. |

**Criterio de aprobación:** la diapositiva propuesta no presenta inferencias o recomendaciones como si fueran datos comprobados.

## Solución de problemas

### Problema 1. Copilot Chat no permite adjuntar el archivo o no reconoce el libro como fuente

**Síntomas:**

- No aparece la opción para adjuntar archivos.
- El archivo no puede seleccionarse.
- Copilot responde que no puede acceder al contenido del libro.
- La respuesta parece genérica y no menciona hojas ni columnas reales.

**Causa probable:**

La sesión puede estar iniciada con una cuenta incorrecta, la licencia o capacidad de adjuntar archivos puede no estar habilitada, el archivo puede no estar en una ubicación autorizada o la carga puede no haberse completado.

**Solución:**

1. Confirme que la sesión utiliza `instructor.copilotdemo@contoso-bancoestado-demo.onmicrosoft.com`.
2. Confirme que el tenant visible corresponde a `contoso-bancoestado-demo.onmicrosoft.com`.
3. Verifique que el archivo existe en `C:\CopilotM365Labs\BancoEstadoDemo\`.
4. Si la política requiere una ubicación en la nube, cargue o seleccione el archivo desde la biblioteca autorizada de SharePoint:
   ```text
   /sites/CopilotM365Demo/Documentos compartidos/Labs/01_Contexto_BancoEstado/
   ```
5. Espere la confirmación visual de archivo adjunto antes de enviar el prompt.
6. Si el problema persiste, no use cuentas personales ni alternativas no autorizadas; registre el incidente y solicite revisión de licencia, permisos o políticas del tenant de demostración.

### Problema 2. Copilot entrega cifras, comparaciones o conclusiones que no coinciden con Excel

**Síntomas:**

- Los valores de Q1 o Q2 no se encuentran en la hoja indicada.
- Copilot mezcla porcentajes con cantidades.
- La variación porcentual no coincide con el cálculo manual.
- La respuesta atribuye causas que no aparecen en el archivo.

**Causa probable:**

La solicitud fue demasiado amplia, el libro contiene varias hojas o tablas con métricas similares, existen formatos de datos ambiguos o Copilot realizó una inferencia no sustentada.

**Solución:**

1. No copie la respuesta a la presentación ni la comunique como conclusión.
2. Regrese a Excel e identifique la hoja, tabla, encabezados, período y unidad correctos.
3. Reformule el prompt con restricciones, por ejemplo:
   ```text
   Usa solo la hoja [nombre real de la hoja] y las columnas [nombres reales].
   Compara exclusivamente Q1 y Q2 de 2026.
   Muestra los valores de origen antes de calcular diferencias.
   Si no puedes confirmar un valor, responde "No validado".
   ```
4. Calcule nuevamente la diferencia en Excel y determine si corresponde informar porcentaje relativo o puntos porcentuales.
5. Elimine o reformule cualquier causa no respaldada como una pregunta de investigación o recomendación sujeta a validación.

## Limpieza

Al finalizar la demostración, el instructor debe realizar las siguientes acciones:

1. Cerrar el libro de Excel sin modificar ni sobrescribir el archivo fuente original, salvo que exista una copia de trabajo autorizada.
2. Cerrar la presentación o guardar solo cambios intencionales y revisados en una copia autorizada.
3. Cerrar Copilot Chat o iniciar un chat nuevo para evitar que un usuario posterior continúe utilizando el contexto del archivo adjunto.
4. No descargar, reenviar ni compartir el archivo de demostración fuera del tenant `contoso-bancoestado-demo.onmicrosoft.com`.
5. Confirmar que no se hayan utilizado cuentas personales, cuentas de producción ni datos reales durante la sesión.
6. Mantener los archivos fuente en la ruta local y/o biblioteca de SharePoint autorizada conforme a las políticas del entorno de demostración.

## Resumen

En esta demostración, el instructor mostró un flujo de trabajo responsable para utilizar Copilot Chat con un archivo de Excel: inspeccionar la fuente, adjuntarla en un entorno autorizado, formular consultas progresivas, solicitar comparaciones estructuradas y validar los resultados directamente en Excel.

Los mensajes principales para los alumnos son:

- Una buena consulta especifica contexto, objetivo, período, indicadores, audiencia, formato y restricciones.
- Copilot puede acelerar la exploración y redacción, pero no reemplaza la comprobación de los datos de origen.
- Las respuestas deben distinguir claramente entre datos observados, inferencias y recomendaciones.
- Los resultados destinados a una presentación ejecutiva deben conservar trazabilidad hacia la fuente, incluir el período correcto y pasar por revisión humana.
- En un contexto bancario, incluso durante una demostración, solo deben utilizarse datos ficticios o anonimizados y entornos corporativos autorizados.

### Recursos opcionales

- [Copilot en Excel: ayuda y aprendizaje de Microsoft](https://support.microsoft.com/es-es/copilot-excel)
- [Introducción a Copilot para Microsoft 365](https://learn.microsoft.com/es-es/copilot/microsoft-365/)
- [Crear y dar formato a tablas en Excel](https://support.microsoft.com/es-es/office/crear-y-dar-formato-a-tablas-8d5b6c92-ae97-4b20-9b6c-1c5c69e7d0e1)
- [Microsoft Trust Center: seguridad, privacidad y cumplimiento](https://www.microsoft.com/es-es/trust-center)

---

# Demo: El instructor demuestra cómo utilizar Copilot Chat para transformar la información de una reunión en una minuta estructurada, identificando los temas principales, acuerdos, decisiones y próximos pasos.

## Metadatos

| Elemento | Valor |
|---|---|
| Duración | 10 minutos |
| Complejidad | Fácil |
| Nivel de Bloom | Aplicar |
| Modalidad | Demostración dirigida por el instructor |
| Tecnologías | Microsoft Copilot Chat, Microsoft Word, Microsoft 365 |

## Descripción general

> ℹ️ **Nota:** Esta práctica es una **Demostración realizada por el instructor**. El instructor ejecutará los pasos y comandos mientras los alumnos observan, toman notas y analizan el procedimiento, en lugar de realizarla individualmente.

En esta demostración, el instructor utilizará Copilot Chat para convertir notas desestructuradas de una reunión ficticia del Programa de Educación Financiera BancoEstado en un borrador de minuta profesional. La demostración cierra el escenario trabajado en las demostraciones anteriores, relacionando la revisión de la presentación y los resultados de indicadores con acuerdos, decisiones y actividades de seguimiento.

El énfasis no está solo en generar contenido: el instructor mostrará cómo solicitar una estructura clara, cómo detectar posibles invenciones de la IA y cómo validar participantes, responsables, fechas y decisiones antes de distribuir una minuta.

## Objetivos de aprendizaje

Al finalizar la demostración, los alumnos podrán:

- [ ] Reconocer cómo Copilot Chat puede transformar notas de reunión en un borrador estructurado de minuta.
- [ ] Identificar los elementos esenciales de una minuta: asistentes, objetivo, temas, decisiones, acuerdos, responsables, fechas, riesgos y próximos pasos.
- [ ] Observar cómo formular un prompt con contexto, objetivo, formato de salida y restricciones explícitas.
- [ ] Comprender por qué deben validarse los datos generados por IA antes de comunicar o distribuir una minuta.
- [ ] Relacionar los acuerdos de la reunión con la presentación y el análisis de indicadores revisados en demostraciones anteriores.

## Requisitos previos

### Conocimientos previos

Antes de realizar la demostración, los alumnos deben haber observado:

- La demostración **01-06-01**, relacionada con la generación o revisión de una presentación del Programa de Educación Financiera.
- La demostración **01-08-01**, relacionada con el análisis de indicadores del programa.
- La estructura básica de una minuta profesional de reunión.
- El principio de uso responsable de IA: validar siempre el contenido generado antes de usarlo para tomar decisiones o comunicar información laboral.

### Acceso y archivos requeridos

El instructor debe confirmar, antes de iniciar la sesión, lo siguiente:

- Acceso a Microsoft 365 mediante la cuenta de demostración:

  ```text
  instructor.copilotdemo@contoso-bancoestado-demo.onmicrosoft.com
  ```

- Uso exclusivo del tenant de demostración:

  ```text
  contoso-bancoestado-demo.onmicrosoft.com
  ```

- Licencia Básica de Copilot M365 activa y acceso funcional a Copilot Chat.
- Interfaz de Microsoft 365 configurada en **español (Chile)**.
- Idioma de revisión configurado en **español (Chile)**.
- Zona horaria configurada como **America/Santiago**.
- Formato de fecha configurado como **dd-MM-aaaa**.
- Disponibilidad del archivo fuente:

  ```text
  C:\CopilotM365Labs\BancoEstadoDemo\Notas_Reunion_Seguimiento_Programa_Educacion_Financiera_2026-09-14.docx
  ```

- Disponibilidad del directorio local de trabajo:

  ```text
  C:\CopilotM365Labs\BancoEstadoDemo\
  ```

- Acceso, si corresponde a la configuración del entorno, a la biblioteca de SharePoint de demostración:

  ```text
  /sites/CopilotM365Demo/Documentos compartidos/Labs/01_Contexto_BancoEstado/
  ```

> **Importante:** El instructor no debe utilizar cuentas personales, cuentas de producción ni información real de clientes, colaboradores, operaciones bancarias o datos personales. Esta demostración utiliza exclusivamente información ficticia o anonimizada.

## Entorno de laboratorio

### Hardware de referencia

| Componente | Requisito de referencia |
|---|---|
| Sistema operativo | Windows 11 Pro 24H2, compilación 10.0.26100.4652 |
| Procesador | 2 núcleos o superior |
| Memoria RAM | 8 GB como mínimo |
| Espacio libre | 5 GB como mínimo |
| Resolución de pantalla | 1920 × 1080 píxeles como mínimo |
| Conectividad | 10 Mbps de descarga y 5 Mbps de subida como mínimo |
| Visualización | Proyector o pantalla compartida para la demostración |

### Software de referencia

| Software | Versión o configuración |
|---|---|
| Microsoft 365 Apps for enterprise | Versión 2502, compilación 16.0.18526.20168 |
| Microsoft Edge | Versión 140.0.3485.81 |
| Microsoft Copilot Chat para Microsoft 365 | Servicio SaaS; demostración fijada al 14-09-2026 |
| Microsoft Word | Aplicación de escritorio de Microsoft 365 |
| Idioma de interfaz | Español (Chile) |

### Preparación técnica del instructor

Antes de compartir pantalla, el instructor puede comprobar que existen la carpeta de trabajo y el archivo fuente mediante PowerShell:

```powershell
Test-Path "C:\CopilotM365Labs\BancoEstadoDemo\"
Test-Path "C:\CopilotM365Labs\BancoEstadoDemo\Notas_Reunion_Seguimiento_Programa_Educacion_Financiera_2026-09-14.docx"
```

El resultado esperado para ambos comandos es:

```text
True
```

Si el archivo fuente se encuentra inicialmente en la biblioteca de SharePoint de demostración, el instructor debe abrirlo desde SharePoint y guardarlo o sincronizarlo en la carpeta local de trabajo autorizada antes de comenzar la demostración.

> **Punto de control para el instructor:** Antes de proyectar Copilot Chat, confirme que está conectado con la cuenta de demostración corporativa y no con una identidad personal o de producción.

## Procedimiento paso a paso

### Paso 1: Presentar el escenario y abrir las notas de reunión

**Objetivo:** Mostrar a los alumnos la información de entrada desestructurada y establecer el contexto de la minuta que se generará.

**Instrucciones:**

1. El instructor explica que la reunión ficticia corresponde al seguimiento del **Programa de Educación Financiera BancoEstado**.
2. El instructor recuerda brevemente que el escenario incorpora:
   - La presentación revisada en la demostración 01-06-01.
   - Los resultados e indicadores analizados en la demostración 01-08-01.
   - Las decisiones y actividades de seguimiento registradas en las notas de la reunión.
3. El instructor abre Microsoft Word.
4. En Word, el instructor abre el archivo:

   ```text
   C:\CopilotM365Labs\BancoEstadoDemo\Notas_Reunion_Seguimiento_Programa_Educacion_Financiera_2026-09-14.docx
   ```

5. El instructor comparte la ventana de Word y permite que los alumnos observen que las notas son información de trabajo no necesariamente organizada como minuta.
6. Sin leer ni interpretar información fuera de lo registrado, el instructor identifica visualmente ejemplos de contenido que normalmente debe convertirse en secciones formales:
   - Referencias a asistentes o participantes.
   - Comentarios sobre la presentación.
   - Resultados de indicadores.
   - Decisiones acordadas.
   - Actividades pendientes.
   - Posibles responsables.
   - Fechas o plazos mencionados.
   - Riesgos o dependencias.

7. El instructor recalca a los alumnos que una nota, comentario o propuesta no necesariamente equivale a una decisión aprobada o a un compromiso definitivo.

**Resultado esperado:**

El archivo de notas queda abierto en Word y los alumnos comprenden que será la única fuente de información para el borrador de minuta.

**Verificación:**

El instructor confirma visualmente que:

- El nombre del archivo abierto corresponde a `Notas_Reunion_Seguimiento_Programa_Educacion_Financiera_2026-09-14.docx`.
- La fecha de referencia de la reunión es **14-09-2026**.
- El contenido mostrado pertenece al escenario ficticio de demostración.
- No se muestran datos de producción, datos personales no autorizados ni información de clientes reales.

---

### Paso 2: Explicar los criterios de una minuta y las restricciones para Copilot Chat

**Objetivo:** Preparar un prompt que incluya contexto, objetivo, audiencia, formato requerido y restricciones de validación.

**Instrucciones:**

1. El instructor indica que Copilot Chat puede crear un borrador inicial, pero no reemplaza la revisión de quien participó en la reunión o conoce el contexto.
2. El instructor explica que la minuta debe separar claramente:
   - Fecha.
   - Asistentes.
   - Objetivo de la reunión.
   - Temas principales.
   - Resumen de discusión.
   - Decisiones.
   - Acuerdos.
   - Responsables.
   - Fechas comprometidas.
   - Riesgos.
   - Próximos pasos.
3. El instructor destaca las siguientes restricciones que incluirá en la solicitud:
   - Usar solamente la información presente en el documento fuente.
   - No inventar asistentes, cargos, responsables, decisiones, acuerdos, fechas ni compromisos.
   - Marcar como **“No especificado en las notas”** cualquier dato requerido que no esté explícitamente indicado.
   - Diferenciar una propuesta, comentario o tema de discusión de una decisión formal.
   - Mantener un tono profesional, claro y apto para circulación interna.
4. El instructor pregunta a los alumnos qué errores podrían ser graves en una minuta generada por IA. Se espera que identifiquen, entre otros:
   - Asignar una tarea a una persona incorrecta.
   - Transformar una propuesta en una decisión.
   - Agregar una fecha límite inexistente.
   - Omitir un riesgo mencionado.
   - Atribuir asistencia a una persona que no participó.
5. El instructor refuerza que, en un contexto bancario, una minuta no debe ser distribuida hasta que se validen los elementos que afectan responsabilidades, plazos, decisiones y riesgos.

**Resultado esperado:**

Los alumnos comprenden que la calidad de la salida depende tanto del prompt como de la revisión humana posterior.

**Verificación:**

El instructor verifica oralmente que los alumnos distinguen entre:

- **Hecho registrado en las notas**.
- **Interpretación o síntesis generada por Copilot**.
- **Dato no informado**, que no debe ser completado por suposición.

---

### Paso 3: Solicitar a Copilot Chat un borrador de minuta estructurada

**Objetivo:** Demostrar cómo utilizar Copilot Chat para transformar las notas de reunión en una minuta estructurada y trazable a su fuente.

**Instrucciones:**

1. El instructor abre Microsoft Copilot Chat desde el entorno de Microsoft 365 autorizado.
2. El instructor confirma en pantalla que está usando la cuenta corporativa de demostración:

   ```text
   instructor.copilotdemo@contoso-bancoestado-demo.onmicrosoft.com
   ```

3. El instructor inicia una nueva conversación en Copilot Chat.
4. El instructor adjunta o referencia el archivo de notas de reunión, según las opciones disponibles en la interfaz de Copilot Chat del tenant de demostración.
5. El instructor pega el siguiente prompt. Si la interfaz permite seleccionar el documento adjunto, debe comprobar que el archivo seleccionado es el documento de notas de reunión correcto.

   ```text
   Actúa como asistente de documentación para una reunión interna ficticia del Programa de Educación Financiera BancoEstado.

   Usa exclusivamente la información contenida en el documento adjunto o referenciado:
   Notas_Reunion_Seguimiento_Programa_Educacion_Financiera_2026-09-14.docx

   Objetivo: generar un borrador de minuta profesional para circulación interna y revisión humana.

   Audiencia: equipo de seguimiento del programa y responsables de las actividades acordadas.

   Genera la minuta en español de Chile, con fecha en formato dd-MM-aaaa, y utiliza exactamente estas secciones:

   1. Fecha
   2. Asistentes
   3. Objetivo de la reunión
   4. Temas principales
   5. Resumen de discusión
   6. Decisiones
   7. Acuerdos
   8. Responsables
   9. Fechas comprometidas
   10. Riesgos o dependencias
   11. Próximos pasos

   Restricciones obligatorias:
   - No inventes asistentes, responsables, cargos, decisiones, compromisos, fechas ni indicadores.
   - Distingue explícitamente entre decisiones confirmadas, propuestas y asuntos pendientes.
   - Si una sección o dato no aparece de forma explícita en las notas, escribe: "No especificado en las notas".
   - No uses datos externos ni conocimiento general para completar información.
   - Mantén un tono objetivo, claro y conciso.
   - Presenta acuerdos, responsables y fechas en una tabla cuando la información esté explícitamente disponible.
   ```

6. El instructor envía el prompt.
7. Mientras Copilot procesa la solicitud, el instructor explica que el prompt incluye los cinco componentes que mejoran la utilidad de una solicitud:
   - **Contexto:** Programa de Educación Financiera BancoEstado y reunión interna ficticia.
   - **Objetivo:** generar un borrador de minuta.
   - **Audiencia:** equipo de seguimiento y responsables.
   - **Formato:** secciones explícitas y tabla para compromisos.
   - **Restricciones:** no inventar información y marcar ausencias de datos.

**Resultado esperado:**

Copilot Chat genera un borrador de minuta organizado en las secciones solicitadas, basado en el archivo de notas proporcionado.

**Verificación:**

El instructor comprueba que la respuesta:

- Incluye las once secciones solicitadas.
- Distingue decisiones de asuntos en discusión o pendientes.
- No presenta datos externos al documento fuente.
- Usa “No especificado en las notas” cuando una información solicitada no está presente.
- Incluye una tabla de acuerdos, responsables y fechas solo cuando dichos datos están explícitamente documentados.

> **Mensaje clave para los alumnos:** Una respuesta bien estructurada no garantiza que sea correcta. La estructura facilita la revisión, pero no reemplaza la confirmación contra las notas originales.

---

### Paso 4: Revisar y validar el borrador generado por Copilot

**Objetivo:** Demostrar una revisión humana sistemática para evitar errores, omisiones o afirmaciones no sustentadas por las notas de la reunión.

**Instrucciones:**

1. El instructor mantiene abiertas, idealmente lado a lado, las siguientes ventanas:
   - El documento fuente en Word.
   - La respuesta de Copilot Chat.
2. El instructor revisa la sección **Fecha** y confirma que corresponde a la fecha indicada en las notas de la reunión.
3. El instructor revisa la sección **Asistentes** comparando cada nombre con el documento fuente.
4. El instructor enfatiza que no se deben aceptar como asistentes:
   - Personas mencionadas en la conversación, pero no confirmadas como participantes.
   - Personas asignadas a una tarea que no estuvieron presentes.
   - Cargos o nombres completados por inferencia.
5. El instructor revisa la sección **Objetivo de la reunión** y valida que represente el propósito registrado, sin ampliar el alcance de la sesión.
6. El instructor revisa los **Temas principales** y el **Resumen de discusión**, verificando que:
   - Sean síntesis fieles de las notas.
   - No mezclen temas distintos.
   - No omitan asuntos relevantes de presentación, indicadores o seguimiento.
   - No conviertan opiniones en hechos.
7. El instructor revisa especialmente las secciones **Decisiones** y **Acuerdos**:
   - Confirma que cada decisión figure como aprobada o acordada en las notas.
   - Identifica si Copilot clasificó erróneamente una propuesta como decisión.
   - Elimina o corrige cualquier afirmación que no esté respaldada por el documento.
8. El instructor revisa la tabla de **Responsables** y **Fechas comprometidas**:
   - Comprueba que cada responsable haya sido mencionado explícitamente.
   - Comprueba que cada fecha esté escrita en las notas.
   - Si hay fechas relativas, por ejemplo “la próxima semana”, el instructor no las convierte en una fecha exacta sin confirmación.
   - Si una tarea no tiene responsable o plazo explícito, mantiene el texto “No especificado en las notas” o lo deja como pendiente de validación.
9. El instructor revisa la sección **Riesgos o dependencias**, confirmando que solo se incluyan riesgos realmente mencionados o claramente documentados.
10. El instructor explica a los alumnos que una minuta validada debe permitir responder, sin ambigüedad, estas preguntas:
    - ¿Qué se decidió?
    - ¿Qué se acordó hacer?
    - ¿Quién es responsable?
    - ¿Para cuándo?
    - ¿Qué impide o podría afectar el avance?
    - ¿Qué debe ocurrir después de la reunión?

**Resultado esperado:**

El instructor identifica y corrige posibles diferencias entre el borrador de Copilot y las notas fuente antes de usar el contenido para crear el documento final.

**Verificación:**

El instructor utiliza la siguiente lista de control durante la revisión:

| Elemento a validar | Criterio de aceptación |
|---|---|
| Fecha | Coincide exactamente con las notas. |
| Asistentes | Solo incluye participantes explícitamente identificados. |
| Decisiones | Están respaldadas por un acuerdo o definición explícita. |
| Acuerdos | No confunden propuestas con compromisos aprobados. |
| Responsables | Se asignan solo cuando el nombre aparece explícitamente en las notas. |
| Fechas | Están documentadas y usan formato dd-MM-aaaa cuando se conoce la fecha exacta. |
| Riesgos | Provienen de lo discutido o registrado; no son inferencias no validadas. |
| Próximos pasos | Son accionables y coherentes con los acuerdos confirmados. |

---

### Paso 5: Solicitar una versión breve para correo electrónico

**Objetivo:** Demostrar cómo reutilizar la minuta validada para crear un resumen breve y accionable destinado a correo electrónico.

**Instrucciones:**

1. Una vez revisado el borrador, el instructor solicita a Copilot Chat una versión resumida para correo electrónico.
2. El instructor utiliza el siguiente prompt:

   ```text
   A partir del borrador de minuta anterior y sin agregar información nueva, redacta un correo breve de seguimiento en español de Chile.

   Destinatarios: participantes y responsables de seguimiento de la reunión ficticia.

   Incluye:
   - Asunto de correo.
   - Agradecimiento breve por la reunión.
   - Resumen de las decisiones confirmadas.
   - Lista de acuerdos con responsable y fecha solo cuando estén explícitamente indicados.
   - Riesgos o pendientes que requieran validación.
   - Próximo paso general.

   Restricciones:
   - No inventes nombres, responsables, fechas, decisiones ni compromisos.
   - Si un dato no está confirmado, indícalo como pendiente de validación.
   - Mantén una extensión máxima aproximada de 180 palabras.
   - Usa un tono profesional y objetivo.
   ```

3. El instructor envía el prompt.
4. El instructor muestra cómo revisar que la versión breve no haya perdido condiciones importantes, como:
   - Un responsable.
   - Una fecha comprometida.
   - Un riesgo relevante.
   - La indicación de que un elemento requiere confirmación.
5. El instructor explica que un correo breve no reemplaza la minuta formal; es un mecanismo de comunicación y seguimiento. La minuta es el registro estructurado que debe conservar el detalle validado.

**Resultado esperado:**

Copilot genera un correo breve con asunto, decisiones, acuerdos y próximos pasos, sin agregar contenido que no esté presente en la minuta validada o en las notas originales.

**Verificación:**

El instructor verifica que el correo:

- Tiene un asunto claro relacionado con la reunión de seguimiento.
- Resume solo decisiones confirmadas.
- No presenta responsables o fechas inexistentes.
- Distingue los pendientes de validación.
- Mantiene un tono apropiado para una comunicación interna.

---

### Paso 6: Crear y guardar la minuta final en Word

**Objetivo:** Demostrar cómo transformar el borrador validado en un documento Word formal y guardarlo con el nombre establecido.

**Instrucciones:**

1. El instructor vuelve a Microsoft Word.
2. El instructor crea un documento en blanco.
3. El instructor copia el contenido validado de la minuta desde Copilot Chat o lo utiliza como referencia para redactar el documento en Word.
4. El instructor aplica una estructura clara con encabezados para las siguientes secciones:
   1. Fecha
   2. Asistentes
   3. Objetivo de la reunión
   4. Temas principales
   5. Resumen de discusión
   6. Decisiones
   7. Acuerdos
   8. Responsables
   9. Fechas comprometidas
   10. Riesgos o dependencias
   11. Próximos pasos
5. El instructor aplica estilos de Word, por ejemplo:
   - Título para el nombre de la minuta.
   - Encabezado 1 para cada sección.
   - Tabla para acuerdos, responsables y fechas, cuando exista información confirmada.
6. El instructor agrega una tabla de seguimiento con una estructura como la siguiente, solo para información validada:

   | Acuerdo o actividad | Responsable | Fecha comprometida | Estado o nota |
   |---|---|---|---|
   | Según notas validadas | Según notas validadas | Según notas validadas | Pendiente, en curso o no especificado |

7. El instructor no completa con suposiciones los campos sin información. Cuando corresponda, conserva la indicación:

   ```text
   No especificado en las notas
   ```

8. El instructor guarda el documento con el nombre obligatorio:

   ```text
   Minuta_Seguimiento_Programa_Educacion_Financiera_2026-09-14.docx
   ```

9. El instructor guarda el archivo en la ruta:

   ```text
   C:\CopilotM365Labs\BancoEstadoDemo\Minuta_Seguimiento_Programa_Educacion_Financiera_2026-09-14.docx
   ```

10. Si el flujo de la organización requiere almacenamiento en SharePoint, el instructor puede guardar una copia en la biblioteca de demostración autorizada:

   ```text
   /sites/CopilotM365Demo/Documentos compartidos/Labs/01_Contexto_BancoEstado/
   ```

11. El instructor explica que una minuta no debe distribuirse automáticamente solo porque fue guardada. Debe pasar por la revisión humana definida por el proceso de trabajo.

**Resultado esperado:**

Se crea y guarda un documento Word con una minuta estructurada, revisada y basada exclusivamente en las notas ficticias de reunión.

**Verificación:**

El instructor confirma que:

- El archivo se guardó con el nombre correcto.
- El archivo tiene extensión `.docx`.
- Todas las secciones solicitadas están presentes.
- Las responsabilidades y fechas están respaldadas por las notas.
- Los datos no especificados no han sido inventados.
- El documento no contiene información real de producción ni datos personales no autorizados.

## Validación y pruebas

El instructor realiza la siguiente validación final frente a los alumnos antes de cerrar la demostración.

### Prueba 1: Confirmación del archivo final

1. En el Explorador de archivos, el instructor navega a:

   ```text
   C:\CopilotM365Labs\BancoEstadoDemo\
   ```

2. El instructor comprueba que existe el archivo:

   ```text
   Minuta_Seguimiento_Programa_Educacion_Financiera_2026-09-14.docx
   ```

**Resultado esperado:** El archivo existe en la carpeta de trabajo y puede abrirse en Word.

### Prueba 2: Validación de contenido contra la fuente

El instructor selecciona al menos un elemento de cada categoría y lo compara entre las notas originales y la minuta final:

| Categoría | Acción de validación |
|---|---|
| Asistentes | Confirmar que cada participante aparece explícitamente en las notas. |
| Decisiones | Confirmar que cada decisión fue efectivamente acordada. |
| Acuerdos | Confirmar que las tareas no son solo sugerencias o ideas. |
| Responsables | Confirmar que cada asignación está documentada. |
| Fechas | Confirmar que cada fecha existe en la fuente. |
| Riesgos | Confirmar que los riesgos no fueron deducidos sin sustento. |
| Próximos pasos | Confirmar que son coherentes con los acuerdos y pendientes. |

**Resultado esperado:** Cada elemento revisado tiene respaldo en el documento fuente o está marcado como no especificado o pendiente de validación.

### Prueba 3: Validación de uso responsable de IA

El instructor formula las siguientes preguntas de cierre a los alumnos:

1. ¿Qué ocurriría si Copilot asignara una tarea a una persona que no fue definida como responsable?
2. ¿Por qué una fecha inferida no debe presentarse como un compromiso confirmado?
3. ¿Qué diferencia existe entre una propuesta discutida y una decisión aprobada?
4. ¿Por qué la minuta debe revisarse antes de enviarse por correo?

**Resultado esperado:** Los alumnos reconocen que Copilot acelera la elaboración de un borrador, pero la exactitud, autorización y distribución de la minuta siguen siendo responsabilidad humana.

## Solución de problemas

### Problema 1: Copilot Chat no permite adjuntar o encontrar el documento de notas

**Síntoma:** El instructor no puede adjuntar `Notas_Reunion_Seguimiento_Programa_Educacion_Financiera_2026-09-14.docx`, Copilot no lo reconoce o no puede acceder a su contenido.

**Causa probable:** El archivo no está disponible en una ubicación accesible para la cuenta de demostración, no terminó de sincronizarse con SharePoint/OneDrive o el instructor inició sesión con una cuenta distinta de la cuenta corporativa autorizada.

**Solución:**

1. Confirmar que el instructor inició sesión con:

   ```text
   instructor.copilotdemo@contoso-bancoestado-demo.onmicrosoft.com
   ```

2. Comprobar que el archivo existe en la carpeta local de demostración:

   ```powershell
   Test-Path "C:\CopilotM365Labs\BancoEstadoDemo\Notas_Reunion_Seguimiento_Programa_Educacion_Financiera_2026-09-14.docx"
   ```

3. Si el archivo se encuentra en SharePoint, abrirlo desde la biblioteca autorizada y confirmar que está disponible para la cuenta de demostración.
4. Reiniciar la conversación de Copilot Chat y volver a adjuntar o referenciar el archivo correcto.
5. Si la interfaz no admite adjuntos en ese momento, el instructor puede utilizar Word como fuente visual y solicitar una demostración conceptual del prompt, sin pegar contenido sensible ni información fuera del entorno autorizado.

### Problema 2: Copilot presenta asistentes, responsables o fechas que no aparecen claramente en las notas

**Síntoma:** El borrador de Copilot incluye nombres, responsabilidades, decisiones o plazos que no pueden confirmarse en el documento fuente.

**Causa probable:** Copilot interpretó una mención contextual como una asignación formal, convirtió una propuesta en decisión o completó información ambigua durante la síntesis.

**Solución:**

1. No aceptar ni distribuir el contenido no confirmado.
2. Comparar cada afirmación con las notas originales.
3. Eliminar o reemplazar el dato no sustentado por:

   ```text
   No especificado en las notas
   ```

4. Solicitar una corrección a Copilot Chat con un prompt como el siguiente:

   ```text
   Revisa el borrador anterior usando exclusivamente las notas fuente.
   Elimina cualquier asistente, responsable, fecha, decisión o compromiso que no esté indicado de forma explícita.
   Para los datos ausentes, escribe "No especificado en las notas".
   Distingue las propuestas de las decisiones confirmadas.
   ```

5. Repetir la validación humana antes de incorporar el contenido corregido al documento Word final.

## Limpieza

Al finalizar la demostración, el instructor debe:

1. Guardar y cerrar el documento final:

   ```text
   C:\CopilotM365Labs\BancoEstadoDemo\Minuta_Seguimiento_Programa_Educacion_Financiera_2026-09-14.docx
   ```

2. Cerrar el documento de notas original sin modificarlo, a menos que el procedimiento de demostración haya requerido una copia de trabajo.
3. Cerrar la conversación de Copilot Chat o iniciar una conversación nueva antes de una demostración con otro escenario.
4. Cerrar sesión de Microsoft 365 si el equipo será utilizado por otro instructor o grupo.
5. Confirmar que no se copiaron archivos ficticios del tenant de demostración a ubicaciones personales, cuentas de producción o servicios no autorizados.
6. Mantener los archivos únicamente en la carpeta local de laboratorio o en la biblioteca de SharePoint de demostración autorizada.

## Resumen

En esta demostración, el instructor utilizó Copilot Chat para generar un borrador de minuta a partir de notas desestructuradas de una reunión ficticia. La solicitud incluyó contexto, objetivo, audiencia, formato de salida y restricciones explícitas para evitar que Copilot completara información no documentada.

La actividad mostró que una minuta profesional debe separar temas, decisiones, acuerdos, responsables, fechas, riesgos y próximos pasos. También reforzó que la salida de IA debe validarse cuidadosamente contra la fuente original antes de utilizarse en comunicaciones o documentos de trabajo.

### Recursos opcionales

- [Uso de Copilot en Microsoft 365](https://support.microsoft.com/es-es/copilot)
- [Resumir reuniones en Microsoft Teams con Copilot](https://support.microsoft.com/es-es/office/resumir-reuniones-en-microsoft-teams-con-copilot-5a1fcf36-6e40-4c3e-aacf-03d864b2157f)
- [Principios de IA responsable de Microsoft](https://www.microsoft.com/es-es/ai/responsible-ai)
