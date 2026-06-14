# SimGravedad
Aprendiendo python desarrollando un simulador gravitatorio

Un simulador dinámico bidimensional de mecánica orbital y fuerzas gravitatorias implementado en Python utilizando gráficos vectoriales mediante la librería nativa `Turtle`.

## Características del Motor de Física
* **Integración Numérica:** Utiliza aproximación por el método de Euler para resolver ecuaciones diferenciales cinemáticas paso a paso ($\Delta t$).
* **Física Gravitatoria N-Cuerpos:** Cálculo continuo de la aceleración resultante aplicando la ley de la inversa del cuadrado de Newton frente a múltiples centros de masa simultáneos.
* **Modelo de Empuje Dinámico (Aeroespacial):** Simulación de sistemas de propulsión de naves mediante la descomposición de vectores de empuje basándose en la orientación (`heading`) y control de acelerador fraccional (`throttle`).
* **Detección de Colisiones Básica:** Restricción de posición y anulación del vector de velocidad relativa al entrar en contacto con el radio de corte del suelo de cualquier cuerpo celeste.

## Controles en Tiempo Real
* `+` / `-`: Control del factor de escala (Zoom dinámico del espacio).
* `.` / `,`: Modificación del diferencial de tiempo ($\Delta t$) para acelerar o ralentizar la simulación.
* `A` / `Z`: Control incremental/decremental de la fuerza de empuje del motor de la nave.
* `X`: Corte de inyección inmediato (Thruster Cut).
* `Q`: Salida segura de la aplicación.
