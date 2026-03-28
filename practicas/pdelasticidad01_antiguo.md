# Práctica Dirigida 1: Esfuerzos Normales
**Curso:** Física 2 (EG-209)  
**Facultad:** Ingeniería Eléctrica y Electrónica - UNAC  
**Docente:** Juan Neil Mendoza Nolorbe  

---

## 1. Diseño de Soportes para Líneas de Transmisión (Esfuerzo Normal)
**Contexto:** Se está evaluando el uso de tubos de acero huecos para actuar como soportes verticales en una subestación. El tubo debe resistir una carga de tracción axial de $400 \text{ kN}$ generada por el tensado de los conductores.

* **Especificaciones:** El diámetro interior del tubo es de $100 \text{ mm}$.
* **Limitación Técnica:** Para garantizar la seguridad estructural, el esfuerzo normal no debe superar los $120 \text{ MPa}$.
* **Reto:** Determine el diámetro exterior mínimo del tubo necesario para cumplir con la normativa.
* **Análisis Crítico:** ¿Cómo afectaría a la seguridad del poste si el material presentara porosidades internas que redujeran el área efectiva de la sección transversal en un 5%?

> **Resultado esperado:** $119.4 \text{ mm}$
---

## 2. Compresión en Núcleos de Transformadores (Materiales Compuestos)
**Contexto:** En el ensamblaje de un núcleo de potencia, se utiliza una barra de acero de $50 \text{ mm}$ de diámetro protegida por una carcasa de hierro fundido de $5 \text{ mm}$ de espesor. El conjunto tiene una longitud total de $2 \text{ m}$.

* **Situación:** Durante el ajuste mecánico, el conjunto se somete a una carga de compresión.
* **Reto:** Deduzca la carga total $P$ necesaria para comprimir la barra compuesta exactamente $0.8 \text{ mm}$.
* **Propiedades de los Materiales:**
    * Acero: $E = 200 \text{ GPa}$
    * Hierro Fundido: $E = 100 \text{ GPa}$
* **Análisis Crítico:** Si la carga se aplica de forma no uniforme, ¿cuál de los dos materiales corre mayor riesgo de alcanzar su límite elástico primero?

> **Resultado esperado:** $191.6 \text{ kN}$

---

## 3. Estabilidad de Cargas Pesadas (Sistemas Indeterminados)
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

> **Resultado esperado:** $22358.4 \text{ kg}$

---

## 4. Análisis de Desplazamiento en Sensores de Nivel
**Contexto:** Una barra rígida $AB$ se utiliza para transmitir el movimiento a dos sensores verticales. La barra está inicialmente horizontal. Se aplica una carga $P = 50 \text{ kN}$ en la posición indicada en la Figura.

:::{figure} https://mathalino.com/sites/default/files/images/213-given.jpg
:alt: dos varillas verticales
:width: 50%
:align: center
:::

* **Situación:** Las varillas de soporte tienen diferentes propiedades elásticas y longitudes.
* **Reto:** Deduzca el movimiento vertical (descenso) del punto donde se aplica la carga $P$.
* **Aumentación con IA:** Ingrese la geometría del problema en una IA y pregunte: *"¿En qué punto de la barra AB debería colocarse la carga P para que el descenso sea uniforme y la barra permanezca horizontal?"*. Analice la importancia del "centro de rigidez" en este escenario.

> **Resultado esperado:** $1.87 \text{ mm}$

---


5. Una varilla esta compuesta por tres varillas de aluminio, acero y bronce, tal como se muestra en la Figura P-108. Se aplican cargas axiales en las posiciones indicadas. Deducir el valor máximo de $P$ en $kN$ tal que el esfuerzo máxima no supere $140 \text{ MPa}$ en el acero, $90 \text{ MPa}$ en el aluminio o $100 \text{ MPa}$ en el bronce. 

:::{figure} https://mathalino.com/sites/default/files/reviewer-strength/01-stress/108-composite-bar-different-area.gif
:alt: barra compuesta aluminio acero bronce
:width: 50%
:align: center
:::
_Respuesta:_ $ 10 \text{ kN}$

## Referencias:
- https://mathalino.com

