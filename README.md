[![Open in MATLAB Online](https://www.mathworks.com/images/responsive/global/open-in-matlab-online.svg)](https://matlab.mathworks.com/open/github/v1?repo=l20211610-svg/MMP2)

# Práctica 2 — Avanze de simulaciones

Repositorio académico de la asignatura **Modelado Matemático**, correspondiente a la **Maestría en Ciencias de la Ingeniería** del Tecnológico Nacional de México / Instituto Tecnológico de Tijuana. La práctica integra modelado mecanicista, análisis cualitativo de sistemas dinámicos no lineales, estimación de parámetros, simulación numérica y experimentación *in silico* en MATLAB y Simulink.


**Docente:** Dr. Paul Antonio Valle Trujillo  
**Departamento:** Ingeniería Eléctrica y Electrónica  
**Institución:** Tecnológico Nacional de México / Instituto Tecnológico de Tijuana  
**Asignatura:** Modelado Matemático  
**Programa:** Maestría en Ciencias de la Ingeniería

**Alumno:** Ing. Ariel Isai Perez Manzano

---


---

<a id="resumen"></a>
## Resumen

Esta práctica estudia un problema inverso sencillo basado en el modelo presa–depredador de Lotka–Volterra. A partir de datos históricos digitalizados manualmente, se estiman los parámetros cinéticos del sistema mediante **regresión no lineal por mínimos cuadrados** con `fitnlm`. Para cada evaluación del modelo durante el ajuste, las ecuaciones diferenciales se resuelven numéricamente mediante el **método de Heun** con paso de integración fijo.

Posteriormente se analiza la dinámica del sistema mediante soluciones temporales y trayectorias en el plano de fase, se calculan sus puntos de equilibrio y se estudia su estabilidad local a partir de la matriz Jacobiana. Finalmente, las soluciones se comparan empleando diferentes solvers de MATLAB y Simulink, incluyendo métodos para sistemas *stiff*, *nonstiff* y de paso fijo.

**Palabras clave:** ecuaciones diferenciales ordinarias; estimación de parámetros; Lotka–Volterra; MATLAB; métodos numéricos; modelo mecanicista; regresión no lineal; sistemas dinámicos no lineales.

[Volver al contenido](#contenido)

---

<a id="objetivos"></a>
## Objetivos

### Objetivo general

Aplicar herramientas de modelado matemático, análisis de sistemas dinámicos y simulación computacional para estudiar la interacción presa–depredador descrita por el sistema de Lotka–Volterra a partir de datos históricos de liebres y linces.

### Objetivos específicos

- Digitalizar y organizar los registros experimentales como series de tiempo.
- Procesar los datos mediante suavizado y normalización.
- Estimar los parámetros \($\alpha$), \($\beta$), \($\delta$) y \($\gamma$) mediante regresión no lineal.
- Calcular estadísticos de los parámetros y criterios de bondad de ajuste.
- Resolver numéricamente el sistema mediante el método de Heun.
- Comparar diferentes solvers de MATLAB y Simulink.
- Construir las soluciones temporales y el plano de fase.
- Calcular los puntos de equilibrio y analizar su estabilidad local.
- Relacionar el análisis matemático con los resultados obtenidos mediante experimentación *in silico*.

[Volver al contenido](#contenido)

---

<a id="datos"></a>


---

## Uso académico

Este repositorio se utiliza con fines docentes en la asignatura **Modelado Matemático** de la **Maestría en Ciencias de la Ingeniería**. El cuaderno computacional debe complementarse con la interpretación matemática y física de los resultados; la ejecución del código por sí sola no sustituye el análisis del sistema dinámico.
