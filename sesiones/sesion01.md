# Sesión 1: Esfuerzos Normales

## I. Fundamento Teórico

### Introducción
Para estudiar las propiedades mecánicas de los materiales, tales como elásticidad y plasticidad, se utilizan probetas o barras que son sometidas a fuerzas de tracción o compresión, hasta que se produce la rotura de la probeta. Este ensayo mide la resistencia de un material a una fuerza estática o aplicada lentamente.

La elasticidad es la propiedad mecánica de ciertos materiales de sufrir deformaciones reversibles debido a la acción de fuerzas y de recuperar su forma original luego de que estas fuerzas se supriman.
Piensa en una pelota o un resorte: Al ejercer una fuerza sobre estos, se deforman y luego vuelven a su estado original una vez que la fuerza se suprime.

Para comprender y cuantificar estas propiedades, se utilizan ensayos de materiales, uno de los más comunes es la prueba de tracción y compresión, donde se somete una muestra cilíndrica o en forma de barra, conocida como probeta, a una fuerza que la estira (tracción) o la aplasta (compresión) lentamente.

Este ensayo no solo evalúa la elasticidad, sino también otras propiedades mecánicas como la resistencia y la plasticidad, que es la capacidad del material para deformarse de forma permanente sin romperse

```{iframe} https://www.doitpoms.ac.uk/vidlib/videos/video/annealed1.mp4
:width: 80%
:align: center
Video 1.  Ensayo de tracción de una probeta de cobre
```

---
### Esfuerzos Normales

Cuando aplicas una fuerza a un objeto, este experimenta una tensión interna que contrarresta la fuerza externa. Esta tensión interna por unidad de área se conoce como esfuerzo. El esfuerzo normal se produce cuando la fuerza aplicada es perpendicular a la superficie del material.

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


### Ley de Hooke
El esfuerzo normal de tracción o compresión sobre una varilla, cable o barra sólida es directamente proporcional a la deformación unitaria. La constante de proporción se denomina Módulo de Elasticidad o Módulo de Young, el cuál es propio de cada material. 

$$
\sigma = E \, \delta 
$$

Donde

$\sigma =\frac{F}{A} =$Tensión o esfuerzo normal (Pa)

$E =$ Módulo de elásticidad (Pa)

$\delta =\frac{\Delta L}{L}=$ deformación unitaria o relativa (%)


### Curva esfuerzo vs. deformación

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
### Módulo de elasticidad
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

### Deformación transversal

Cuando un material se deforma en una dirección determinada, ocasiona deformaciones en las direcciones transversales. Así por ejemplo cuando la probeta es sometida a una tracción longitudinal el diámetro se reduce. La deformación transversal unitaria es proporcional a la deformación longitudinal unitaria.

$$ \delta_{T}=\,-\mu\,\delta_{L} $$ 

Donde

$\delta_{T}$ = Deformación transversal.

$\mu$ =Coeficiente de Poisson. 

$\delta_{L}$ = Deformación longitudinal

El signo negativo en la ecuación indica que mientras la deformación longitudﬁnal aumenta, la deformación transversal disminuye, o viceversa. 

:::{figure}  https://github.com/jnolorbe/fisica2/blob/main/figuras/500px-PoissonRatio.png
:alt: coeficiente de poisson
:width: 50%
:align: center
Figura 6.  Deformación transversal de una varilla
:::

### Coeficiente de Poisson
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

### Módulo de compresibilidad

Considera un bloque rectangular sujeto a fuerzas de compresión normal a toda sus caras, digamos en las direcciones de los ejes  X, Y y Z, como se muestra en la siguiente figura.

```{figure} https://s3-us-west-2.amazonaws.com/courses-images-archive-read-only/wp-content/uploads/sites/222/2014/12/20102444/Figure_06_03_09a.jpg
:alt: compresibilidad
:width: 50%
:align: center
Figura 7.  Deformación Volumétrica
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

## II. Problemas Resueltos

### Problema 1: Cable conductor 💡
```{admonition} Diseño de un cable 
:class: important
Se está diseñando una línea de transmisión de alta tensión que debe cruzar un valle. Para la selección del material, el equipo de ingenieros ha evaluado dos aleaciones conductoras: una de Cobre (Cu) y otra de Aluminio (Al), cuyas curvas de esfuerzo vs. deformación se muestran en la Figura.

:::{figure} https://github.com/jnolorbe/fisica2/blob/main/figuras/curvaesfuerzodeformacion.jpg
:alt: curva esfuerzo deformacion cobre y aluminio
:width: 50%
:align: center
Figura 8. Curva esfuerzo deformación Cobre y Aluminio
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

### Problema 2: Cable compuesto 💡
```{admonition} Deformación de un cable compuesto 
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

## III. Actividades para el Portafolio Digital 📓

### Desafío 1 
**Diseño de Soportes para Líneas de Transmisión (Esfuerzo Normal)**
**Contexto:** Se está evaluando el uso de tubos de acero huecos para actuar como soportes verticales en una subestación. El tubo debe resistir una carga de tracción axial de $400 \text{ kN}$ generada por el tensado de los conductores.

* **Especificaciones:** El diámetro interior del tubo es de $100 \text{ mm}$.
* **Limitación Técnica:** Para garantizar la seguridad estructural, el esfuerzo normal no debe superar los $120 \text{ MPa}$.
* **Reto:** Determine el diámetro exterior mínimo del tubo necesario para cumplir con la normativa.
* **Análisis Crítico:** ¿Cómo afectaría a la seguridad del poste si el material presentara porosidades internas que redujeran el área efectiva de la sección transversal en un 5%?
---

### Desafío 2 
**Compresión en Núcleos de Transformadores (Materiales Compuestos)**
**Contexto:** En el ensamblaje de un núcleo de potencia, se utiliza una barra de acero de $50 \text{ mm}$ de diámetro protegida por una carcasa de hierro fundido de $5 \text{ mm}$ de espesor. El conjunto tiene una longitud total de $2 \text{ m}$.

* **Situación:** Durante el ajuste mecánico, el conjunto se somete a una carga de compresión.
* **Reto:** Deduzca la carga total $P$ necesaria para comprimir la barra compuesta exactamente $0.8 \text{ mm}$.
* **Propiedades de los Materiales:**
    * Acero: $E = 200 \text{ GPa}$
    * Hierro Fundido: $E = 100 \text{ GPa}$
* **Análisis Crítico:** Si la carga se aplica de forma no uniforme, ¿cuál de los dos materiales corre mayor riesgo de alcanzar su límite elástico primero?
---

### Desafío 3
**Estabilidad de Cargas Pesadas (Sistemas Indeterminados)**
**Contexto:** Un bloque rígido de masa $M$ debe ser soportado simétricamente por tres varillas verticales para asegurar que permanezca nivelado.

:::{figure} https://mathalino.com/sites/default/files/images/236-block-supported-by-three-rods.jpg
:alt: tres varillas
:width: 50%
:align: center
:::

* **Configuración:**
    * **2 Varillas de Cobre:** Área = $900 \text{ mm}^2$, $E = 120 \text{ GPa}$, $\sigma_{adm} = 70 \text{ MPa}$.
    * **1 Varilla de Acero (Central):** Área = $1200 \text{ mm}^2$, $E = 200 \text{ GPa}$, $\sigma_{adm} = 140 \text{ MPa}$.
* **Reto:** Calcule la masa máxima $M$ (en kg) que puede soportarse sin que ninguna de las varillas falle.
* **Reflexión:** Dado que el bloque es rígido, las deformaciones en las tres varillas deben ser iguales ($\delta_c = \delta_a$). Use esta condición de compatibilidad para resolver el sistema.
---

### Desafío 4

**Análisis de Desplazamiento en Sensores de Nivel**
**Contexto:** Una barra rígida $AB$ se utiliza para transmitir el movimiento a dos sensores verticales. La barra está inicialmente horizontal. Se aplica una carga $P = 50 \text{ kN}$ en la posición indicada en la Figura.

:::{figure} https://mathalino.com/sites/default/files/images/213-given.jpg
:alt: dos varillas verticales
:width: 50%
:align: center
:::

* **Situación:** Las varillas de soporte tienen diferentes propiedades elásticas y longitudes.
* **Reto:** Deduzca el movimiento vertical (descenso) del punto donde se aplica la carga $P$.
* **Aumentación con IA:** Ingrese la geometría del problema en una IA y pregunte: *"¿En qué punto de la barra AB debería colocarse la carga P para que el descenso sea uniforme y la barra permanezca horizontal?"*. Analice la importancia del "centro de rigidez" en este escenario.
---

### Desafío 5
**Evaluación de Fallas en Actuadores Multi-Etapa**
**Contexto:** Un actuador lineal está compuesto por tres secciones unidas: aluminio, acero y bronce. En el sistema de automatización, se aplican cargas axiales en diferentes puntos debido a la resistencia de los mecanismos internos (Figura P-108).

:::{figure} https://mathalino.com/sites/default/files/reviewer-strength/01-stress/108-composite-bar-different-area.gif
:alt: barra compuesta aluminio acero bronce
:width: 50%
:align: center
:::

* **Límites de Esfuerzo:**
    * Acero: $140 \text{ MPa}$
    * Aluminio: $90 \text{ MPa}$
    * Bronce: $100 \text{ MPa}$
* **Reto:** Deduzca el valor máximo de la carga de referencia $P$ (en kN) para que ninguna sección supere su esfuerzo admisible.
* **Metacognición:** Identifique el tramo con el menor factor de seguridad. Si tuviera que optimizar el diseño aumentando el área de una sola sección para permitir una carga $P$ mayor, ¿cuál elegiría?
---

## IV. Referencias

 - https://www.doitpoms.ac.uk/tlplib/mechanical_properties/tensile.php
 - https://www.youtube.com/embed/XTfMkBiUXOA
 - https://courses.lumenlearning.com/suny-osuniversityphysics/chapter/12-3-stress-strain-and-elastic-modulus/
 - https://www.mdpi.com/1996-1944/14/21/6305#
 - https://mathalino.com