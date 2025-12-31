MR_contaminación_del_aire_envejecimiento_epigenético
Descripción del proyecto

Este repositorio documenta un pipeline de inferencia causal basado en Mendelian Randomization (MR) para evaluar la relación entre contaminación atmosférica, inflamación sistémica y envejecimiento epigenético acelerado, utilizando estadísticas de resumen provenientes de estudios genómicos a gran escala.

El objetivo principal es explorar mecanismos causales, no asociaciones descriptivas, bajo un marco metodológico reproducible y alineado con estándares internacionales de reporte.

Pregunta causal

¿Cuál es el efecto causal de la exposición a contaminación atmosférica sobre el envejecimiento epigenético acelerado, y en qué medida este efecto podría estar mediado por inflamación sistémica?

Diseño metodológico

El estudio se basa en un enfoque de Aleatorización Mendeliana (MR) utilizando estadísticas de resumen (two-sample MR), estructurado en un pipeline modular guiado por DAGs.

Componentes clave:

Diseño causal previo mediante DAG

Selección y validación de instrumentos genéticos
(p < 5×10⁻⁸, r² < 0.001, F > 10)

Armonización de alelos

Modelos de inferencia causal, seleccionados según la pregunta y la disponibilidad de datos:

MR univariable (Exposición → Outcome)

MR de mediación / two-step MR (Exposición → Mediador → Outcome)

Multivariable MR (MVMR)

MR bidireccional (cuando aplica)

Análisis de robustez y sensibilidad
(IVW, MR-Egger, weighted median/mode, heterogeneidad, pleiotropía, leave-one-out)

Variables principales

Exposición: indicadores genéticos proxy de contaminación atmosférica (ej. PM₂.₅, NO₂)

Mediadores: marcadores de inflamación sistémica (ej. CRP)

Desenlaces: relojes epigenéticos (GrimAge, PhenoAge, Hannum, Horvath)

Fuentes de datos

IEU OpenGWAS: https://gwas.mrcieu.ac.uk

MR-Base: https://www.mrbase.org

EWAS Atlas (opcional): https://ngdc.cncb.ac.cn/ewas/

Todos los datos utilizados son secundarios, anonimizados y de acceso público.

Estado del proyecto

✔ Diseño causal (DAG) definido

✔ Pipeline metodológico estructurado

🔄 Análisis MR en desarrollo

🔄 Integración de resultados y sensibilidad

Transparencia y reproducibilidad

El proyecto sigue las directrices STROBE-MR para estudios de Aleatorización Mendeliana.
Este repositorio alojará:

Scripts de análisis en R

Figuras (forest plots, scatter plots, funnel plots)

Tablas de resultados y sensibilidad

Documentación metodológica reproducible

Licencia

Este proyecto se distribuye bajo Licencia MIT.

Contacto

Irma Valdebenito
Doctorado en Salud Ambiental y Biomedicina
Chile
