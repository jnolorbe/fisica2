# Vectores

## Cantidades físicas vectoriales

Las cantidades físicas vectoriales se representan con un vector, el cual tiene **magnitud**, **dirección** y **sentido**. 
La velocidad, aceleración, desplazamiento y fuerza son ejemplos de cantidades físicas vectoriales.

```{figure} https://upload.wikimedia.org/wikipedia/commons/thumb/c/c4/Vector_00.svg/1280px-Vector_00.svg.png
:alt: vector (fuente: Dnu72)
:width: 300px
:align: center
```

## Vectores Unitarios $\mathbf{\hat{i}}$ y $\mathbf{\hat{j}}$

En un sistema de coordenadas cartesianas, los vectores unitarios son la base fundamental para expresar cualquier otro vector.

* El vector unitario **i** (también escrito como $\mathbf{\hat{i}}$) apunta en la dirección positiva del eje x.
* El vector unitario **j** (también escrito como $\mathbf{\hat{j}}$) apunta en la dirección positiva del eje y.

Estos vectores tienen una **magnitud de 1** y solo definen la dirección. 

Cualquier vector $\vec{A}$ puede ser expresado como la suma de sus componentes, multiplicadas por sus respectivos vectores unitarios:

$\vec{A} = A_x \hat{i} + A_y \hat{j}$

Donde:
* $A_x$ es el componente del vector en el eje x.
* $A_y$ es el componente del vector en el eje y.

---
**_Ejemplo 1:_**\
El vector $\vec{A}$ de la figura representa la aceleración de una partícula. Expresar la aceleración en función de sus componentes y calcular su magnitud.

```{figure} https://upload.wikimedia.org/wikipedia/commons/thumb/5/5d/Position_vector.svg/250px-Position_vector.svg.png
:alt: vector aceleracion
:width: 300px
:align: center
```

```{admonition} Resolución
:class: dropdown
- Expresamos $\vec{A}$ en función de sus componentes:\
$\vec{A} = (2 \hat{i} + 3 \hat{j}) m/s^2$

- Calculamo su módulo:\
$A = \sqrt{2^2 + 3^2} = 3.6 m/s^2$
```
---

## Descomposición Rectangular de un Vector

La descomposición rectangular de un vector $\vec{A}$ con magnitud $|\vec{A}|$ y un ángulo $\theta$ con respecto al eje x es:

$A_x = |\vec{A}| cos(\theta)$

$A_y = |\vec{A}| sen(\theta)$

---
**_Ejemplo 2:_**\
Una fuerza $\vec{F}$ tiene una magnitud de $10 \text{ N}$ y forma un ángulo de $30^\circ$ con el eje x. Expresar la fuerza en términos de sus componentes.

```{admonition} Resolución
:class: dropdown
- Descomponemos la fuerza:\
$F_x = 10 cos(30^\circ) = 8.66 \text{ N}$\
$F_y = 10 sen(30^\circ) = 5.00 \text{ N}$

- Expresamos el vector $\vec{F}$ en términos de sus componentes y vectores unitarios como:\
$\vec{F} = (8.66 \hat{i}  + 5.00 \hat{j})\text{ N}$
```
---

## 3. Producto Escalar (o Producto Punto)

El producto escalar es una operación que toma dos vectores y da como resultado un número (un escalar). Se usa para determinar el ángulo entre dos vectores y para encontrar la proyección de un vector sobre otro.

El producto escalar de dos vectores $\vec{A}$ y $\vec{B}$ se define como:

$\vec{A} \cdot \vec{B} = |\vec{A}||\vec{B}| \cos(\theta)$

Donde $\theta$ es el ángulo entre los vectores.

Si conoces las componentes de los vectores, el producto escalar se calcula de forma más sencilla:

$\vec{A} \cdot \vec{B} = (A_x \hat{i} + A_y \hat{j}) \cdot (B_x \hat{i}  + B_y \hat{j}) = A_x B_x + A_y B_y$

---

**_Ejemplo 3:_**\
Un cuerpo es deplazado horizontalmente una distancia de $2.5 \text{ m}$, la fuerza que empuja al cuerpo tiene una magnitud de $100 \text{ N}$ y forma un ángulo de
ángulo de $28^\circ$ con el vector desplazamiento. Deducir el trabajo realizado por la fuerza. 

```{admonition} Resolución
:class: dropdown
- Calculamos el trabajo mecánmico de la fuerza:\
$W = |\vec{F}||\vec{\Delta r}|\cos(\theta)$\
$W = (100 \text{ N})(2.5 \text{ N})\cos(28^\circ)$\
$W = 221 \text{ J}$
```
---

**_Ejemplo 4:_**\
Tres personas ejercen fuerzas sobre una caja para desplazarla a través del plano inliclinado: $\vec{F}_1 = (400 \hat{i} + 300 \hat{j}) \text{ N}$,  $\vec{F}_2 = (1200 \hat{i} + 500 \hat{j}) \text{ N}$ 
y $\vec{F}_3 = (500 \hat{i} + 100 \hat{j}) \text{ N}$. El desplazamiento de la caja es  $\vec{\Delta r} = (2.0 \hat{i} + 1.5\hat{j}) \text{ m}$. Calcula el trabajo neto realizado. (_Sugerencia: El trabajo neto es 
el producto escalar de la fuerza neta por desplazamiento_). 

```{figure} https://org-dcmp-staticassets.s3.us-east-1.amazonaws.com/posterimages/1788_1.jpg
:alt: plano inclinado. (Fuente: DCMP)
:width: 400px
:align: center
```

```{admonition} Resolución
:class: dropdown
- Calculamos la fuerza neta:\
$\vec{F}_{neta} = \vec{F}_1 + \vec{F}_2 + \vec{F}_3$\
$\vec{F}_{neta} = (2100 \hat{i} + 900 \hat{j}) \text{ N}$

- Calculamos el trabajo neto:\
$W_{neto} = \vec{F}_{neta} \cdot \vec{\Delta r}$\
$W_{neto} = (2100 \hat{i} + 900 \hat{j}) \cdot  (2.0 \hat{i} + 1.5\hat{j})$\
$W_{neto} = 2100 (2.0) + 900(1.5) = 5550 $\
$W_{neto} = 5550 \text{ J}$
```
---
## Ejercicios propuestos

1. Calcula el módulo de la fuerza resultante de la suma de dos fuerzas $\vec{F}_1 = (500 \hat{i} + 1200 \hat{j}) \text{ N}$ y $\vec{F}_2 = (900 \hat{i} + 1200 \hat{j}) \text{ N}$ 

2. Un pelota es lanzada con una velocidad de $22.2 \text{ m/s}$ que forma y $62^\circ$ con la horizoantal, calcular los componetes horizontal y vertical de la velocidad.

3. Una persona realiza los siguientes desplazamientos: $\vec{\Delta r}_1 = (400 \hat{i} + 300 \hat{j}) \text{ m}$, $\vec{\Delta r}_2 = (-1000 \hat{i} + 800 \hat{j}) \text{ m}$ 
y $\vec{\Delta r}_3 = (1400 \hat{i} - 1300 \hat{j}) \text{ m}$. Calcular el módulo del desplazmaiento total.

4. Se empuja una caja hacia arriba sobre un plano inclinado de $30^\circ$, la fuerza empleada tiene una magnitud de $500 \text{ N} y forma $43^\circ$ con la horizoantal. 
Calcular el trabajo de la fuerza empleada.

5. Calcula el trabajo desarrollado por una fuerza horizontal $\vec{F} = 1500 \hat{i} \text{ N}$ que empuja a un bloque, tal que se desplaza $\vec{\Delta r} = (400 \hat{i} + 300 \hat{j}) \text{ m}$ 

---
