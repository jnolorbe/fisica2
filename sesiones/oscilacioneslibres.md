# Sesión 3: Oscilaciones Libres

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

## 1. Cinemática del MAS

Una partícula describe un **Movimiento Armónico Simple (MAS)** cuando oscila en línea recta alrededor de una posición de equilibrio con un periodo de oscilación constante. Las ecuaciones cinemáticas de posición ($\vec{x}$), velocidad ($\vec{v}$) y aceleración ($\vec{a}$) se expresan mediante funciones armónicas sinusoidales:

$$\vec{x} = A \text{ sen}(\omega t + \phi)$$

$$\vec{v} = \frac{dx}{dt} = A\omega \cos(\omega t + \phi)$$

$$\vec{a} = \frac{dv}{dt} = -A\omega^2 \text{ sen}(\omega t + \phi)$$

Donde:
* $A$: Amplitud de oscilación ($m$).
* $\omega$: Frecuencia angular ($rad/s$).
* $\phi$: Ángulo de fase ($rad$).

::: {figure} https://github.com/jnolorbe/fisica2/blob/main/figuras/s3_mas01.jpg
:width: 60%
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

## 2. Dinámica del MAS

Según la segunda ley de Newton ($\vec{F} = m\vec{a}$), la fuerza necesaria para generar este movimiento es:

$$\vec{F}_{neta} = -m\omega^2 \vec{x}$$

Esta fuerza es proporcional y opuesta al desplazamiento, por lo que se define como una **Fuerza Recuperadora**.

---
## 3. Energía del Oscilador Armónico

### Energía Potencial ($U$)
La fuerza recuperadora es conservativa, por lo que tiene asociada una energía potencial elástica:
$$U = \frac{1}{2}m \omega^2 x^2$$

### Conservación de la Energía Mecánica ($E$)
En ausencia de fricción, la energía cinética ($K$) y la potencial ($U$) se intercambian constantemente, pero su suma permanece invariable:

$$E = \frac{1}{2}mv^2 + \frac{1}{2}m \omega^2 x^2 = \text{constante}$$

* **En los extremos ($x = \pm A$):** La energía es puramente potencial ($E = \frac{1}{2}kA^2$).
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
:width: 50%
:align: center
**Figura 3.** Esquema de un péndulo simple y fuerzas actuantes.
:::

---

### Péndulo Físico
Cualquier cuerpo rígido que oscila alrededor de un punto de suspensión fijo. Usando dinámica de rotación y considerando el momento de inercia ($I$) respecto al punto de suspensión:

$$T = 2 \pi \sqrt{\frac{I}{mgb}}$$

Donde $b$ es la distancia desde el eje de rotación hasta el centro de masa del cuerpo.

::: {figure} https://raw.githubusercontent.com/jnolorbe/fisica2/main/figuras/s3_mas06.jpg
:width: 50%
:align: center
**Figura 4.** Análisis del péndulo físico.
:::

---

**Metacognición:** ¿Por qué el periodo de un péndulo simple no depende de su masa, pero en un sistema masa-resorte la masa es un factor determinante? Refleja sobre esta diferencia basándote en la naturaleza de la fuerza recuperadora en cada caso.

