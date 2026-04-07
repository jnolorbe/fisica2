# Sesión 3: Oscilaciones

## Introducción

Imagina entrar al Panteón de París en 1851. Del techo cuelga un cable de 67 metros con una pesada esfera de bronce. El péndulo comienza a oscilar en una línea recta, pero con el paso de las horas, notas algo inquietante: la trayectoria de oscilación parece girar lentamente.

¿Es el péndulo el que cambia su dirección? No. Es la Tierra la que está rotando debajo de él. El **Péndulo de Foucault** es quizás la aplicación más famosa y majestuosa de las oscilaciones, demostrando cómo un sistema físico local puede revelarnos secretos de la dinámica de todo un planeta.

::: {figure} https://github.com/jnolorbe/fisica2/blob/main/figuras/s3_foucault.jpg
:alt: Péndulo de Foucault en Valencia
:width: 60%
:align: center
Figura 1. Péndulo de Foucault en la Ciudad de las Artes y las Ciencias, Valencia. (Créditos: Daniel Sancho / CC-BY-SA).
:::

---

## 1. Cinemática del Movimiento Armónico Simple

Una partícula describe un **Movimiento Armónico Simple (MAS)** cuando oscila en línea recta alrededor de una posición de equilibrio con un periodo de oscilación constante. Las ecuaciones cinemáticas de posición ($\vec{x}$), velocidad ($\vec{v}$) y aceleración ($\vec{a}$) se expresan mediante funciones armónicas sinusoidales:

$$\vec{x} = A \text{ sen}(\omega t + \phi)$$

$$\vec{v} = \frac{dx}{dt} = A\omega \cos(\omega t + \phi)$$

$$\vec{a} = \frac{dv}{dt} = -A\omega^2 \text{ sen}(\omega t + \phi)$$

Donde:
* $A$: Amplitud de oscilación ($m$).
* $\omega$: Frecuencia angular ($rad/s$).
* $\phi$: Ángulo de fase ($rad$).

::: {figure} https://github.com/jnolorbe/fisica2/blob/main/figuras/s3_mas01.jpg
:width: 80%
:align: center
Figura 2. Partícula realizando un MAS
:::

### Características Principales

* **Movimiento Oscilatorio:** La partícula se desplaza entre los puntos extremos $x = A$ y $x = -A$, pasando por el equilibrio ($x = 0$).
* **Movimiento Periódico:** El ciclo se repite en un intervalo de tiempo $T$ llamado **periodo**, el cual es independiente de la amplitud.
* **Frecuencia ($f$):** Número de oscilaciones por unidad de tiempo. Se mide en Hertz ($Hz$).

$$f = \frac{N}{t} = \frac{1}{T}$$
    
* **Frecuencia ángular ($\omega$):** Relaciona la frecuencia con la fase circular, expresada en ($rad/s$).

$$\omega =  2 \pi \, f = \frac{2\pi}{T}$$

### Ecuación de Fase (Velocidad vs. Posición)
Al combinar las ecuaciones de posición y velocidad, obtenemos una relación que permite conocer la rapidez de la partícula en cualquier punto de su trayectoria:

$$\vec{v} = \pm \omega \sqrt{ A^2 - x^2}$$

::: {figure} https://github.com/jnolorbe/fisica2/blob/main/figuras/s3_mas03.jpg
:width: 60%
:align: center
Figura 3. Diagrama de fase de un MAS
:::

**Análisis físico:**
* En los extremos ($x = \pm A$), la velocidad es nula ($\vec{v} = 0$).
* En el equilibrio ($x = 0$), la velocidad es máxima ($v_{máx} = \pm A\omega$).

#### Aceleración y Desplazamiento
Al relacionar $\vec{x}$ con $\vec{a}$, se observa que la aceleración es directamente proporcional pero opuesta al desplazamiento:

$$\vec{a} = - \omega^2 x$$

Este signo negativo es fundamental: evidencia que la aceleración siempre apunta hacia la posición de equilibrio (**fuerza recuperadora**). Cuando el cuerpo está a la derecha ($+x$), la aceleración tira hacia la izquierda ($-a$).

---

## 2. Dinámica del Movimiento Armónico Simple

Según la segunda ley de Newton ($\vec{F} = m\vec{a}$), la fuerza necesaria para generar este movimiento es:

$$\vec{F}_{neta} = -m\omega^2 \vec{x}$$

Esta fuerza es proporcional y opuesta al desplazamiento, por lo que se define como una **Fuerza Recuperadora**.

---
## 3. Energía del Movimiento Armónico Simple

### Energía Potencial ($U$)
La fuerza recuperadora es conservativa, por lo que tiene asociada una energía potencial elástica:
$$U = \frac{1}{2}m \omega^2 x^2$$

### Conservación de la Energía Mecánica ($E$)
En ausencia de fricción, la energía cinética ($K$) y la potencial ($U$) se intercambian constantemente, pero su suma permanece invariable:

$$E = \frac{1}{2}mv^2 + \frac{1}{2}m \omega^2 x^2 = \text{constante}$$

* **En los extremos ($x = \pm A$):** La energía es puramente potencial ($E = \frac{1}{2}m \omega^2 A^2$).
* **En el equilibrio ($x = 0$):** La energía es puramente cinética ($E = \frac{1}{2}mv_{máx}^2$).

## 4. Sistemas Oscilantes Clásicos

### Sistema Masa-Resorte
Para una masa $m$ sujeta a un resorte de constante $k$ (Ley de Hooke):
$$\vec{F} = -k \vec{x} \implies \omega = \sqrt{\frac{k}{m}}$$

El periodo resultante es:
$$T = 2\pi \sqrt{\frac{m}{k}}$$

**Dato clave:** El periodo depende de la masa y la rigidez, pero **no de la amplitud**. Un reloj de masa-resorte marcará el mismo tiempo así la oscilación sea pequeña o grande.

---

### Péndulo Simple
Consiste en una masa puntual suspendida de un hilo de longitud $L$. Para ángulos pequeños ($\theta \le 10^\circ$), el arco se aproxima a una línea recta y el movimiento es un MAS con periodo:

$$T = 2 \pi \sqrt{\frac{L}{g}}$$

::: {figure} https://raw.githubusercontent.com/jnolorbe/fisica2/main/figuras/s3_mas04.jpg
:width: 30%
:align: center
**Figura 3.** Péndulo simple.
:::

---

### Péndulo Físico
Cualquier cuerpo rígido que oscila alrededor de un punto de suspensión fijo. Usando dinámica de rotación y considerando el momento de inercia ($I$) respecto al punto de suspensión:

$$T = 2 \pi \sqrt{\frac{I}{mgb}}$$

Donde $b$ es la distancia desde el eje de rotación hasta el centro de masa del cuerpo.

::: {figure} https://raw.githubusercontent.com/jnolorbe/fisica2/main/figuras/s3_mas06.jpg
:width: 30%
:align: center
**Figura 4.** Péndulo físico.
:::
---

## 5. Oscilaciones Amortiguadas
En los sistemas oscilantes reales, las fuerzas de fricción disipan la energía mecánica, provocando que la amplitud disminuya progresivamente hasta que el movimiento se detiene.

:::{figure} https://github.com/jnolorbe/fisica2/blob/main/figuras/s4_maa01.jpg
:alt: Oscilaciones amortiguadas
:width: 60%
:align: center
**Figura 5.** Sistemas oscilantes amortiguados con agua, aceite y aire, [! Ver video][https://www.youtube.com/watch?v=FZNtXdAtFGE]
:::

### Sistma Masa - Resorte Amortiguado
El caso más común es un oscilador sujeto a una fuerza viscosa proporcional a la velocidad: $\vec{f} = -c\vec{v}$, donde $c$ es el coeficiente de amortiguamiento.

:::{figure} https://github.com/jnolorbe/fisica2/blob/main/figuras/s4_maa02.png
:alt: Sistema oscilatorio amortiguado
:width: 60%
:align: center
**Figura 6.**. Fuerzas Recuperadora y Fuerza Viscosa
:::

Aplicando la segunda ley de Newton $F_{neta} = ma = md^2x/dt^2$ y $v = dx/dt$ se tiene la ecuación diferencial de las oscilaciones amortiguadas:

$$F_{neta} = -kx -cv$$

$$\frac{d^2x}{dt^2} + 2\gamma\frac{dx}{dt} + \omega_o^2 x = 0$$

Donde:
* **$\gamma = \frac{c}{2m}$**: Parámetro de amortiguamiento ($rad/s$).
* **$\omega_o = \sqrt{\frac{k}{m}}$**: Frecuencia angular de las oscilaciones libres.

### Regímenes de Movimiento
1. **Amortiguamiento Débil ($\gamma < \omega_o$):** El sistema oscila con una amplitud que decae exponencialmente.
   $$\vec{x} = A e^{-\gamma t} \cos(\omega t + \phi)$$
   Donde $\omega = \sqrt{\omega_o^2 - \gamma^2}$ es la frecuencia amortiguada.
2. **Amortiguamiento Crítico ($\gamma = \omega_o$):** El sistema no oscila y regresa al equilibrio en el tiempo mínimo posible. Es el ajuste ideal para amortiguadores de vehículos.
3. **Sobreamortiguamiento ($\gamma > \omega_o$):** El sistema es tan "pesado" que regresa al equilibrio muy lentamente, sin oscilar.

::: {figure} https://jnolorbe/fisica2/main/figuras/oscilaciones_amortiguadas.png
:width: 70%
:align: center
**Figura 7.** Comparación de los tres regímenes de amortiguamiento.
:::

---

## 6. Oscilaciones Forzadas y Resonancia
Cuando un sistema amortiguado se somete a una fuerza externa periódica $F = F_o \cos(\omega_F t)$, el movimiento puede mantenerse activo. Tras una fase transitoria, el sistema entra en una **fase estacionaria** donde oscila con la frecuencia de la fuerza externa ($\omega_F$).

$$x = A \, sen (\omega_F t - \delta)$$

donde 

La amplitud final ($A$) depende de qué tan cerca esté la frecuencia externa de la frecuencia natural del sistema.  Cuando $\omega_F \approx \omega_o$, el sistema entra en **Resonancia**, alcanzando amplitudes máximas que pueden comprometer la integridad de los materiales.

$$A = \frac{F_o/m}{\sqrt{[\omega_o^2 - \omega_F^2]^2 + [2\gamma\omega_F]^2}}$$

El ángulo de fase:

$$tan \, \delta = \frac{\omega_F^2 - \omega_o^2}{2 \gamma \omega_F}$$

---
