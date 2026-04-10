#  Proyecto Fuga de Talento

## Descripción del proyecto

ABC Corporation nos ha encargado el análisis de sus datos de empleados con el objetivo de identificar los factores que influyen en la rotación de empleados.

Este proyecto tiene como finalidad transformar datos en información útil para la toma de decisiones estratégicas, ayudando a mejorar la retención y optimizar la gestión del talento.

---

## 🧱 Fases del proyecto
🔍 Fase 1: Análisis Exploratorio de Datos (EDA)

Se ha realizado un análisis inicial del dataset para comprender:

* Estructura de los datos
* Tipos de variables
* Valores nulos
* Distribución de variables
  
---

## 🔧 Fase 2: Transformación de datos

En esta fase se ha trabajado en la limpieza y preparación de los datos:

* Tratamiento de valores nulos (mediana, moda, categoría "unknown")
* Conversión de tipos de datos
* Homogeneización de variables categóricas
* Corrección de errores en variables

---

## 📊 Fase 3: Visualización de datos

Se han desarrollado diferentes visualizaciones para analizar el comportamiento de los empleados y detectar patrones relevantes.

Las visualizaciones han permitido identificar:

* Factores clave de abandono
* Áreas de mejora dentro de la empresa
* Variables con mayor impacto en la rotación

### 📊 Principales insights

🔥 Rotación de empleados
Aproximadamente un 16% de los empleados abandona la empresa

💰 Salario
Los empleados con menores salarios presentan mayor abandono

😞 Satisfacción laboral
La baja satisfacción está directamente relacionada con el abandono

⏰ Horas extra
Los empleados que realizan horas extra tienen mayor probabilidad de abandonar

⏳ Antigüedad
El abandono se concentra en los primeros años en la empresa

🏢 Departamentos
Sales presenta la mayor tasa de abandono (~20%)
Human Resources también muestra una tasa elevada
Research & Development es el más estable

🎓 Formación
No se observa una relación clara entre formación y abandono

🧠 Conclusión
La rotación de empleados es un fenómeno multifactorial que depende de variables económicas, laborales y emocionales.
Los factores más relevantes identificados han sido:
* Salario
* Satisfacción laboral
* Carga de trabajo

🚀 Recomendaciones

* Revisar la política salarial
* Mejorar la satisfacción laboral
* Reducir la carga de trabajo y horas extra
* Reforzar el onboarding
* Analizar en profundidad el departamento de Sales

---

## Fase 4: Diseño de BBDD e Insercción de los Datos.

# Proyecto de carga de empleados a MySQL

Este proyecto toma un archivo CSV con información de empleados, lo carga en un DataFrame de pandas y lo inserta en una base de datos MySQL con una estructura relacional normalizada.

## Descripción

El script realiza las siguientes tareas:

- Importa librerías necesarias para trabajar con MySQL y análisis de datos.
- Carga el archivo `empleados_abc_limpio.csv`.
- Verifica visualmente los datos con ejemplos del inicio, final y muestras aleatorias.
- Guarda una copia del CSV como `abc_limpio_ok.csv`.
- Se conecta a un servidor MySQL.
- Crea un esquema para la empresa.
- Genera varias tablas relacionadas.
- Inserta los datos del CSV en las tablas correspondientes.

## Tecnologías usadas

- Python 3
- pandas
- numpy
- mysql-connector-python
- MySQL

## Estructura de datos

El dataset contiene información de empleados, como por ejemplo:

- edad
- abandono de la empresa (`attrition`)
- tipo de viaje de negocios
- departamento
- nivel educativo
- género
- rol de trabajo
- estado civil
- ingresos mensuales
- satisfacción laboral
- balance vida-trabajo
- años en la empresa
- años con el manager actual

## Archivos esperados

Esquema de base de datos

El código crea las siguientes tablas:

1. departments

Guarda los departamentos únicos de la empresa.

Campos:

department_id
department_name
2. job_roles

Guarda los roles de trabajo únicos.

Campos:

job_role_id
role_name
3. employees

Guarda la información básica del empleado.

Campos:

employee_number
age
gender
marital_status
education
4. employee_finance_details

Guarda información financiera y la relación con departamento y rol.

Campos:

finance_id
employee_number
monthly_income
over_time
department_id
job_role_id
5. employee_career_path

Guarda la evolución profesional del empleado dentro de la empresa.

Campos:

career_path_id
employee_number
years_at_company
years_in_current_role
years_since_last_promotion
years_with_curr_manager
total_working_years
6. employee_satisfaction

Guarda métricas de satisfacción del empleado.

Campos:

survey_id
employee_number
environment_satisfaction
job_satisfaction
relationship_satisfaction
work_life_balance
Flujo del proceso
1. Carga del CSV

Mejoras futuras

Algunas mejoras recomendables para este proyecto:

usar variables de entorno para la contraseña
separar el código en archivos .py
añadir validaciones de datos antes de insertar
registrar logs del proceso
usar transacciones controladas
crear claves únicas adicionales donde sea necesario
documentar mejor el diccionario de datos

---

## Fase 5: Presentación Visual

La última fase consistió en una presentación visual de los resultados obtenidos, creada en unas diapositivas, donde se resumen los hallazgos más relevantes mediante un diagrama, tablas y visualizaciones de imagenes que facilitan la comprensión del análisis realizado.

---

## Tecnologías Utilizadas


![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)![Pandas](https://img.shields.io/badge/pandas-%23150458.svg?style=for-the-badge&logo=pandas&logoColor=white) ![MySQL](https://img.shields.io/badge/mysql-4479A1.svg?style=for-the-badge&logo=mysql&logoColor=white) ![Jupyter Notebook](https://img.shields.io/badge/jupyter-%23FA0F00.svg?style=for-the-badge&logo=jupyter&logoColor=white) 

![Visual Studio Code](https://img.shields.io/badge/Visual%20Studio%20Code-0078d7.svg?style=for-the-badge&logo=visual-studio-code&logoColor=white)  ![Canva](https://img.shields.io/badge/Canva-%2300C4CC.svg?style=for-the-badge&logo=Canva&logoColor=white)

![Matplotlib](https://img.shields.io/badge/Matplotlib-ffffff?style=for-the-badge&logo=matplotlib&logoColor=black)
![Seaborn](https://img.shields.io/badge/Seaborn-2E8B57?style=for-the-badge)

---

## Instrucciones de uso

1. Clona el repositorio
2. Ejecuta el archivo principal: `limpieza_abc.ipynb`
3. Sigue las instrucciones en el archivo .


---

## Estructura del repositorio
```
da-project-promo-63-modulo-3-team-3/

├── data/
│   ├── hr.csv
│   └── empleados_limpio.csv
├── notebooks/
│   ├── limpieza_abc.ipynb
│   └── visualizacion.ipynb
├── README.md

```

---

## Autoras

[Estefanía Moreno Delmo](https://github.com/fany-data)

[Katyah Uba](https://github.com/katyakuba)

[Natalia Pozo](https://github.com/nataliapozoaraque-hash)

[Esther Gil](https://github.com/Esther-GIL)

[Carlota](https://github.com/ezcarlota)


---

## Estado del proyecto

    Version beta finalizada
---

