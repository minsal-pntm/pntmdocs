---
layout: default
title: Reporte Global de solicitudes
nav_order: 1
grand_parent: Reportes
parent: Reportes - Laboratorio
has_children: false
has_toc: true
---

# Reporte Global de solicitudes

La Plataforma Nacional de Toma de Muestra (PNTM) es un sistema diseñado para recopilar información sobre muestras de pruebas de diagnóstico, como las pruebas PCR y de antígenos, realizadas en establecimientos de salud pública en todo el país.
El reporte global de solicitudes es una herramienta que permite a los usuarios obtener información sobre las muestras de prueba realizadas en la PNTM. Para generar este informe, los usuarios deben asignar una fecha de inicio (DESDE) y una fecha de finalización (HASTA) que correspondan a la fecha de toma de muestra.

Es importante destacar que si el usuario no asigna ninguna fecha, el sistema tomará automáticamente la fecha y hora actual como el punto de partida y finalización para la generación del reporte.

El reporte global de solicitudes proporciona información detallada sobre el número total de muestras de prueba realizadas en la PNTM durante el período de tiempo especificado. Esto permite a los usuarios obtener información más específica sobre la distribución de muestras.

El reporte generado por la Plataforma Nacional de Toma de Muestra (PNTM) contiene información detallada sobre las muestras de prueba de diagnóstico, como las pruebas PCR y de antígenos, realizadas en establecimientos de salud pública en todo el país. A continuación se describen los campos que se incluyen en el reporte:

Para acceder al reporte global de solicitudes de PCR, sigue estos pasos:

- Accede al menú de reportes en la interfaz de usuario.
- Selecciona el submenú de PCR en la lista de opciones disponibles.
- Haz clic en el botón para generar el reporte global de solicitudes.
Selecciona las fechas "DESDE" y "HASTA" para definir el rango de tiempo que deseas incluir en el reporte. Ten en cuenta que estas fechas corresponden a la fecha de toma de la muestra.
- Si no asignas ninguna fecha, el sistema tomará por defecto el día y la hora actual.
Una vez que ingreses las fechas requeridas, el reporte global de solicitudes de PCR se generará automáticamente y se descargará automáticamente a tu dispositivo en el formato Excel.


![Alt text](img/Reporte-PCR.jpg)

_Reporte global de solicitudes_

![Alt text](img/Reportes-PCR-Global.png)

_Reporte global de solicitudes_

El reporte generado por la Plataforma Nacional de Toma de Muestra (PNTM) contiene información detallada sobre las muestras de prueba de diagnóstico, como las pruebas PCR y de antígenos, realizadas en establecimientos de salud pública en todo el país. A continuación se describen los campos que se incluyen en el reporte:

- `id_muestra`: un número único que identifica a cada muestra de prueba.
- `estado_muestra`: el estado actual de la muestra de prueba (ej. si se encuentra en proceso de análisis o ya se tiene un resultado disponible).
- `estado_muestra_significado`: una descripción del significado del estado de la muestra de prueba.


| Estado de muestra | Descripción                                                                                                                                                                                                                                                 |
|-------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| 1                 | La muestra de prueba se encuentra en proceso de creación y aún no se ha enviado al laboratorio.                                                                                                                                                             |
| 2                 | La muestra de prueba ha sido enviada al laboratorio para su procesamiento.                                                                                                                                                                                  |
| 3                 | La muestra de prueba ha sido recepcionada por el laboratorio y se encuentra en proceso de análisis.                                                                                                                                                         |
| 4                 | La muestra de prueba ha sido procesada y se dispone de un resultado.                                                                                                                                                                                        |
| 5                 | La muestra de prueba se encuentra en proceso de modificación, es decir, se está realizando alguna corrección o actualización de la información asociada a la muestra.                                                                                       |
| 6                 | La muestra de prueba ha sido rechazada y no es apta para su procesamiento.                                                                                                                                                                                  |
| 7                 | La muestra de prueba ha sido enviada a mutaciones para su análisis y seguimiento.                                                                                                                                                                           |
| 8                 | La muestra de prueba ha sido procesada en mutaciones y se dispone de un resultado de la mutación.                                                                                                                                                           |
| 9                 | La muestra de prueba se encuentra en un estado de edición autorizada, es decir, se ha dado permiso a un usuario específico para realizar modificaciones en la información asociada a la muestra. Este estado se utiliza para evitar cambios no autorizados. |

- `nombre_profesional`, `rut_profesional`, `titulo_profesional`, `especialidad_profesional`: información sobre el profesional de salud que tomó la muestra de prueba.
- `profesional_solicitante`, `rut_profesional_solicitante`: información sobre el profesional de salud que solicitó la toma de muestra.
- `tipo_documento_paciente`, `id_paciente`: información sobre el paciente al que se le realizó la prueba.
- `pais_origen_paciente`, `nombre_paciente`, `apellido_paterno_paciente`, `apellido_materno_paciente`, `fecha_nacimiento_paciente`, `edad_paciente`, `comuna_paciente`, `dirección_paciente`, `telefono_paciente`, `paciente_email`, `sexo_paciente`, `prevision_paciente`: información personal y médica del paciente al que se le realizó la prueba.
- `laboratorio`, `tipo_laboratorio`, `codigo_servicio_salud_laboratorio`, `servicio_salud_laboratorio`: información sobre el laboratorio que procesó la muestra de prueba.
- `establecimiento`, `fecha_toma_muestra`, `hora_muestra`, `tecnica_muestra`, `resultado`, `tipo_muestra`, `codigo_servicio_salud_establecimiento`, `servicio_salud_establecimiento`: información sobre el establecimiento de salud donde se realizó la toma de muestra, así como detalles sobre la técnica utilizada para la prueba y los resultados obtenidos.
- `epivigila`: información sobre el sistema de vigilancia epidemiológica utilizado para el seguimiento de los casos.
- `fecha_recepcion_muestra`, `hora_recepcion`, `fecha_resultado_muestra`, `hora_resultado`: información sobre la fecha y hora de recepción de la muestra y la fecha y hora de los resultados obtenidos.
- `busqueda_activa` es un campo que indica si la muestra de prueba se realizó como parte de una búsqueda activa de casos (BAC). Si el valor de este campo es "VERDADERO", significa que la muestra se tomó como parte de un operativo BAC, mientras que si es "FALSO", significa que la muestra se tomó por otra razón.
- `tiposolicitud`, `codigo_muestra_cliente`, `fecha_informada_recepcion_laboratorio`, `hora_informada_recepcion_laboratorio`, `fecha_informada_resultado_laboratorio`, `hora_informada_resultado_laboratorio`, `fecha_creacion`, `tipo_establecimiento`, `estrategia`, `subestrategia`: información adicional sobre la muestra de prueba, como el tipo de búsqueda utilizada para la detección de casos y la estrategia de atención médica utilizada.

En resumen, el reporte global de solicitudes de la PNTM es una herramienta para obtener información sobre las muestras de prueba realizadas en establecimientos de salud pública en todo el país. Los usuarios pueden utilizar este informe para analizar la distribución de muestras de prueba en diferentes áreas y tipos de establecimientos de salud, lo que puede ayudar a informar la toma de decisiones en materia de salud.