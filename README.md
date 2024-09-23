# Proyecto Series de Tiempo - Análisis Predictivo Avanzado

Este proyecto fue desarrollado como parte de la materia **Análisis Predictivo Avanzado** en la facultad. En él, analizamos un conjunto de datos de la ciudad de Tetuán, situada en el norte de Marruecos, con el propósito de estudiar las relaciones entre las **variables ambientales** (temperatura, humedad, presión atmosférica) y el **consumo de energía** en tres zonas específicas de la ciudad: **Quads**, **Smir** y **Boussafou**.

## Análisis Realizado

### 1. Descomposición de series temporales
Identificamos los siguientes componentes en las series temporales:

- **Tendencia**: Evolución a largo plazo de los datos.
- **Estacionalidad**: Patrones repetitivos a lo largo del tiempo, que se observan en intervalos regulares.
- **Componente aleatoria**: Variaciones no explicadas por los demás componentes.
- **Ciclos**: Fluctuaciones que ocurren en intervalos no fijos.

### 2. Análisis de estacionalidad
Realizamos un análisis detallado de la estacionalidad utilizando las siguientes técnicas:

- **Autocorrelación (ACF)**: Mide la correlación entre una variable y sus valores rezagados.
- **Autocorrelación parcial (PACF)**: Mide la correlación entre una variable y sus valores rezagados después de eliminar el efecto de otros retardos.
- **Test de Dickey-Fuller aumentado (ADF)**: Aplicamos el test en su versión sin diferenciar y diferenciada para verificar la **estacionariedad** de las series temporales.

### 3. Modelos aplicados
Desarrollamos y ajustamos distintos modelos para predecir el consumo energético, teniendo en cuenta las características identificadas en el análisis previo:

- **ARIMA (Autoregressive Integrated Moving Average)**: Modelo utilizado para capturar tanto la autocorrelación como la diferenciación necesaria para que las series sean estacionarias.
- **Tendencia cuadrática**: Aplicada para capturar la evolución a largo plazo del consumo, incorporando una curva cuadrática en lugar de una simple línea recta.
- **Transformación logarítmica**: Empleada para estabilizar la varianza y manejar variaciones exponenciales, mejorando así la precisión del modelo.
