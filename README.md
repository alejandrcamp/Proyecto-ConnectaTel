# Proyecto-ConnectaTel

## Objetivo
Analizar el comportamiento de los clientes de ConnectaTel, una empresa de telecomunicaciones en Latinoamérica. El objetivo es limpiar y explorar la información para detectar comportamientos atípicos (outliers), segmentar a los clientes y generar recomendaciones accionables para mejorar la oferta actual de planes y experiencia del usuario.

## Dataset
Se utilizaron 3 datasets: 
- plans.csv, el cual contenia la 	información de los planes actuales
- users_latam.csv con la información de los clientes
- usage.csv con detalle del uso real del servicio (llamadas y mensajes)

## 🧩 Etapas del análisis
- Carga y exploración — lectura de los 3 datasets y revisión de estructura 
- Identificación de problemas de calidad de datos — detección de nulos, valores sentinel 
- Limpieza de datos — imputación de sentinels, tratamiento de nulos y corrección de fechas imposibles.
- Construcción del perfil de usuario — agregación del uso por user_id y combinación con users.
- Estadística descriptiva y visualización — histogramas de edad y variables de uso, segmentados por plan.
- Detección de outliers — boxplots y cálculo de límites con el método IQR.
- Segmentación de clientes — por nivel de uso (grupo_uso) y por edad (grupo_edad), con countplots de distribución.
- Insight ejecutivo — síntesis de hallazgos y recomendaciones de negocio para stakeholders.

## Cómo ejecutar el notebook
- Clona este repositorio.
- Coloca los 3 archivos CSV en una carpeta datasets/ en la raíz del proyecto 
- Abre el notebook con jupyter notebook o jupyter lab y ejecuta todas las celdas en orden.
