# Desafío Alura Store: Análisis de Rendimiento de Tiendas y Recomendación Estratégica 📈📉💰

## Introducción al Proyecto 🚀

¡Bienvenidos/as al primer desafío de la especialización en Data Science del programa Oracle Next Education - con Alura Latam!

Este proyecto se centra en un caso de negocio: **ayudar al Sr. Juan, propietario de la cadena de tiendas "Alura Store", a tomar una decisión estratégica crucial.** El Sr. Juan necesita identificar cuál de sus **cuatro tiendas actuales tiene el menor desempeño** para poder venderla y liberar capital, el cual planea invertir en un nuevo emprendimiento.

Mi rol en este desafío ha sido actuar como **Analista de Datos**, utilizando el poder de Python y sus librerías para procesar, analizar y visualizar los datos de ventas y rendimiento de cada tienda. El objetivo final es proporcionar una **recomendación clara y justificada**, basada en evidencia, sobre qué tienda debería considerar vender el Sr. Juan.

---

## El Problema a Resolver 🤔

El desafío consistió en responder a la pregunta central del Sr. Juan: **¿Qué tienda de Alura Store es la menos eficiente o rentable, y por qué?**

Para ello, mi análisis se basó en los siguientes **cinco aspectos clave** del rendimiento de cada tienda:

1.  **Facturación Total:** Cuánto dinero ha generado cada tienda.
2.  **Ventas por Categoría:** Qué tipo de productos (categorías) son los más populares o lucrativos en cada tienda.
3.  **Calificación Promedio de Clientes:** El nivel de satisfacción de los clientes con cada tienda.
4.  **Productos Más y Menos Vendidos:** Identificación de los productos estrella y los de bajo rendimiento en cada sucursal.
5.  **Costo Promedio de Envío:** La eficiencia en los costos de logística de entrega por tienda.

---

## Fuentes de Datos y Herramientas Utilizadas 🛠️

Los datos para este desafío fueron proporcionados por Alura y consisten en archivos CSV individuales para cada una de las cuatro tiendas (`tienda_1.csv`, `tienda_2.csv`, `tienda_3.csv`, `tienda_4.csv`).

Para llevar a cabo el análisis, se utilizaron las siguientes herramientas y librerías:

* **Python 3:** El lenguaje de programación principal.
* **Pandas:** Esencial para la carga, manipulación y análisis de los datos tabulares.
* **Matplotlib:** Utilizada para la creación de visualizaciones de datos claras y efectivas.
* **Google Colab:** El entorno de desarrollo utilizado para el proyecto, facilitando la ejecución y compartición del código.

---

## Metodología y Análisis Realizado ⚙️

El proceso de análisis siguió una metodología estructurada:

1.  **Carga y Consolidación de Datos:** Se cargaron los cuatro archivos CSV en DataFrames de Pandas y se consolidaron en un único DataFrame principal, añadiendo una columna para identificar a qué tienda pertenece cada registro.
2.  **Limpieza y Transformación:** Se realizaron ajustes menores en los tipos de datos (ej., asegurando que las columnas de precios y costos fueran numéricas).
3.  **Cálculo de Métricas Clave:** Se calcularon las métricas relevantes para cada uno de los cinco aspectos de evaluación:
    * Suma de ingresos por tienda (Facturación Total).
    * Promedio de calificaciones por tienda.
    * Promedio del costo de envío por tienda.
    * Ingresos por categoría de producto para cada tienda.
    * Identificación de los 3 productos con mayores y menores ingresos por tienda.
4.  **Generación de Visualizaciones:** Se crearon diferentes tipos de gráficos para representar los hallazgos de manera visual.

---

## Visualizaciones Clave 📊

Para una comprensión clara del rendimiento de cada tienda, se generaron **tres tipos de gráficos distintos**:

1.  **Gráfico de Barras Verticales:** Utilizado para mostrar la **Facturación Total por Tienda**. Permite una comparación directa de los ingresos entre todas las sucursales, identificando rápidamente las tiendas de mayor y menor rendimiento financiero.

    <img width="889" height="590" alt="Grafico barras vertical Ingreso Total Ventas" src="https://github.com/user-attachments/assets/51a83b10-9c22-4650-a11f-4b1a6a7a9da4" />

2.  **Gráfico de Líneas:** Empleado para visualizar el **Promedio de Calificación de Clientes por Tienda**. Este gráfico ayuda a observar la variación en la satisfacción del cliente entre las tiendas, indicando la percepción general de calidad.

    <img width="889" height="590" alt="Grafico promedio calificaciones" src="https://github.com/user-attachments/assets/28b55c1f-24bc-4dc2-9d59-ae3bfc5f3010" />

3.  **Gráfico de Barras Horizontales:** Se usó para representar el **Costo Promedio de Envío por Tienda**. Este formato es efectivo para comparar la eficiencia logística y los gastos operativos relacionados con el envío entre las diferentes tiendas.

    <img width="890" height="590" alt="Grafico costo envios" src="https://github.com/user-attachments/assets/d5e63c97-c05b-4686-88dc-4c3b3c16d4dd" />

---

## Resultados Clave y Recomendación Final 🎯

Tras el análisis de los datos y las visualizaciones, se llegó a la siguiente conclusión sobre el desempeño de cada tienda:

* **Facturación Total:** La **Tienda 1** fue la de mayor facturación, mientras que la **Tienda 4** fue consistentemente la de menor ingreso.
* **Ventas por Categoría y Productos:** **Electrónicos** y **Electrodomésticos** son las categorías clave en todas las tiendas. Sin embargo, la **Tienda 4** mostró una **facturación notablemente menor en Electrodomésticos** en comparación con las otras, contribuyendo a su bajo desempeño general. Los productos top (TV LED UHD 4K, Refrigerador, iPhone 15) y los de menor ingreso (Cuerda para saltar, Cubo mágico 8x8, Dinosaurio Rex) fueron consistentes en todas las tiendas.
* **Costo Promedio de Envío:** La **Tienda 4** demostró ser la **más eficiente** en costos de envío, mientras que la Tienda 1 tuvo los más altos.
* **Calificación Promedio de Clientes:** Las calificaciones fueron generalmente altas en todas las tiendas. La **Tienda 3 y Tienda 2 destacaron ligeramente**, mientras que la **Tienda 1** tuvo el promedio más bajo, pero la **Tienda 4** se mantuvo en un punto intermedio, aceptable pero no sobresaliente.

---

### Recomendación para el Sr. Juan:

Basándome en un análisis integral, mi recomendación al Sr. Juan es considerar la venta de la **Tienda 4**.

**Justificación de la Elección:**

La **Tienda 4** es la que presenta el **menor desempeño general** entre todas las sucursales. Si bien tiene fortalezas como el costo de envío más bajo, estas no logran compensar sus debilidades financieras:

1.  **Menor Facturación Total:** Este es el factor **más crítico**. La Tienda 4 es la que menos ingresos genera, afectando directamente la rentabilidad global.
2.  **Debilidad en Categorías Clave:** Su facturación significativamente menor en la categoría de Electrodomésticos, un pilar de ingresos para las otras tiendas, es un indicador de un problema estructural en sus ventas.
3.  **Eficiencia No Compensatoria:** A pesar de ser la más eficiente en costos de envío, esta ventaja no se traduce en un mejor desempeño financiero general, lo que sugiere que el problema reside en la generación de demanda o ventas, no solo en la logística.
4.  **Calificación Intermedia:** Aunque su calificación de cliente, aceptable, no es tan destacada como para justificar su menor rendimiento en ingresos.

---

## CONCLUSIÓN ✨

En conclusión, la **Tienda 4** exhibe la **mayor debilidad financiera** y el **menor potencial de crecimiento aparente** dadas las métricas actuales. Vender esta tienda permitiría al Sr. Juan **optimizar su cartera de negocios**, liberando recursos para una inversión estratégica más prometedora que no esté lastrada por un desempeño inferior.

---

## Cómo Ejecutar este Proyecto 🚀

Para replicar este análisis:

1.  **Clona este repositorio:** `git clone https://m.youtube.com/watch?v=KrJwqsuhZ8U&pp=0gcJCYUJAYcqIYzv`
2.  **Abre el archivo `.ipynb`** (cuaderno de Jupyter) en Google Colab.
3.  **Ejecuta las celdas** de código en orden. Asegúrate de tener conexión a internet para que Pandas pueda cargar los datos desde las URLs proporcionadas.

## Agradecimientos 🙏

Un agradecimiento especial a **Alura Latam** y al programa **Oracle Next Education** por proporcionar este desafiante y enriquecedor proyecto que ha permitido aplicar y practicar habilidades clave en Data Science.
