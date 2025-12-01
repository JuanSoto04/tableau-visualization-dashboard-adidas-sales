# **Resumen Ejecutivo**
Este proyecto consiste en una solución de Inteligencia de Negocios (BI) End-to-End diseñada para analizar el rendimiento comercial de Adidas en Estados Unidos. El objetivo principal fue transformar datos transaccionales crudos en insights accionables para optimizar estrategias de venta omnicanal.

El dashboard permite a los gerentes de ventas y ejecutivos identificar rápidamente cuellos de botella en la rentabilidad y oportunidades de expansión geográfica, respondiendo preguntas clave sobre dónde, qué y cómo se vende mejor.

# **Enlaces al Dashboard Interactivo**
Para experimentar la interactividad completa (filtros, tooltips y navegación), visita las versiones en vivo:

👉 Ver en Tableau Public: [[DASHBOARD VENTAS ADIDAS]](https://public.tableau.com/app/profile/juan.pablo.soto/viz/EntregaFINALSoto/Portada)

# **Hallazgos Clave (Insights)**
Tras el análisis de los datos transaccionales, se detectaron patrones cruciales para la toma de decisiones:

* Rentabilidad por Categoría: Se descubrió que, aunque el volumen de ventas es alto en diversas categorías, las líneas masculinas generan un margen de ganancia superior en comparación con las femeninas.
* Dominio del Retailer: El minorista "West Gear" se posicionó como el socio comercial líder en volumen de ventas, sugiriendo la necesidad de programas de fidelización B2B específicos para este cliente.
* Estrategia de Canales: Se evidenció una discrepancia entre volumen y margen según el método de venta (Online vs. In-Store), permitiendo ajustar la inversión en marketing digital hacia las regiones con mayor conversión online.

# **Aspectos Técnicos Destacados**
Este proyecto destaca por integrar diseño de interfaz (UI) con lógica de datos avanzada:

  1. **Diseño UI/UX con Figma**:
  En lugar de usar la interfaz nativa estándar, se diseñó un sistema de fondos y botoneras en Figma para emular una experiencia de aplicación web (App-like navigation). Esto mejora la adopción del usuario final al hacer la navegación intuitiva entre "Vista General", "Regiones" y "Minoristas".
  2. **Parámetros Dinámicos y Lógica Condicional**:
  Se implementó una lógica de visualización dinámica controlada por el usuario:
  * Color Switching: El dashboard cambia su paleta de colores automáticamente (Verde/Rosa/Neutro) según el género seleccionado en el parámetro, facilitando la distinción visual inmediata.
* Metric Switching: Permite al usuario alternar los gráficos entre Ventas, Ganancias y Margen sin necesidad de duplicar visualizaciones, manteniendo el diseño limpio.

3. **Modelado de Datos (Esquema Estrella)**
Se estructuró un modelo relacional robusto para asegurar el rendimiento del reporte:

*  Tabla de Hechos: Ventas (Transaccional).

*  Dimensiones: Producto, Geografía (Ciudad/Estado/Región), Minorista, Método de Venta.

*  Relaciones: Cardinalidad 1 a Muchos optimizada para filtrado cruzado.

## Stack Tecnológico
* **Visualización & BI**: Tableau.

* **Diseño de Interfaz**: Figma (Prototipado y Assets gráficos).

* **Procesamiento de Datos**: Excel / SQL (Limpieza y estructuración).

* **Fuente de Datos**: Dataset simulado de ventas minoristas Adidas (US Market).
