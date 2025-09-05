# SQLab: SQL para Investigación Científica 🔬

Un taller introductorio a SQL enfocado en la manipulación y análisis de datos de física de partículas. Este repositorio contiene el material de apoyo para el taller, utilizando datos de colisiones del detector ATLAS del CERN.

-----

### 📚 Temas del Taller

En este taller, cubrimos los conceptos esenciales de SQL para que te sientas cómodo trabajando con bases de datos relacionales.

  * **Fundamentos de SQL:** Anatomía de una *query* y el orden de ejecución.
  * **Filtrado de datos (`WHERE`):** Cómo seleccionar filas que cumplen con una condición.
  * **Agregación y Agrupación (`GROUP BY`):** Resumir y analizar datos con funciones como `COUNT()`, `AVG()`, y `SUM()`.
  * **Unión de Tablas (`JOINs`):** Combinar datos de múltiples tablas basándose en una columna común.
  * **Subconsultas (`Subqueries`):** Realizar consultas más complejas dentro de otras consultas.

-----

### 🚀 Cómo Usar Este Repositorio

Para ejecutar el taller, necesitas tener instalado Python y conectarte a una base de datos MySQL.

#### Requisitos

  * **Python 3.x**
  * **Librería de conexión a MySQL:** `mysql-connector-python`
  ##### Requisito extra para ejecutar local
  * Docker CLI instalados y la imagen de MySQL:8.0

#### Pasos

1.  **Clonar el repositorio**

    ```bash
    git clone https://github.com/PabloNatB/SQLab.git
    cd SQLab
    ```

2.  **Instalar las dependencias de Python**

    ```bash
    pip install mysql-connector-python jupyter
    ```

3.  **Configurar la conexión a la base de datos**

    Abre el archivo `SQLab queries basicas.ipynb` en tu editor de código o Jupyter Notebook. En la celda de conexión, reemplaza los valores de `<user>`, `<pwd>`, y `<host address>` con tus propios datos de conexión.

    ```python
    config = {
        'user':"<user>", 
        'password':"<pwd>", 
        'host':"<host address>", 
        'port':3306, 
        'database':"particles"
    }
    ```

4.  **Ejecutar el taller**

    Inicia el Jupyter Notebook en tu terminal y abre el archivo `.ipynb`.

    ```bash
    jupyter notebook
    ```

    Sigue las instrucciones en el notebook, ejecuta las celdas de código y completa los retos.

-----

### 📊 Datos Usados

Los datos utilizados en este taller son una versión simplificada de un conjunto de datos de colisiones de alta energía, simulando información de un experimento real.

  * **Referencia:** ATLAS collaboration (2025). ATLAS ROOT ntuple format Run 2 2015+2016 proton-proton collision data beta release, 2J2LMET30 skim. CERN Open Data Portal. DOI:10.7483/OPENDATA.ATLAS.0CJR.N7ZT

-----

### ✍️ Autor

  * **Nombre:** Pablo Natera Bravo
  * **LinkedIn:** [Pablo Natera](www.linkedin.com/in/pablo-natera-464531299)

-----

### 📄 Licencia

Este proyecto está bajo la Licencia MIT.