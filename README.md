# Proyecto RappiPlus: De Datos a Decisiones de Negocio

## 📌 1. Introducción y Contexto del Negocio
RappiPlus es el servicio de suscripción premium dentro del ecosistema de Rappi, diseñado estratégicamente para incrementar la frecuencia de compra, optimizar el ciclo de vida del usuario y maximizar el valor económico generado por cliente (Customer Lifetime Value). 

A pesar de su propuesta de valor, el equipo directivo requería certificar si el modelo actual estaba cumpliendo con sus objetivos de rentabilidad, en qué etapas del proceso de compra existían pérdidas de conversión y si las últimas modificaciones de producto realmente generaron un impacto positivo. Este proyecto aborda de manera integral estas dudas mediante un análisis de datos estructurado de extremo a extremo.

---

## 💡 2. Preguntas Clave del Negocio
* **Calidad:** ¿Podemos confiar plenamente en las bases de datos transaccionales antes de tomar decisiones?
* **Rentabilidad:** ¿El modelo de suscripción está generando ganancias reales o absorbiendo costos excesivos?
* **Embudo de Conversión:** ¿En qué pasos del proceso de compra se detectan los mayores puntos de abandono (*drop-off*)?
* **Retención:** ¿Los usuarios de RappiPlus regresan de manera recurrente o abandonan la plataforma en el tiempo?
* **Experimentación:** ¿Los cambios recientes implementados en el producto generaron un impacto estadísticamente significativo?

---

## 🛠️ 3. Estructura Analítica y Herramientas Utilizadas
El análisis se ejecutó siguiendo un flujo modular donde cada etapa aportó una capa de validación para la toma de decisiones:

* **Etapa 1: Calidad de Datos (Python):** Evaluación, limpieza y estructuración de tres datasets crudos (pedidos, catálogo y marketing) utilizando `Pandas` y `NumPy` en Jupyter Notebook para eliminar inconsistencias y asegurar datos confiables.
* **Etapa 2: Rentabilidad del Negocio (Python):** Modelado financiero y cálculo de KPIs clave (ingresos/revenue, costos operativos y ganancias netas) para la identificación de segmentos de usuarios rentables.
* **Etapa 3: Funnel de Conversión (SQL):** Análisis detallado del recorrido del usuario para identificar las etapas críticas de abandono y determinar con precisión el mayor *drop-off* en el proceso de compra.
* **Etapa 4: Análisis de Retención por Cohortes (SQL):** Construcción de matrices de cohortes para evaluar el comportamiento longitudinal de los suscriptores y monitorear la tasa de recurrencia en el tiempo.
* **Etapa 5: Evaluación de Impacto / Experimentación A/B (Python):** Aplicación de pruebas estadísticas inferenciales para evaluar si los cambios en el producto generaron un impacto real en las métricas de negocio.
* **Etapa 6: Dashboard Ejecutivo y Comunicación (Tableau):** Diseño de un sistema visual interactivo orientado a la experiencia del usuario operativo y directivo para centralizar los hallazgos y KPIs en tiempo real.

---

## 📊 4. Hallazgos Principales e Impacto Operativo
* **Validación de Confianza:** Se estandarizaron las bases transaccionales primarias, garantizando que la dirección cuente con reportes libres de sesgo por datos duplicados o nulos.
* **Optimización de la Conversión:** La detección analítica del mayor punto de abandono (*drop-off*) en el funnel de compra permitió proponer acciones concretas de rediseño de interfaz, minimizando la fricción en el checkout del usuario.
* **Estrategia basada en Evidencia:** La combinación de pruebas de hipótesis estadísticas (A/B Testing) y análisis de cohortes en SQL blindó la toma de decisiones comerciales, asegurando que los recursos de marketing se enfoquen en los segmentos y cambios de producto de mayor rentabilidad demostrada.

---

## 📦 5. Entregables del Repositorio
* `RappiPlus_Data_Quality_and_Experimentation.ipynb`: Código en Python enfocado en limpieza de datos, rentabilidad y pruebas estadísticas A/B.
* `RappiPlus_Queries_Funnel_Cohortes.sql`: Consultas optimizadas en SQL para la extracción de embudos y matrices de retención.
* `Enlace a Tableau Public`: *(Opcional: puedes pegar aquí el link de tu dashboard interactivo para que lo vean en vivo)*.
