# Observaciones preliminares

- Para poder realizar esta tarea van a tener que tener ya instalados OpenFOAM v10 y Paraview
- Apoyarse sin miedo tanto en el foro de consultas del Classroom como en chats de inteligencias artificiales (ChatGPT, Gemini, etc) al no saber como continuar en algún punto (siempre responsablemente con el objetivo de aprender y no de que la IA nos haga la modificación por nosotros.

# Tarea Clase 2 - Introducción a OpenFOAM v10

## 1 - Copiar archivos a una carpeta de trabajo.

Vamos a utilizar los carpetas de los tutoriales vistos durante la clase cavity o Square bend liq (Elegir uno a gusto). Que estan en las carpetas:

- `cavity`: `/opt/openfoam10/tutorials/incompressible/icoFoam/cavity/cavity`
- `Square bend liq`: `/opt/openfoam10/tutorials/compressible/rhoSimpleFoam/squareBendLiq`

*Observación*:

*El tutorial `Square bend liq` es mas complicado que el `cavity` ya que tenemos un campo mas y por defecto viene con el modelo de turbulencia RAS*.

## 2 - Realizar una corrida con el tutorial así como está.

Realizar una ejecución del caso tutorial según los comandos vistos en clase. 

(En esta parte no deberíamos ver fallas ni problemas, salvo que nos equivoquemos de comandos).

## 2 - Realizar una modificación en una condición de contorno

Modificar alguna de las condiciones de contorno de la simulación (aumentando o disminuyendo la velocidad, la presión, la temperatura). Elegir alguna a conciencia y modificar su valor con **cuidado**.

Luego realizar una corrida del caso tutorial nuevamente y visualizar los datos en Paraview del campo de presiones y velocidades.

Posteriormente exportar una imagen de sus mapas de presión y velocidad como .png desde Paraview.

## 3 - Modifcar el blockMesh del caso tutorial

Tomar la geometria inicial (que está en blockMesh) y modificarla. Tomar alguna de sus dimensiones (en x, y o z) y hacerla mas grande (por ejemplo en X si corresponde). Luego también agregar mas celdas en la dimensión que volvimos mas grande. Por ejemplo:

Si a un tubo rectangular lo volvimos mas grande en la dimensión X, deberemos agregar mas celdas en esa dimensión tambien para que la simulación sea consistente.

Luego de esto, simular nuevamente y posteriormente exportar una imagen de sus mapas de presión y velocidad como .png desde Paraview.

## 4 - (Opcional) para el caso `Square bend liq`

Modificar el modelo de transporte de momento, de turbulento a laminar y analizar los mapas de presión y temperatura. 
1. ¿Cambian en algo sus mapas?
2. ¿Sus residuos son iguales?
3. Si tengo la turbulencia "activada", ¿La simulación tarda mas o menos?.
