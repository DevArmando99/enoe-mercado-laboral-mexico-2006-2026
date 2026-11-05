# Criterios metodológicos base

Este documento resume los criterios transversales del cuaderno. La definición implementada, las validaciones y los filtros exactos se documentarán en el cuaderno técnico definitivo.

## Universo y expansión

El análisis considera observaciones ocupadas con factor trimestral de expansión válido y positivo. Los conteos son estimaciones de población al aplicar `fac_tri`; no son recuentos de registros muestrales.

## Ingresos reales

Los ingresos se expresan en pesos de 2026T1. Para cada trimestre se aplica un factor de deflactación obtenido del INPC; el factor de 2026T1 es 1. Las comparaciones temporales se interpretan en términos reales.

## Medidas de posición

Cuando se reporta una mediana, percentil o decil de población, la posición se calcula de manera ponderada: se ordena la variable y se acumulan los factores de expansión hasta alcanzar la proporción de población de interés. Esto equivale conceptualmente a representar a cada observación según el tamaño poblacional que representa, sin expandir físicamente la base.

## Empleo principal y horas

Las horas trabajadas se refieren al empleo principal. El ingreso real por hora se obtiene a partir del ingreso laboral individual del empleo principal, las horas semanales declaradas y el factor de conversión mensual definido en el cuaderno.

## Formalidad

La clasificación de formalidad corresponde a la variable de empleo principal conservada en la base analítica. Los resultados formal/informal deben leerse dentro del universo con empleo clasificado.

## Limitaciones

La ENOE es una encuesta por muestreo y las comparaciones descriptivas no identifican relaciones causales. El segundo trimestre de 2020 se excluye por la interrupción del levantamiento habitual. Para 2026 solo se incorpora T1.
