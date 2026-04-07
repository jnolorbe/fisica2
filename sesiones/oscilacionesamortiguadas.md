# Sesión 4: Oscilaciones Amortiguadas y Forzadas

## Introducción: El Desastre del Puente Tacoma Narrows
En 1940, un puente recién inaugurado en el estado de Washington comenzó a oscilar violentamente bajo una brisa moderada. No fue un terremoto lo que lo derribó, sino un fenómeno físico extremo. En el siguiente video, se atribuye de forma categórica la destrucción del puente al fenómeno de Resonancia. Sin embargo, en el mundo de la ingeniería, las explicaciones simples suelen ocultar fenómenos complejos. ¿Fue realmente una resonancia clásica (como la de una copa rompiéndose por la voz de un tenor) o estamos ante un sistema de retroalimentación aeroelástica mucho más sofisticado?

```{iframe} https://www.youtube.com/embed/k5yTVHr6V14?si=xguYGQsjyCejd_sU
:width: 100%
:align: center
Video 1.  Destrucción del puente Tacoma Narrows
```
---

## 2. Oscilaciones Amortiguadas
En los sistemas oscilantes reales, las fuerzas de fricción disipan la energía mecánica, provocando que la amplitud disminuya progresivamente hasta que el movimiento se detiene.

:::{figure} https://github.com/jnolorbe/fisica2/blob/main/figuras/s4_maa01.jpg
:alt: Oscilaciones amortiguadas
:width: 60%
:align: center
Figura 1. [!Sistemas oscilantes amortiguados con agua, aceite y aire]][https://www.youtube.com/watch?v=FZNtXdAtFGE]
:::

### Sistma Masa - Resorte Amortiguado
El caso más común es un oscilador sujeto a una fuerza viscosa proporcional a la velocidad: $\vec{f} = -c\vec{v}$, donde $c$ es el coeficiente de amortiguamiento.

:::{figure} https://github.com/jnolorbe/fisica2/blob/main/figuras/s4_maa02.png
:alt: Sistema oscilatorio amortiguado
:width: 60%
:align: center
Figura 2. Fuerzas Recuperadora y Fuerza Viscosa
:::

Aplicando la segunda ley de Newton $F_{neta} = ma = md^2x/dt^2$ y $v = dx/dt$ se tiene la ecuación diferencial de las oscilaciones amortiguadas:

$$F_{neta} = -kx -cv$$

$$\frac{d^2x}{dt^2} + 2\gamma\frac{dx}{dt} + \omega_o^2 x = 0$$

Donde:
* **$\gamma = \frac{b}{2m}$**: Parámetro de amortiguamiento ($rad/s$).
* **$\omega_o = \sqrt{\frac{k}{m}}$**: Frecuencia angular de las oscilaciones libres.

### Regímenes de Movimiento
1. **Amortiguamiento Débil ($\gamma < \omega_o$):** El sistema oscila con una amplitud que decae exponencialmente.
   $$\vec{x} = A e^{-\gamma t} \cos(\omega t + \phi)$$
   Donde $\omega = \sqrt{\omega_o^2 - \gamma^2}$ es la frecuencia amortiguada.
2. **Amortiguamiento Crítico ($\gamma = \omega_o$):** El sistema no oscila y regresa al equilibrio en el tiempo mínimo posible. Es el ajuste ideal para amortiguadores de vehículos.
3. **Sobreamortiguamiento ($\gamma > \omega_o$):** El sistema es tan "pesado" que regresa al equilibrio muy lentamente, sin oscilar.

::: {figure} https://raw.githubusercontent.com/jnolorbe/fisica2/main/figuras/s4_damped_graphs.png
:width: 70%
:align: center
**Figura 2.** Comparación de los tres regímenes de amortiguamiento.
:::

---

## 3. Oscilaciones Forzadas y Resonancia
Cuando un sistema amortiguado se somete a una fuerza externa periódica $F = F_o \cos(\omega_F t)$, el movimiento puede mantenerse activo. Tras una fase transitoria, el sistema entra en una **fase estacionaria** donde oscila con la frecuencia de la fuerza externa ($\omega_F$).

### Factor de Magnificación (FM)
La amplitud final ($A$) depende de qué tan cerca esté la frecuencia externa de la frecuencia natural del sistema:

$$A = \frac{F_o/k}{\sqrt{[1-(\omega_F/\omega_o)^2]^2 + [2\gamma(\omega_F/\omega_o)]^2}}$$

El **Factor de Magnificación** define la relación entre la amplitud dinámica y el desplazamiento estático. Cuando $\omega_F \approx \omega_o$, el sistema entra en **Resonancia**, alcanzando amplitudes máximas que pueden comprometer la integridad de los materiales.

---

## 4. Problemas Resueltos 💡


http://googleusercontent.com/immersive_entry_chip/0

---

## 5. Actividades con Recursos TIC 📱

1. **Simulador de Resonancia:** Experimenta con las curvas de amplitud y fase en el [Simulador de Walter Fendt](http://www.walter-fendt.de/ph14s/resonance_s.htm).
2. **Laboratorio Virtual:** Analiza las gráficas de energía disipada en [esta plataforma educativa](http://goo.gl/sk6htM).

---

## 6. Problemas Propuestos

1. **Interpretación Física:** Verifique que $x = e^{-\gamma t} [A + Bt]$ es solución para un amortiguamiento crítico. ¿Qué representa físicamente $B$?
2. **Motor Eléctrico:** Un motor de $30 \text{ kg}$ sobre resortes ($k=100 \text{ N/m}$) tiene un rotor desbalanceado. Determine la frecuencia de resonancia si $\gamma = 0.15$.
3. **Potencia Disipada:** Demuestre que la rapidez de cambio de la energía mecánica en un oscilador amortiguado es $\frac{dE}{dt} = -bv^2$. ¿Qué importancia tiene este resultado para el diseño de frenos electromagnéticos?

---

**Metacognición:** * ¿Cómo se aplica el concepto de resonancia en la sintonización de una radio analógica? 
* En un circuito eléctrico RLC, ¿cuál componente cumple la función del amortiguador ($b$) en el sistema mecánico? Justifica tu respuesta.

---

# Reto de Investigación: El Colapso del Tacoma Narrows – Desmontando el Mito

## 1. El Conflicto Teórico (Tensión Cognitiva)
Durante décadas, el colapso del puente Tacoma Narrows (1940) se ha enseñado en los cursos de física como el ejemplo supremo de **Resonancia Forzada**. Sin embargo, la comunidad científica e ingenieril ha demostrado que esta explicación es incompleta. El fenómeno real involucró una interacción compleja entre la estructura y el viento conocida como **Flameo Aeroelástico (Flutter)**.

**Tu misión:** Como futuro ingeniero de la FIEE-UNAC, debes investigar la frontera donde la resonancia y la autoexcitación se encuentran, utilizando fuentes de alto rigor académico.

---

## 2. El Producto: Video-Ensayo o Informe Técnico
Deberás producir un contenido (video de 3 min o informe de 2 páginas) que sustente la siguiente tesis:

> *"El viento constante no empujó al puente rítmicamente como una fuerza externa; fue la geometría del puente la que 'convirtió' ese flujo constante en torques periódicos (vórtices), creando un sistema de retroalimentación (feedback) que indujo una inestabilidad torsional catastrófica."*

### Puntos clave a desarrollar:
1. **Vortex Shedding (Desprendimiento de Vórtices):** Explica cómo el aire genera remolinos periódicos al chocar con una viga sólida y cómo estos generan fuerzas oscilatorias.
2. **El Fenómeno de Sincronización (Lock-in):** Describe cómo la frecuencia de los vórtices se "engancha" a la frecuencia natural de la estructura.
3. **Resonancia vs. Autoexcitación:** Argumenta si la resonancia es la causa final o solo un síntoma del proceso de flameo.
4. **Analogía Eléctrica (FIEE):** Compara el colapso con un **Circuito Oscilador con Retroalimentación Positiva**. Explica cómo una fuente de energía continua (viento/CC) puede transformarse en una oscilación alterna (vibración/CA) debido al diseño del sistema.



---

## 3. Fuentes de Investigación Obligatorias
Para que tu trabajo sea válido, debes contrastar la información de al menos dos de estas fuentes:

* **Billah, K. & Scanlan, R. (1991):** *"Resonance, Tacoma Narrows Bridge Failure, and Undergraduate Physics Textbooks"*. (El texto definitivo que critica la versión de los libros escolares).
* **APS Physics (2016):** [History: Collapse of the Tacoma Narrows Bridge](https://www.aps.org/archives/publications/apsnews/201611/physicshistory.cfm).
* **Green, D. & Unruh, W. G. (2006):** *"The Failure of the Tacoma Bridge: A physical model"*. (Para un análisis matemático más profundo).
* **Physics Today (2015):** *"The Tacoma Narrows Bridge collapse on film and video"*. (Análisis de la evidencia visual).

---

## 4. Metacognición y Aumentación con IA
Para finalizar, responde en tu Portafolio Digital:
1. **Indagación con IA:** Pregunta a un modelo de IA: *"¿Por qué el artículo de Billah y Scanlan de 1991 afirma que el colapso del Tacoma Narrows NO fue resonancia en el sentido estricto?"*. Compara su respuesta con tu lectura personal de la fuente.
2. **Reflexión:** Tras investigar, ¿cómo explicarías ahora este fenómeno a un compañero de primer ciclo sin usar la palabra "resonancia"?
3. **Aplicación:** ¿Qué lecciones de este desastre mecánico aplicarías al diseñar un sistema de control para un motor eléctrico sujeto a cargas variables?

---
*Material diseñado para la Unidad I: Oscilaciones — Física 2 (FIEE-UNAC) 2026.*
*Material diseñado para el curso Física 2 - Facultad de Ingeniería Eléctrica y Electrónica (UNAC).*