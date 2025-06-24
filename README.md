# Orbiting satellites Data Analysis

<img src="https://github.com/user-attachments/assets/2e6bba7c-ecc8-49a1-82f5-60e3fea7cdcf" alt="Satelite" width="200" height="200">
<img src="https://github.com/user-attachments/assets/11429b53-df0b-40a4-b1d1-fc897b27e425" alt="Launch" width="100" height="120">

## Satélites en órbita sobre la Tierra

<img src="https://github.com/user-attachments/assets/45c87350-ca65-421f-9743-7f837b84c4de" alt="Union of Concerned Scientist" width="200" height="80">

#### Union of Concerned Scientist Satellite Database
Fecha de actualización: 01/01/2023

Referencia
“UCS-Satellite-Database-1-1-2023”. By UCS, Teri Grimwood, Tom Z. Collina, Dr. Alvin M. Saperstein, Dr. Jonathan McDowell. 
Acceso a través de www.ucsusa.org/satellite_database


## Introducción

En este proyecto abordaremos el análisis de los datos ofrecidos por la UCS
con tal de extraer información de relevancia sobre la mayoría de satélites
artificiales que se encuentren activos (con capacidad de maniobrar y de
establecer comunicación) a la última fecha de actualización de este dataset (1-
1-2023).

Se convertirá el conjunto de datos a  tablas epara realizar consultas y gestionar la base de datos.
Se utilizará PowerBI para representar esos datos y visualizar.

## Objetivos

Análisis descriptivo de los datos relevantes sobre los satélites en órbita activos y sus características, para a través de una visualización y representación de los datos (gráficos, tablas), facilitar la comprensión y poder medir su evolución a través del tiempo y posibles tendencias. 
A través del análisis de estos datos se puede recuperar información que podría ser de valor para implementar mejoras futuras que favorecerían en el ámbito de la ciencia, tecnología y sustentabilidad ambiental.

---

## Tabla de contenidos         Página

1. Introducción
  - Descripción de la temática
  - Herramientas utilizadas
  - Tabla de versiones
2. Base de datos
  - SQL
  - Diagrama Entidad – Relación
  - Listado de tablas
  - Descripción de columnas por tabla
3. Objetivos y aplicación
  - Hipótesis
  - Alcance y nivel de aplicación
  - Medidas utilizadas
4. Dashboard PowerBI
5. Diagrama Entidad-Relación dentro de PowerBI.
6. Conclusión
7. Futuras líneas

---

## Contenido del dataset (dividido en tablas):

### Descripción de columnas por tabla
###Tablas:
#### 1- Satélite

**COSPAR_ID** :	Número de identificación Internacional de objetos en el espacio.</br>
**Name of Satellite** :	Nombre común del satélite.</br>
**NORAD_ID** :	Número de identificación del comando aeroespacial de USA.</br>
**Operator/Owner** :Actual operador del satélite o dueño (puede ser alquilado).</br>
**Official** : Name	Nombre oficial del satélite</br>
**Date of Launch** : Fecha de lanzamiento a órbita</br>
**Launch Vehicle** :	Vehículo de propulsión en el que fue puesto en órbita</br>
**Expected Lifetime (yrs.)** :	Expectativa de vida útil del satélite.</br>
**Launch Mass (kg.)** :	Masa del satélite al momento del lanzamiento. Incluye combustible</br>
**Dry Mass (kg.)** :	Masa del satélite sin tener en cuenta combustibles.</br>
**Power (watts)** : 	Energía eléctrica que produce el satélite. Varía a lo largo del tiempo</br>

**Class of Orbit**: Clase de órbita:
  - Casi circular (Low earth orbit (LEO), médium earth (MEO) o geosíncrona (GEO). 
  - Elíptica</br>
  
**Type of Orbit** :	Tipo de órbita:
  - Casi circulares: Equatorial—órbita ecuatorial baja, con una inclinación entre 0º y 20º.
  - Nonpolar Inclined: órbita baja-media con una inclinación entre 20º y 85º.
  - Polar: órbita baja polar, inclinación entre 85º y 95º y mayor que 104º.
  - Sun-synchronous: órbita baja sincronizada al sol, con una inclinación entre 95º y 104º.</br>
  - 
**Longitude of GEO (degrees)** : 	Longitud de la tierra donde el satélite se mantiene (para satélites geosíncronos) (Positivo en longitud este del 0º meridiano de Greenwich, y negativo en longitud oeste).</br>
**Perigee (km)** :	Punto más cercano del satélite en altitud con respecto a la tierra</br>
**Apogee (km)	** : Punto más lejano del satélite en altitud con respecto a la tierra</br>
**Eccentricity** : 	Excentricidad de la órbita (que tanto se desvía la órbita de ser un círculo).</br>
**Inclination (degrees)** : 	Angulo de inclinación entre el ecuador de la tierra y el plano orbital.</br>
**Period (minutes)** : 	Tiempo en el que el satélite da una órbita a la tierra.</br>


#### 2- Operador
**Country of Operator/Owner** :	País donde está establecido el operador o dueño.</br>
**Contractor** :	Contratista que se encargó de la construcción del satélite</br>
**Country of Contractor** : País donde está establecido el contratista.</br>

#### 3- País
**Country/Org of UN Registry** : País responsable registrado ante el registro de objetos espaciales de las Naciones Unidas.</br>
**Launch Site** : Lugar de lanzamiento.</br>

#### 4- Propósito
**Users** : 	Usuarios que utilizan el satélite. Comercial, civil, gobierno (científico, meteorológico), militar.</br>
**Purpose** : 	Categoría de propósito del satélite. Auto-reportado.</br>
**Detailed Purpose** : Propósito detallado de la finalidad del satélite.</br>
**Comments** : 	Comentarios con información adicional.</br>
