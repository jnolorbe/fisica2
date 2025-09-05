# Esfuerzo normal 

## Introducción
Para estudiar las propiedades mecánicas de los materiales, tales como elásticidad y plasticidad, se utilizan probetas o barras que son sometidas a fuerzas de tracción o compresión, hasta que se produce la rotura de la probeta. Este ensayo mide la resistencia de un material a una fuerza estática o aplicada lentamente.

La elasticidad es la propiedad mecánica de ciertos materiales de sufrir deformaciones reversibles debido a la acción de fuerzas y de recuperar su forma original luego de que estas fuerzas se supriman.
Cuando aplicamos una fuerza a un objeto, este puede deformarse. La elasticidad es la propiedad que tienen algunos materiales de deformarse de manera reversible ante una fuerza y, luego de que la fuerza se retira, recuperar completamente su forma original. Piensa en un resorte o una banda elástica: se estiran al aplicar una fuerza y vuelven a su estado inicial cuando la sueltas.

Para comprender y cuantificar estas propiedades, los ingenieros utilizan ensayos de materiales. Uno de los más comunes es la prueba de tracción y compresión, donde se somete una muestra cilíndrica o en forma de barra, conocida como probeta, a una fuerza que la estira (tracción) o la aplasta (compresión) lentamente.

Este ensayo no solo evalúa la elasticidad, sino también otras propiedades mecánicas como la resistencia y la plasticidad, que es la capacidad del material para deformarse de forma permanente sin romperse

```{iframe} https://www.doitpoms.ac.uk/vidlib/videos/video/annealed1.mp4
:width: 80%
:align: center
Video 1.  Ensayo de tracción de una probeta de cobre
```

---
## Esfuerzos Normales

Cuando aplicas una fuerza a un objeto, este experimenta una tensión interna que contrarresta la fuerza externa. Esta tensión interna se conoce como esfuerzo. El esfuerzo normal se produce cuando la fuerza aplicada es perpendicular a la superficie del material.

Se clasifica en dos tipos principales:

**Esfuerzo de Tracción:** Ocurre cuando la fuerza externa tiende a estirar o alargar el material. Piensa en una cuerda que está siendo jalada por ambos extremos. La tensión interna que se desarrolla dentro de la cuerda para resistir ese estiramiento es un esfuerzo de tracción.

**Esfuerzo de Compresión:** Se produce cuando la fuerza externa tiende a aplastar o acortar el material. Un claro ejemplo es una columna que soporta el peso de un techo. El material de la columna experimenta un esfuerzo de compresión para resistir el peso que lo comprime.

El esfuerzo normal se calcula como dividiendo la fuerza entre el área transversal sobre la que actúa. 

$$\sigma = \frac{F}{A}$$

Donde:

$\sigma$ es el esfuerzo normal, medido en pascales (Pa).

$F$ es la fuerza normal aplicada.

$A$ es el área de la sección transversal.

```{figure} https://study.com/cimages/multimages/16/stress_strain_img_0000032635480025331965683.jpg
:alt: Esfuerzos normales
:width: 300px
:align: center

Figura 1.  Esfuerzo normal: (a) tracción y (b) compresión
```


## Ley de Hooke
El esfuerzo normal de tracción o compresión sobre una varilla, cable o barra sólida es directamente proporcional a la deformación unitaria. La constante de proporción se denomina Módulo de Elasticidad o Módulo de Young, el cuál es propio de cada material. 

$$
\sigma = E \, \delta 
$$

Donde

$\sigma =\frac{F}{A} =$Tensión o esfuerzo normal (Pa)

$E =$ Módulo de elásticidad (Pa)

$\delta =\frac{\Delta L}{L}=$ deformación unitaria o relativa (%)


## Curva esfuerzo vs. deformación

Para conocer las propiedades elásticas de un sólido se utilizan máquinas de ensayo de tracción que miden la deformación longitudinal unitaria de una probeta en función del esfuerzo de tracción aplicado.

```{figure} https://upload.wikimedia.org/wikipedia/commons/thumb/0/0c/Inspekt_desk_50kN_IMGP8563.jpg/250px-Inspekt_desk_50kN_IMGP8563.jpg
:alt: Máquina de ensayo de tracción universal
:width: 300px
:align: center
:class: centered-caption
Figura 2.  Máquina de ensayo de tracción universal
```


```{figure} http://personales.upv.es/~avicente/curso/unidad2/FIG2-3.jpg
:alt: Máquina de ensayo de tracción
:width: 300px
:align: center
:class: centered-caption
Figura 3.  Probetas para ensayos de tracción
```
El resultado de los ensayos de tracción se muestra en una gráfica de la tensión o esfuerzo (en MPa) vs deformación unitaria (en %), que es característico de cada material, en ella se puede observar una zona elástica, en la que que el esfuerzo y la deformación tienen una relación lineal y la zona plástica donde el material se deforma sin que exista un incremento apreciable en el esfuerzo. 

En la gráfica se puede observar el _punto de fluencia_ ($Y$) donde el material deja de comportarse elásticamente para comenzar a deformarse de forma irreversible. En materiales que no tienen un punto de fluencia claro, se define el "_límite convencional de fluencia_", que es la tensión ($S_Y$) necesaria para alcanzar una deformación permanente específica del $0.2\%$. El punto de máximo esfuerzo $U$ se le denomina resistencia a la tracción $S_U$, a partir de este punto el material continua deformándose a pesar de que el esfuerzo empieza a disminuir hasta que se produce la ruptura $F$.

:::{figure} http://www.mecapedia.uji.es/images/modulo_de_elasticidad.2.gif
:alt: curva esfuerzo - deformacion
:width: 50%
:align: center
:class: centered-caption
Figura 4.  Gráfica de la tensión vs. la deformación unitaria
:::

En la siguiente Figura se compara la gráfica de la tensión vs deformación de un material Frágil y un material Ductil.

:::{figure} http://www.mecapedia.uji.es/images/ensayo_de_traccion.1.gif
:alt: material ductil y fragil
:width: 50%
:align: center
:class: centered-caption
Figura 5.  Curva esfuerzo - deformación de un material fragil y otro ductil
:::
---
## Módulo de elasticidad
En la siguiente tabla se muestra los valores del módulo de elasticidad de algunos materiales.

<table border="1">
<caption>Tabla 1. Módulo de Elasticidad. Fuente: Koshkin N. I., Shirkévich M. G.. Manual de Física Elemental. Editorial Mir 1975.</caption>
<tr>
 <th>Metal</th>
 <th>Módulo de elasticidad (GPa)</th>
</tr>
<tr>
 <td>Acero</td>
 <td>170 - 206</td>
</tr>
<tr>
 <td>Cobre</td>
 <td>82 - 127</td>
</tr>
<tr>
 <td>Aluminio</td>
 <td>63-70</td>
</tr>
<tr>
 <td>Latón</td>
 <td>89 - 98</td>
</tr>
<tr>
 <td>Niquel</td>
 <td>204</td>
</tr>
<tr>
 <td>Titanio</td>
 <td>116</td>
</tr>
<tr>
 <td>Cinc Laminado</td>
 <td>82</td>
</tr>
<tr>
 <td>Plata</td>
 <td>82,7</td>
</tr>
</table>

## Deformación transversal

Cuando un material se deforma en una dirección determinada, ocasiona deformaciones en las direcciones transversales. Así por ejemplo cuando la probeta es sometida a una tracción longitudinal el diámetro se reduce. La deformación transversal unitaria es proporcional a la deformación longitudinal unitaria.

$$ \delta_{T}=\,-\mu\,\delta_{L} $$ 

Donde

$\delta_{T}$ = Deformación transversal.

$\mu$ =Coeficiente de Poisson. 

$\delta_{L}$ = Deformación longitudinal

El signo negativo en la ecuación indica que mientras la deformación longitudﬁnal aumenta, la deformación transversal disminuye, o viceversa.

:::{figure} https://upload.wikimedia.org/wikipedia/commons/thumb/e/ec/PoissonRatio.svg/300px-PoissonRatio.svg.png
:alt: coeficiente de poisson
:width: 50%
:align: center
Figura 6.  Deformación transversal de una varilla
:::

## Coeficiente de Poisson
En la siguiente tabla se muestra los valores del coeficiente de Poisson de algunos materiales.


<table border="1">
<caption>Tabla 2. Coeficiente de Poisson</caption>
<tr>
 <th>Metal</th>
 <th>Coeficiente de Poisson</th>
</tr>
<tr>
 <td>Acero</td>
 <td>0,27 - 0,30</td>
</tr>
<tr>
 <td>Cobre</td>
 <td>0,34</td>
</tr>
<tr>
 <td>Plomo</td>
 <td>0,44</td>
</tr>
<tr>
 <td>Bronce</td>
 <td>0,31</td>
</tr>
<tr>
 <td>Niquel</td>
 <td>0,30</td>
</tr>
<tr>
 <td>Titanio</td>
 <td>0,34</td>
</tr>
</table>

## Módulo de compresibilidad

Considera un bloque rectangular sujeto a fuerzas de compresión normal a toda sus caras, digamos en las direcciones de los ejes  X, Y y Z, como se muestra en la siguiente figura.

```{figure} https://s3-us-west-2.amazonaws.com/courses-images-archive-read-only/wp-content/uploads/sites/222/2014/12/20102444/Figure_06_03_09a.jpg
:alt: compresibilidad
:width: 50%
:align: center
Figura 7.  Defomeación Volumétrica
```

La deformación total en la dirección del eje  X, resulta ser la suma de la deformación longitudinal debido al esfuerzo de tracción en el eje X más las defomaciones transversales debido a los esfuerzos  de tracción en los ejes Y y Z, y de este mismo modo la deformación total en cada una de las direcciones se expresa:

$$\epsilon_x\,=\,\frac{\sigma_x}{E} - \mu \frac{\sigma_y}{E} - \mu \frac{\sigma_z}{E}$$

$$\epsilon_y\,=\,\frac{\sigma_y}{E} - \mu \frac{\sigma_x}{E} - \mu \frac{\sigma_z}{E}$$

$$\epsilon_z\,=\,\frac{\sigma_z}{E} - \mu \frac{\sigma_x}{E} - \mu \frac{\sigma_y}{E}$$

La deformación volumétrica es la suma de las deformaciones totales en cada dirección.

$$\delta_V\,=\,\epsilon_x \, + \,\epsilon_y \, + \, \epsilon_z$$

$$\delta_V\,=\,\frac{(1- 2\mu)}{E}(\sigma_x \, + \,\sigma_y \, + \, \sigma_z)$$

Si los esfuerzos normales son en todas las direcciones de la misma magnitud, como es el caso de un cuerpo sujeto a la presión de un fluido, esposible definir el módulo de compresibilidad en función del módulo de elásticidad.

$$\delta_V\,=\,\frac{3(1- 2\mu)}{E}(\sigma)$$

De aqui se define el módulo de compresibiliad K.

$$K \,=\,\frac{E}{3(1- 2\mu)}$$


## Problemas Resueltos
---
```{admonition} Problema 1: Diseño de un cable conductor para una línea de transmisión 💡
:class: important
Se está diseñando una línea de transmisión de alta tensión que debe cruzar un valle. Para la selección del material, el equipo de ingenieros ha evaluado dos aleaciones conductoras: una de Cobre (Cu) y otra de Aluminio (Al), cuyas curvas de esfuerzo vs. deformación se muestran en la [](#fig1).

:::{figure} https://github.com/jnolorbe/fisica2/blob/main/figuras/curvaesfuerzodeformacion.jpg
:label: fig1
:alt: curva esfuerzo deformacion cobre y aluminio
:width: 50%
:align: center
Curva esfuerzo deformación Cobre y Aluminio ([](https://doi.org/10.3390/ma14216305) )
:::

- a) Calcula el Módulo de Young para cada material y determina cuál de los dos materiales es más elástico.
- b) Se estima que el cable experimentará un esfuerzo máximo de $300 \text{ MPa}$, determina cuál de los dos materiales es el más adecuado.
- c) Si el cable tendrá una sección transversal de $120 mm^2$, calcula la máxima tensión (en kN) que soportará en el tramo elástico.
- d) Si el tramo del cable es de $500 \text{ m}$, calcula el cambio de longitud que experimentará bajo un esfuerzo de $300 \text{ MPa}$.

```
```{admonition} Solución
:class: dropdown hint
**a)** En el tramo lineal de cada gráfica, es posible estimar que para $\delta = 2 \times 10^{-3}$, los esfuerzos en cada material son: $\sigma_{Al} = 120 \text{ MPa}$ y $\sigma_{Cu} = 250 \text{ MPa}$. por lo que el módulo de Young se calcula:

$E_{Al} = \frac{\sigma_{Al}}{\delta} = \frac{120 \text{ MPa}}{2 \times 10^{-3}} = 60 \text{ GPa}$

$E_{Cu} = \frac{\sigma_{Cu}}{\delta} = \frac{250 \text{ MPa}}{2 \times 10^{-3}} = 125 \text{ GPa}$

**El resultado muestra que el aluminio es más elástico que el cobre.**

**b)** En la gráfica se muestra que el límite de fluencia de cada material son aproximadamente: 
- $\sigma_{Y(Al)} = 250 \text{ MPa}$
- $\sigma_{Y(Cu)} = 450 \text{ MPa}$

El cobre será el materia que pueda soportar un esfuerzo máximo de $ 300 \text{ MPa}$ sin que el materia experimente deformaciones permanentes.

**c)** La máxima tensión que el cable puede soportar es:

$F_{max} = \sigma_{max} A = (300 \text{ MPa})(120 mm^2)$

$F_{max} = 36 000 \text{ N}= 36 \text{ kN}$

**d)** El cambio de longitud es:

$\Delta L = \sigma L_{o} / E = (300 \text{ MPa}) (500 \text{ m})/ 125 \text{ GPa}$

$\Delta L = 1.2 \text{ m}$
```
---

```{admonition} Problema 2: Cable compuesto 💡
:class: important
Una varilla de cobre de longitud $100 \text{ cm}$ y de sección $2 \text{ cm}^2$ esta sujeta por uno de sus extremos a otra varilla de acero dulce de longitud $L$ y de sección $4 \text{ cm}^2$. Esta varilla compuesta se somete a una tracción de $30 \text{ kN}$ en sus extremos. Si la deformación longitudinal de cada varilla es la misma, deducir la longitud $L$ de la varilla de acero dulce. ($E_{cobre} = 130 \text{ GPa}$, $E_{acero} = 270 \text{ GPa}$).
```

```{admonition} Solución
:class: dropdown hint

- La deformación de las varillas son iguales: 

$\Delta L_{cobre}=\Delta L_{acero}$

- Utilizando la Ley de Hooke:

$[\frac{FL_o}{AE}]_{cobre} = [\frac{FL_o}{AE}]_{acero}$

$\frac{100 \text{ cm}}{(2 \text{ cm}^{2})(130 \text{ GPa})}=\frac{L}{(4 \text{ cm}^{2})(210\text{ GPa})}$

$L=320 \text{ cm}$


```
---


 ## Referencias:
 - https://www.doitpoms.ac.uk/tlplib/mechanical_properties/tensile.php
 - https://www.youtube.com/embed/XTfMkBiUXOA
 - https://courses.lumenlearning.com/suny-osuniversityphysics/chapter/12-3-stress-strain-and-elastic-modulus/
 - https://github.com/jnolorbe/fisica2/blob/main/figuras/curvaesfuerzodeformacion.jpg

 
