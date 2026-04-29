# 📊 Pokémon BI Dashboard with Power BI

Proyecto de análisis de datos y Business Intelligence desarrollado con **Power BI**, utilizando una base de datos de Pokémon como caso práctico.

El objetivo del proyecto es demostrar cómo transformar datos en información visual útil mediante procesos reales de **Explorar Dataset en Excel, modelado de datos, métricas DAX y dashboards interactivos**.

---

# 🚀 Objetivos del Proyecto

- Importar datos desde Excel
- Limpiar y transformar datos con Power Query
- Crear un modelo de datos eficiente
- Diseñar medidas DAX dinámicas
- Construir un dashboard visual e interactivo
- Extraer conclusiones a partir de los datos

---

# 📁 Dataset Utilizado

Archivo base:

`pokemon_powerbi.xlsx`

Contiene información como:

- Nombre del Pokémon
- Tipo principal
- Tipo secundario
- HP
- Ataque
- Defensa
- Velocidad
- Estadísticas totales
- Legendario
- Generación

---

# 🛠️ Herramientas Utilizadas

- Power BI Desktop
- Power Query
- DAX (Data Analysis Expressions)
- Microsoft Excel
- GitHub

---

# 📌 Proceso del Proyecto

## 1️⃣ Carga de Datos

Se importó el archivo Excel en Power BI mediante:

`Inicio > Obtener datos > Excel`

---

## 2️⃣ Transformación de Datos (Power Query)

Se realizaron tareas de limpieza como:

- Renombrado de columnas
- Corrección de tipos de datos
- Eliminación de duplicados
- Gestión de valores nulos
- Validación de consistencia

---

## 3️⃣ Modelado de Datos

Se trabajó con una tabla principal optimizada para análisis.

En futuras versiones se puede evolucionar a modelo estrella con tablas dimensión.

---

## 4️⃣ Métricas DAX

Ejemplos de medidas creadas:

```DAX
Total_Pokemon = COUNTROWS(Pokemon)

Promedio_Ataque = AVERAGE(Pokemon[Ataque])

Legendarios =
CALCULATE(
    COUNTROWS(Pokemon),
    Pokemon[Legendary] = TRUE()
)