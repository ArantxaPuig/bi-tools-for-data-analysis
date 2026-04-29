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

# 🪜 PASO A PASO DEL PROYECTO EN POWER BI

---

## 1. 📥 Importación de datos

1. Abrir **Power BI Desktop**
2. Click en **Obtener datos**
3. Seleccionar **Excel**
4. Importar el archivo `pokemon_powerbi.xlsx`
5. Seleccionar la hoja correspondiente
6. Pulsar **Cargar**

---

## 2. 🧹 Limpieza de datos (Power Query)

1. Ir a **Transformar datos**
2. Revisar tipos de datos:
   - Texto → Nombre, Tipo
   - Número entero → estadísticas
3. Renombrar columnas si es necesario:
   - `HP` → Vida
   - `Attack` → Ataque
   - `Defense` → Defensa
4. Eliminar duplicados si existen
5. Revisar valores nulos
6. Cerrar y aplicar cambios

---

## 3. 🧠 Modelado de datos

En este caso trabajamos con una sola tabla, pero se revisa:

- Correcta estructura de columnas
- Relación interna si hubiera otras tablas (tipos, generaciones, etc.)
- Organización de campos (numéricos vs categóricos)

---

## 4. 📐 Creación de medidas DAX

Ejemplos de medidas utilizadas:

### 🔢 Total de Pokémon
```DAX
Total Pokemon = COUNTROWS(Pokemon)