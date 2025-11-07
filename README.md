# Showz: Análisis de Rentabilidad de Marketing (ROMI)

## Contexto del Proyecto

"Showz", una empresa de venta de entradas para eventos, busca optimizar sus gastos de marketing. Este proyecto analiza los registros del servidor, los pedidos y los costos de marketing desde enero de 2017 hasta diciembre de 2018 para identificar qué canales de adquisición son rentables y cuáles no.

## Objetivos del Análisis

1.  **Analizar el Comportamiento del Usuario:** Entender cómo usan el servicio (DAU, WAU, MAU) y cuándo compran.
2.  **Calcular Métricas de Negocio:** Determinar el Costo de Adquisición de Clientes (CAC) y el Valor de Vida del Cliente (LTV) por cada fuente de marketing.
3.  **Evaluar la Rentabilidad (ROMI):** Calcular el Retorno de la Inversión en Marketing (ROMI) para cada fuente, identificando el punto de equilibrio.
4.  **Generar Recomendaciones:** Aconsejar al equipo de marketing sobre dónde reasignar el presupuesto para maximizar la rentabilidad.

## Herramientas Utilizadas

* **Python**
* **Pandas** para la manipulación, limpieza y agrupación de datos.
* **Matplotlib** y **Seaborn** para la visualización de datos (mapas de calor, gráficos de barras).
* **Jupyter Notebook** como entorno de trabajo.

## Hallazgos Clave y Análisis de Rentabilidad

El análisis se centró en el **ROMI (Retorno de la Inversión en Marketing)**, ya que es la métrica definitiva que une los costos (CAC) con los ingresos (LTV).

**ROMI = LTV / CAC**

El punto de equilibrio (rentabilidad) se establece en **ROMI = 1.0**, donde los ingresos generados por un cliente igualan el costo de adquirirlo.

* **Fuentes Rentables (ROMI > 1.0):**
    * **Fuente 1:** Es la plataforma más rentable, con un ROMI de ~1.5. Cada $1 invertido genera ~$1.50 de vuelta.
    * **Fuente 2:** Rentable, con un ROMI de ~1.1.
    * **Fuente 5 y 9:** Ligeramente rentables, con un ROMI justo por encima del punto de equilibrio.

* **Fuentes No Rentables (ROMI < 1.0):**
    * **Fuente 4 y 10:** A pesar de tener un CAC (costo) bajo, el LTV de sus clientes no es suficiente para ser rentables.
    * **Fuente 3:** Es la plataforma con peor desempeño, con un ROMI negativo (~ -0.6). Cada cliente adquirido por esta fuente genera una pérdida neta significativa.

## Recomendaciones Estratégicas

Basado en el análisis de ROMI, se proponen las siguientes acciones para optimizar el presupuesto de marketing:

1.  **Priorizar y Aumentar Inversión (ROMI > 1.0):**
    * Reasignar el presupuesto para **aumentar la inversión** en la **Fuente 1**, ya que es el motor de rentabilidad más fuerte.
    * Mantener y optimizar la inversión en las **Fuentes 2, 5 y 9**, monitoreando que su ROMI se mantenga por encima de 1.0.

2.  **Pausar o Eliminar Inversión (ROMI < 1.0):**
    * **Pausar inmediatamente** la inversión en la **Fuente 3**. Esta plataforma está perdiendo dinero activamente.
    * **Reducir o pausar** la inversión en las **Fuentes 4 y 10**. Aunque son baratas para adquirir clientes, no son rentables; ese presupuesto estaría mejor reasignado a la Fuente 1.

### Conclusión Final
Showz debe reenfocar su estrategia de "adquisición barata" (CAC bajo) a "adquisición rentable" (ROMI alto). La clave es invertir en las fuentes que demuestren un retorno sobre la inversión superior a 1.0.
