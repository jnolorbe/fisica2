# Sesión 2: Esfuerzos Cortantes

## Introducción
Los esfuerzos cortantes o de cizalladura son la principal causa de la rotura de pines, remaches, tornillos, entre otras piezas mecánicas utilizadas para sostener o unir piezas. En el siguiente video puedes ver un test de esfuerzo cortante del pegamento que une dos laminas metálicas.

```{iframe} https://www.youtube.com/embed/z-cKD2LgEJk?si=lRlMdSqGCfwx3JA2
:width: 100%
:align: center
Video 1.  Ensayo de esfuerzo cortante de un pegamento
```

## Esfuerzo cortante

Las fuerzas que actúan sobre un cuerpo pueden descomponerse tanto en una dirección normal como en una dirección tangente o cortante al área sobre la que actúa, originando esfuerzos normales y esfuerzos cortantes respectivamente, tal como se observa en la figura.

```{figure} https://i0.wp.com/jesuscapistran.com/wp-content/uploads/2021/08/Screen-Shot-2021-08-19-at-17.33.53.png
:alt: Esfuerzo normal y cortante
:width: 300px
:align: center
Figura 1.  Esfuerzo Normal y Esfuerzo Cortante
```
El esfuerzo cortante $\sigma_c$ es la fuerza cortante por unidad de área y se mide en pascales (Pa).  

$$\sigma_c =\frac{dF_t}{dA}$$

## Ley de Hooke para la cizalla

Considera un bloque formado por laminas o planos paralelos, se aplican un par de fuerzas iguales y opuestas en los planos de arriba y abajo, estas fuerzas producen esfuerzos cortantes que deforman el bloque, haciendo que los planos deslicen unos sobre el otro. El desplazamiento horizontal máximo que experimenta el plano de arriba con respecto al plano de abajo es proporcional al esfuerzo cortante.

$$\sigma_c =G \, \frac{\Delta x}{l}$$

Donde 

$G$ = módulo de cizalla (Pa).  

$\Delta x$ = desplazamiento máximo del plano superior con respecto al plano inferior.  

$l$ = posición o altura del plano superior con respecto al plano inferior.  

La ecuación anterior tambien puede expresarse como:  

$$\sigma_c =G \, \phi $$

```{figure} https://github.com/jnolorbe/fisica2/blob/main/figuras/cizalla02.png
:alt: Esfuerzo y deformación cortante
:width: 300px
:align: center
Figura 2.  Esfuerzo cortante y deformación
```

## Problemas Resueltos
---
```{admonition} Problema 1: Análisis de Esfuerzo Cortante en Uniones Asimétricas 💡
:class: important

Este problema está basado en el ensayo de laboratorio **"Bolt Shear Test #1"**, donde se analiza el comportamiento de una unión de pletinas bajo carga de tracción con una distribución desigual de pernos. En el video referencial, se observa una prueba de tracción sobre dos pletinas unidas por pernos de acero. La configuración presenta una asimetría crítica:
* **Sección A (Superior):** 4 pernos.
* **Sección B (Inferior):** 2 pernos.

    ```{iframe} https://www.youtube.com/embed/is9DQOakQhs?si=th9RS-98fWZCsl53
    :width: 100%
    :align: center
    Video 2. Ensayo de esfuerzo cortante de un pegamento
    ```
Se desea determinar la capacidad de carga de una unión de dos pletinas de acero sujetas a una fuerza de tracción $P$. La unión se realiza mediante 6 pernos de $1/2$ pulgada de diámetro ($d \approx 12.7 \text{ mm}$), distribuidos de forma asimétrica (4 arriba y 2 abajo).

Considerando que el material de los pernos tiene un **esfuerzo de fluencia cortante** de $\tau_{f} = 250 \text{ MPa}$:

1. **Analizar** el efecto de la distribución de carga por cada perno e **Identificar** razonadamente qué sección de la unión fallará primero.
2. **Calcular** la carga máxima $P$ que puede aplicarse a la estructura antes de que ocurra la falla por cizalladura de los pernos.

```
```{admonition} Solución
:class: dropdown hint

### 1. Análisis de la Sección Crítica
Para que la unión esté en equilibrio, la fuerza total de tracción $P$ debe ser transmitida íntegramente a través de ambas secciones de pernos. 

* En la **sección de 4 pernos**, cada perno soporta una fuerza $F_4 = \frac{P}{4}$.
* En la **sección de 2 pernos**, cada perno soporta una fuerza $F_2 = \frac{P}{2}$.

Dado que el esfuerzo cortante es $\tau = \frac{F}{A}$ y el área $A$ es la misma para todos, el esfuerzo en los pernos de la sección inferior es el doble ($\tau_2 = 2\tau_4$). Por lo tanto, **la falla ocurrirá inevitablemente en la sección de 2 pernos**.

### 2. Cálculo de la Carga Máxima ($P_{max}$)

**1. Área de la sección transversal de un perno ($A$):**
Convertimos el diámetro a metros ($d = 0.0127 \text{ m}$):

$A = \frac{\pi \cdot d^2}{4} = \frac{\pi \cdot (0.0127 \text{ m})^2}{4} \approx 1.2667 \times 10^{-4} \text{ m}^2$

**2. Condición de falla en la sección inferior ($n = 2$):**
El esfuerzo actuante no debe superar el esfuerzo de fluencia ($\tau \leq \tau_{f}$):

$\tau_{f} = \frac{P_{max}}{n \cdot A}$

**3. Despeje de la carga $P$:**

$P_{max} = \tau_{f} \cdot (2 \cdot A)$

$P_{max} = (250 \times 10^6 \text{ Pa}) \cdot (2 \cdot 1.2667 \times 10^{-4} \text{ m}^2)$

$P_{max} = 63,335 \text{ N}$

**Resultado:** La carga máxima que puede soportar la unión es de aproximadamente **$63.34 \text{ kN}$**.

```
---

```{admonition} Problema 2: Acoplamiento Motor-Generador (Análisis de Torsión) 💡
:class: important

En la figura se muestra un sistemas de ejes escalonados que transmiten potencia. En la práctica industrial, un motor eléctrico entrega un torque constante a un generador. Si el eje es demasiado delgado o los pernos de acoplamiento son insuficientes, el sistema fallará por cizalladura antes de alcanzar la potencia de diseño.

:::{figure} https://github.com/jnolorbe/fisica2/blob/main/figuras/pd2_prob4.png
:alt: Acoplamiento Motor - Generador
:width: 60%
:align: center
Figura 3. Acoplamiento Motor - Generador
:::

**Situación Problemática**

Un motor acoplado a un generador transmite un torque de **$1500 \text{ lb}\cdot\text{ft}$**. El eje de transmisión es de acero macizo con un diámetro de **$3 \text{ pulgadas}$** y una longitud de **$5 \text{ pies}$**. Para unir el eje al generador, se utiliza una brida con **6 pernos** de **$0.5 \text{ pulgadas}$** de diámetro, ubicados a una distancia radial de **$4 \text{ pulgadas}$** del centro. Módulo de rigidez del acero: $G = 12 \times 10^6 \text{ psi}$

**Retos de Análisis:**

1.  **Integridad del Eje:** Calcule el esfuerzo cortante máximo en la superficie del eje. Si el acero falla a los $10 \text{ ksi}$ por cizalla, ¿es seguro este diámetro?
2.  **Deformación Operativa:** Determine el ángulo de giro ($\phi$) en grados que experimenta el eje.
3.  **Análisis de la Brida:** Calcule el esfuerzo cortante promedio en cada uno de los 6 pernos. ¿Qué sucede con este esfuerzo si el radio del círculo de pernos se reduce a la mitad?

```
```{admonition} Solución Comentada
:class: dropdown hint

**1. Esfuerzo Cortante Máximo en el Eje:**
Aplicamos la relación directa para ejes circulares:
* $T = 1500 \text{ lb}\cdot\text{ft} \times 12 = 18,000 \text{ lb}\cdot\text{in}$
* $d = 3 \text{ in}$

$\tau_{max} = \frac{16 \cdot (18,000 \text{ lb}\cdot\text{in})}{\pi \cdot (3 \text{ in})^3}$

$\tau_{max} \approx 3,395.3 \text{ psi} \approx 3.4 \text{ ksi}$

**Análisis:** Como $3.4 \text{ ksi} < 10 \text{ ksi}$, el eje trabaja en un rango seguro con un factor de seguridad considerable.

**2. Ángulo de Giro ($\phi$):**
Aplicamos la relación directa para ejes circulares macizos:

$\phi = \frac{32 \cdot T \cdot L}{G \cdot \pi \cdot d^4}$

Sustituyendo los valores:

$\phi = \frac{32 \cdot (18,000) \cdot (60)}{(12 \times 10^6) \cdot \pi \cdot (3^4)}$

$\phi = \frac{34,560,000}{(12 \times 10^6) \cdot \pi \cdot 81}$

$\phi = \frac{34,560,000}{3,053,628,059} \approx 0.01131 \text{ rad}$

Convertimos a grados:

$\phi_{grados} = 0.0113 \cdot \left(\frac{180}{\pi}\right) \approx 0.65^\circ$

**3. Cizalladura en los Pernos de la Brida**

-  **Fuerza de corte total ($F$):** Se obtiene del torque dividido por el radio de ubicación de los pernos ($R = 4 \text{ in}$).
    $F = \frac{T}{R} = \frac{18,000 \text{ lb}\cdot\text{in}}{4 \text{ in}} = 4,500 \text{ lb}$
-  **Fuerza por perno ($V$):** $V = \frac{4,500}{6} = 750 \text{ lb}$ por perno.
-  **Esfuerzo en el perno:** Con $d_p = 0.5 \text{ in}$, el área es $A \approx 0.196 \text{ in}^2$.
    $\tau_{perno} = \frac{750 \text{ lb}}{0.196 \text{ in}^2} \approx 3,826 \text{ psi} \approx 3.83 \text{ ksi}$

**4. Metacognición y Transferencia**

* **Pregunta de reflexión:** Si comparas el esfuerzo en el eje ($3.4 \text{ ksi}$) con el esfuerzo en los pernos ($3.83 \text{ ksi}$), ¿cuál componente fallaría primero ante una sobrecarga?
* **Aumentación con IA:** Pide a un modelo de lenguaje que explique: *"¿Cómo cambia el ángulo de giro si el eje fuera hueco pero mantuviera el mismo diámetro exterior?"*. Comenta su respuesta basándote en lo aprendido sobre la distribución de esfuerzos en el radio exterior.
```
---

```{admonition} Problema 3: Ejes acoplados (Análisis de Torsión) 💡
:class: important

En un sistema de control de posición de una antena parabólica, se utilizan dos ejes de acero macizo ($G = 80 \text{ GPa}$) conectados por engranajes en el punto $C$. El eje $AD$ tiene un diámetro $d_A = 40 \text{ mm}$ y el eje $BE$ tiene un diámetro $d_B = 30 \text{ mm}$. El radio del engranaje $A$ es $r_A = 100 \text{ mm}$ y el del engranaje $B$ es $r_B = 50 \text{ mm}$. Se aplica un torque de entrada en el extremo $E$ de $T_E = 150 \text{ Nm}$. Ambos ejes tienen una longitud $L = 0.8 \text{ m}$.

:::{figure} https://github.com/jnolorbe/fisica2/blob/main/figuras/pd2_prob5.png
:alt: Ejes Acoplados
:width: 50%
:align: center
Figura 4. Ejes Acoplados (Beer - Johnston - Dewolf - Mazurek. _Mechanic of Materials_)
:::


**Reto:** Determine el esfuerzo cortante máximo en cada eje y el ángulo de giro total en el extremo $E$ respecto al soporte fijo $D$.

```
```{admonition} Solución Paso a Paso
:class: dropdown hint

**1. Análisis de Torques (Equilibrio):**

El torque aplicado en el eje $BE$ se transmite al eje $AD$ a través de los engranajes. La fuerza de contacto en los dientes es la misma.

1. **Torque en el eje B:** $T_B = 150 \text{ N}\cdot\text{m}$.
2. **Fuerza tangencial (F):** $F = T_B / r_B = 150 / 0.05 = 3000 \text{ N}$.
3. **Torque transmitido al eje A:** $T_A = F \cdot r_A = 3000 \cdot 0.10 = 300 \text{ N}\cdot\text{m}$.

**2. Esfuerzos Cortantes Máximos:**

Utilizamos la relación: $\tau_{max} = \frac{16T}{\pi d^3}$

* **Eje AD ($d = 0.04 \text{ m}$):**

  $\tau_A = \frac{16 \cdot 300}{\pi \cdot (0.04)^3} \approx 23.87 \text{ MPa}$

* **Eje BE ($d = 0.03 \text{ m}$):**
  
  $\tau_B = \frac{16 \cdot 150}{\pi \cdot (0.03)^3} \approx 28.29 \text{ MPa}$

**3. Ángulos de Giro ($\phi$):**

Utilizamos la relación: $\phi = \frac{32 T L}{G \pi d^4}$

* **Giro del eje AD (debido a la torsión propia):** 

    $\phi_A = \frac{32 \cdot 300 \cdot 0.8}{(80 \times 10^9) \cdot \pi \cdot (0.04)^4} \approx 0.0119 \text{ rad}$

* **Giro del engranaje B por acoplamiento:**
   
   Debido a que los engranajes están en contacto, el arco recorrido es el mismo ($S = r \phi$):
   $r_A \phi_A = r_B \phi_{B,acop} \implies \phi_{B,acop} = 0.0119 \cdot \left(\frac{100 \text{ mm}}{50 \text{ mm}}\right) = 0.0238 \text{ rad}$

* **Giro propio del eje BE (debido a su propia torsión):**

   $\phi_{B,tor} = \frac{32 \cdot 150 \cdot 0.8}{(80 \times 10^9) \cdot \pi \cdot (0.03)^4} \approx 0.0189 \text{ rad}$

* **Giro total en E:** El giro total es la suma del giro que "hereda" del primer eje más su propia deformación:
 
   $\phi_E = \phi_{B,acop} + \phi_{B,tor} = 0.0238 + 0.0189 = \mathbf{0.0427 \text{ rad } (\approx 2.45^\circ)}$
```
---
*Material preparado para Física 2 - FIEE UNAC*
