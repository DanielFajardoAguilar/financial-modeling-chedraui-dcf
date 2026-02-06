# Valuación de acciones Chedraui (DCF + WACC) en Excel

Este repositorio contiene un modelo financiero en Excel para estimar el valor del capital (equity value) y un valor teórico por acción de Chedraui mediante el enfoque de Flujo de Efectivo Descontado (DCF), utilizando información pública.

Incluye:
- Proyección de ingresos, costos y partidas relevantes
- Cálculo de flujo de efectivo libre (FCL)
- Estimación de WACC (costo de capital)
- Sensibilidad y escenarios
- Reporte en PDF con explicación del procedimiento

## Contenido del repositorio
- model/Chedraui_Modelo.xlsx  
  Archivo principal del modelo.
- report/Valor_de_las_acciones.pdf  
  Documento con metodología, supuestos y conclusiones.
- screenshots/  
  Capturas del modelo (para lectura rápida).

## Metodología (resumen)
1) Proyección de desempeño
Se proyectan variables operativas y financieras en un horizonte multianual con base en supuestos explícitos (crecimiento, márgenes, inversión, capital de trabajo).

2) Flujo de efectivo libre (FCL)
Se estima el FCL a partir de utilidad operativa y ajustes típicos (depreciación, inversiones, cambios en capital de trabajo, impuestos), y se descuenta a valor presente.

3) Tasa de descuento (WACC)
Se calcula una tasa de descuento con base en estructura de capital, costo de deuda y costo de capital. El WACC se usa para descontar el FCL.

4) Valor terminal y valuación por acción
Se incluye valor terminal y se obtiene un valor de negocio y un valor del capital. A partir de ahí se obtiene un valor por acción.

5) Escenarios y sensibilidad
Se evalúan cambios razonables en supuestos clave para observar la estabilidad del resultado.

## Resultado y lectura correcta del número final
El modelo entrega un valor estimado bajo los supuestos seleccionados. Ese número no es “la verdad”, es una consecuencia directa de:
- supuestos de crecimiento/márgenes
- inversiones y capital de trabajo proyectados
- WACC seleccionado
- tratamiento del valor terminal
- consistencia y disponibilidad de datos históricos

Por eso el resultado debe interpretarse como un rango (según escenarios) y no como un punto exacto.

## Posibles afectaciones al cálculo (limitaciones reales)
Este proyecto usa información pública. En la práctica, algunos datos necesarios no siempre están completos o disponibles con el mismo nivel de detalle, lo cual puede afectar el cálculo. Ejemplos típicos:

1) Datos faltantes o incompletos
Esto puede distorsionar el FCL y, por tanto, el valor final.

2) Supuestos “forzados” por falta de guía
Cuando no hay información suficiente para justificar una tasa o un crecimiento, se usan supuestos conservadores o escenarios. Esto es correcto como ejercicio, pero el valor por acción cambia mucho con pequeñas variaciones.

3) Sensibilidad alta al WACC y al valor terminal
En DCF, gran parte del valor suele venir del valor terminal. Si cambias WACC o la tasa de crecimiento terminal, el resultado puede moverse fuerte (a veces demasiado). Por eso se incluyen escenarios.

4) Calidad de la serie histórica
Si ciertos años tienen eventos atípicos (cambios contables, shocks de mercado, efectos no recurrentes), proyectar “como si fuera normal” puede inducir sesgo.

5) Diferencias entre “valor teórico” y “precio de mercado”
Aunque el modelo esté bien armado, el mercado puede estar valuando:
- expectativas distintas
- riesgo percibido
- liquidez y sentimiento
- noticias recientes
El DCF no pretende adivinar el precio de mañana; pretende estimar valor bajo supuestos.

## Notas
- Proyecto académico y reproducible con información pública.
- El objetivo es mostrar criterio financiero, estructuración de modelo y trazabilidad de supuestos.

