# Spin Coater 🌀

Este repositorio ha sido desarrollado como parte del curso de **Proyecto de Instrumentación** y contiene el diseño, construcción y caracterización de un sistema **Spin Coater** para la deposición de películas delgadas sobre sustratos planos.

---

## Problema

¿Es posible desarrollar un Spin Coater de bajo costo capaz de controlar de manera precisa la velocidad de rotación de un sustrato para la fabricación reproducible de películas delgadas?

---

## Marco teórico 📑

El **spin coating** es una técnica utilizada para depositar películas delgadas y uniformes sobre superficies planas.

El proceso consiste en colocar una determinada cantidad de solución sobre un sustrato y hacerlo girar a alta velocidad. Debido al movimiento de rotación, la solución se distribuye radialmente sobre la superficie y el exceso de material es expulsado hacia los bordes.

La calidad y el espesor final de la película dependen de diferentes parámetros del proceso, entre ellos:

- **Velocidad de rotación**
- **Aceleración**
- **Tiempo de rotación**
- **Viscosidad de la solución**
- **Concentración de la solución**
- **Geometría y dimensiones del sustrato**

Para obtener resultados reproducibles es necesario mantener un control adecuado de la velocidad de rotación.

En este proyecto se plantea desarrollar un sistema de control en **lazo cerrado**, donde la velocidad real del motor es medida y comparada con una velocidad de referencia establecida por el usuario.

De forma general, el sistema estará compuesto por:

- Motor eléctrico.
- Sistema de accionamiento del motor.
- Microcontrolador.
- Sistema de medición de velocidad.
- Controlador de velocidad.
- Interfaz de usuario.
- Estructura mecánica y soporte del sustrato.
- Sistema de protección.

El error utilizado por el sistema de control puede expresarse como:

El error utilizado por el sistema de control puede expresarse como:

$$
e(t) = \omega_{ref}(t) - \omega(t)
$$

donde:

- $e(t)$ es el error de velocidad.
- $\omega_{ref}(t)$ es la velocidad angular deseada.
- $\omega(t)$ es la velocidad angular medida.

A partir de este error, el controlador modifica la señal aplicada al sistema de accionamiento con el objetivo de mantener la velocidad del sustrato cercana al valor de referencia.

---

## Integrantes y roles 👷

| Foto | Nombre | Rol |
|---|---|---|
| <img src="Resources/Images/integrante1.jpg" width="150"> | Alexis Calderon Quispe   | Responsable de ... |
| <img src="Resources/Images/integrante2.jpg" width="150"> | Kevin Diaz Colonia       | Responsable de ... |
| <img src="Resources/Images/integrante3.jpg" width="150"> | Cristhoper Yañez Malpica | Responsable de ... |

**Proyecto de Instrumentación - 2026**

---

## Referencias 🔗

[1] D. Carbonell Rubio, W. Weber y E. Klotzsch,  
“Maasi: A 3D printed spin coater with touchscreen,”  
*HardwareX*, vol. 11, e00316, 2022.  
https://doi.org/10.1016/j.ohx.2022.e00316

[2] A. G. Emslie, F. T. Bonner y L. G. Peck,  
“Flow of a viscous liquid on a rotating disk,”  
*Journal of Applied Physics*, vol. 29, pp. 858–862, 1958.

[3] D. Meyerhofer,  
“Characteristics of resist films produced by spinning,”  
*Journal of Applied Physics*, vol. 49, pp. 3993–3997, 1978.
