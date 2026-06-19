# Análisis de Ventas y Rendimiento de Productos - Juegos de Mesa 🎲📊

Este proyecto consiste en un análisis de datos interactivo desarrollado en **Tableau** enfocado en el rendimiento comercial, la gestión de inventario y la logística de envíos para una categoría de juegos de mesa. El objetivo es transformar datos operativos en decisiones estratégicas de negocio.

## 🔗 Acceso al Dashboard Interactivo
Podés interactuar con los filtros y visualizar el proyecto completo en tiempo real en Tableau Public:
👉 [Ver Proyecto en Tableau Public](https://public.tableau.com/app/profile/oriana.daniela.moragues/viz/EntregaFinalMoragues/Dashboard1#1b)

---

## 📈 Estructura y Componentes del Análisis

### 1. Resumen de Ventas y Rendimiento de Productos
Este tablero ofrece una visión global y macro del negocio, permitiendo identificar rápidamente los ingresos, volúmenes de venta y la rentabilidad geográfica.

* **Objetivo:** Monitorear los principales KPIs de ingresos y volumen físico vendidos.
* **Métricas Clave:** Unidades vendidas, ingresos totales, ganancias totales y volumen de juegos analizados.
* **Visualizaciones Incluidas:**
  * Análisis de dispersión de Ganancia por cada venta.
  * Matriz de calor regional (Capital Federal, Gran Buenos Aires e Interior) cruzada por Tienda Oficial.
  * Gráfico de barras horizontales con el Top de productos por ganancia generada.
  * Gráfico de doble eje para la relación de precios por juego.
* **Filtros Activos:** Tienda Oficial.

Dashboard1.png

---

### 2. Análisis de Envío - Publicación - Reputación
Este tablero profundiza en la eficiencia logística y en cómo las condiciones de publicación y la reputación del vendedor impactan de manera directa en el comportamiento de la demanda.

* **Objetivo:** Evaluar el impacto de los tipos de envío (Gratis, Flex, Full) y los tiempos de exposición en el éxito de las ventas.
* **Métricas Clave:** Distribución porcentual de envíos y mediana de días de publicación.
* **Visualizaciones Incluidas:**
  * Gráfico de dona para la proporción de Envío Gratis (Sí / No).
  * Panel de control de stock y reglas lógicas de decisión ("Prioridad por stock" / "No ofrecer producto").
  * Gráfico combinado de barras y líneas para evaluar la Mediana de Días publicados vs. Unidades vendidas.
  * Gráfico de burbujas (Packed Bubbles) para segmentación de ventas según niveles de Reputación (Gold, Líder, Platinum).
* **Filtros Activos:** Nombres de Juegos de Mesa, Ubicación (Regiones).

![Dashboard 2 - Análisis Logístico](dashboard2.jpg)

---

## 🛠️ Desarrollo Técnico y Campos Calculados
Para estructurar, limpiar y enriquecer los datos originales dentro de Tableau, se diseñaron e implementaron los siguientes campos calculados avanzados:

* **Limpieza de Cadenas:** `Investiga1` y `Nombres Juegos Mesa` (utilizando funciones `REPLACE` y `SPLIT` para optimizar las etiquetas de texto en las visualizaciones).
* **Lógica de Negocio:** `Prioridad por stock` (función condicional `IF` para determinar automáticamente la disponibilidad estratégica de los productos).
* **Estandarización:** `Tienda Oficial` y `ubicacion2` (estructuras `CASE` y `REPLACE` para unificar criterios geográficos y de sucursales).
* **Alertas Visuales y Métricas Avanzadas:** `KPI-COLOR` (condicionales orientados al formato visual según rendimiento) y `WINDOWS_AVG` (cálculos de agregación de ventana).
* **Estética:** Aplicación de paleta cromática profesional e integrada utilizando Coolors.co.
## 🛠️ Aspectos Técnicos y Campos Calculados
Para lograr la segmentación y optimización de las vistas visuales, se desarrollaron las siguientes funciones lógicas y de texto:
* `Investiga1` y `Nombres Juegos Mesa`: Funciones de cadena (`REPLACE`, `SPLIT`) para la limpieza y mejora visual de etiquetas.
* `Prioridad por stock`: Función lógica `IF` para determinar la estrategia de oferta de productos.
* `Tienda Oficial`: Expresiones `CASE` para estandarizar nombres de sucursales.
* `KPI-COLOR` y `WINDOWS_AVG`: Cálculos avanzados y de ventana para alertas visuales de rendimiento.
* **Diseño:** Paleta de colores personalizada extraída de Coolors.co.
