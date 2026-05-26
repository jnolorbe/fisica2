# Sesión 5: Hidrostática

## 📌 I. Fundamento Teórico

En esta sesión se estudia el comportamiento de fluidos en reposo, analizando la distribución de presión en el interior de un fluido, las fuerzas que ejerce sobre superficies sumergidas, y los principios de Pascal y Arquímedes que fundamentan máquinas hidráulicas y la flotación de cuerpos.

---

### 1.1. Presión Hidrostática. Ecuación Fundamental de la Hidrostática

**Presión:** Fuerza normal por unidad de área ejercida por un fluido.

$$P = \frac{F}{A}$$

Unidades: Pa (Pascal) = N/m², atm, bar, mmHg, psi.

**Ecuación fundamental de la hidrostática:**

Para un fluido incompresible en reposo, la presión aumenta linealmente con la profundidad:

$$P = P_0 + \rho g h$$

donde:
* $P_0$: presión en la superficie libre
* $\rho$: densidad del fluido
* $g$: aceleración de la gravedad
* $h$: profundidad medida desde la superficie

**Diferencial de presión (forma general):**

$$\frac{dP}{dy} = -\rho g$$

El signo negativo indica que la presión disminuye al ascender ($y$ positivo hacia arriba).

> **💡 Regla de Oro:** La presión en un punto de un fluido en reposo es la misma en todas las direcciones (isotropía de la presión). La presión depende solo de la profundidad, no de la forma del recipiente.

---

### 1.2. Presión Atmosférica. El Barómetro

**Presión atmosférica estándar:**

$$P_{atm} = 1 \text{ atm} = 101325 \text{ Pa} = 760 \text{ mmHg} = 1013.25 \text{ mbar}$$

**Barómetro de mercurio (Torricelli, 1643):**

Un tubo lleno de mercurio invertido en una cubeta. La columna de Hg se equilibra con la presión atmosférica:

$$P_{atm} = \rho_{Hg} g h$$

A nivel del mar y 0°C: $h = 760$ mm.

**Variación de la presión atmosférica con la altitud:**

Para la atmósfera ideal (temperatura constante):

$$P = P_0 e^{-\frac{Mgh}{RT}}$$

donde $M$ es la masa molar del aire, $R$ la constante de los gases.

> **💡 Regla de Oro:** En Lima (a ~150 msnm), la presión atmosférica es aproximadamente 100.5 kPa, ligeramente menor que al nivel del mar. En el lago Titicaca (3812 msnm), desciende a ~64 kPa.

---

### 1.3. Manómetros de Tubos en Forma de U. Presión Manométrica

**Presión manométrica ($P_{man}$):** Diferencia entre la presión absoluta y la atmosférica.

$$P_{man} = P_{abs} - P_{atm}$$

**Manómetro de tubo en U:**

Dos fluidos inmiscibles en un tubo doblado. La diferencia de alturas $\Delta h$ está relacionada con la diferencia de presiones:

$$P_1 - P_2 = (\rho_2 - \rho_1) g \Delta h$$

Para un manómetro con un lado abierto a la atmósfera:

$$P_{man} = \rho g h$$

donde $h$ es la diferencia de niveles del fluido manométrico.

**Tipos de manómetros:**

| Tipo | Fluido manométrico | Rango típico |
|------|-------------------|--------------|
| Piezómetro | Agua | Presiones pequeñas |
| Manómetro de agua | Agua | Hasta ~10 kPa |
| Manómetro de mercurio | Mercurio | Hasta ~100 kPa |
| Manómetro diferencial | Aceite | Pequeñas diferencias de presión |

---

### 1.4. Fuerzas de Presión sobre Superficies Planas

**Fuerza hidrostática sobre una superficie plana sumergida:**

$$F = P_{cg} \cdot A = (P_0 + \rho g h_{cg}) \cdot A$$

donde $h_{cg}$ es la profundidad del centro de gravedad (centroide) de la superficie.

**Centro de presión:** Punto donde puede considerarse aplicada la fuerza resultante, siempre por debajo del centro de gravedad (excepto para superficies horizontales).

$$y_{cp} = y_{cg} + \frac{I_{cg}}{y_{cg} \cdot A}$$

donde $I_{cg}$ es el momento de inercia del área respecto al eje centroidal.

**Momentos de inercia para figuras comunes:**

| Figura | Área | $I_{cg}$ |
|--------|------|----------|
| Rectángulo ($b \times h$) | $bh$ | $\frac{bh^3}{12}$ |
| Círculo (radio $R$) | $\pi R^2$ | $\frac{\pi R^4}{4}$ |
| Triángulo ($b \times h$) | $\frac{bh}{2}$ | $\frac{bh^3}{36}$ |

---

### 1.5. Principio de Pascal. Máquinas Hidráulicas

**Principio de Pascal (1653):** La presión aplicada a un fluido confinado se transmite sin disminución a todos los puntos del fluido y a las paredes del recipiente.

$$\frac{F_1}{A_1} = \frac{F_2}{A_2} \Rightarrow F_2 = F_1 \cdot \frac{A_2}{A_1}$$

**Multiplicación de fuerzas:** Si $A_2 \gg A_1$, una fuerza pequeña $F_1$ genera una fuerza grande $F_2$.

**Prensa hidráulica:**

$$\frac{F_1}{A_1} = \frac{F_2}{A_2} = P$$

**Relación de desplazamientos:** Conservación de volumen:

$$A_1 d_1 = A_2 d_2 \Rightarrow d_2 = d_1 \cdot \frac{A_1}{A_2}$$

> **💡 Regla de Oro:** La prensa hidráulica multiplica fuerzas pero no energía. El trabajo $W = F \cdot d$ es el mismo en ambos pistones (idealmente): $F_1 d_1 = F_2 d_2$.

---

### 1.6. Principio de Arquímedes. Flotación de Cuerpos

**Principio de Arquímedes (250 a.C.):** Todo cuerpo sumergido en un fluido experimenta un empuje vertical hacia arriba igual al peso del fluido desalojado.

$$\vec{E} = \rho_{fluido} \, V_{sumergido} \, g \quad \text{(hacia arriba)}$$

**Condiciones de flotación:**

| Condición | Relación de densidades | Comportamiento |
|-----------|------------------------|----------------|
| $\rho_{cuerpo} > \rho_{fluido}$ | El cuerpo es más denso | Se hunde |
| $\rho_{cuerpo} = \rho_{fluido}$ | Densidades iguales | Equilibrio neutro |
| $\rho_{cuerpo} < \rho_{fluido}$ | El cuerpo es menos denso | Flota parcialmente sumergido |

**Fracción sumergida para un cuerpo flotante:**

$$\frac{V_{sum}}{V_{total}} = \frac{\rho_{cuerpo}}{\rho_{fluido}}$$

**Estabilidad de flotación:** Un cuerpo flota establemente si su centro de gravedad está por debajo del centro de carena (centro de gravedad del fluido desalojado), o si la metacentre está por encima del centro de gravedad.

> **💡 Regla de Oro:** El empuje actúa sobre el volumen efectivamente sumergido. Para un cuerpo parcialmente sumergido, solo se desaloja el volumen bajo la línea de flotación.

---

## 🚀 II. Problemas Resueltos

---

### 🧩 Problema N° 1

```{admonition} El Embalse de Tinajones
:class: important
**Situación:** La represa del embalse de Tinajones (Cajamarca, Perú) contiene agua hasta una altura máxima $H = 35$ m. La pared de la represa es vertical y tiene ancho $w = 120$ m. Calcular: (a) la presión en la base de la represa, (b) la fuerza hidrostática total sobre la pared, (c) la altura donde actúa la fuerza resultante (centro de presión), y (d) la presión a 15 m de profundidad.
```

```{admonition} Solución
:class: dropdown hint
**1. Planteamiento:**
* **Ruta de la solución:** Aplicar la ecuación fundamental de la hidrostática para la presión. La fuerza sobre la pared vertical requiere integrar la presión variable sobre el área rectangular. El centro de presión de una pared rectangular está a 1/3 de la altura desde la base.
* **Predicción cualitativa:** La presión en la base será de ~3.5 atm (350 kPa). La fuerza total será enorme (millones de newtons) debido al gran ancho de la represa.

**2. Resolución:**

**Datos:**
* $\rho_{agua} = 1000$ kg/m³
* $g = 9.8$ m/s²
* $H = 35$ m, $w = 120$ m
* $P_{atm} = 101325$ Pa

**(a) Presión en la base:**
$$P_{base} = P_{atm} + \rho g H = 101325 + 1000 \times 9.8 \times 35$$
$$P_{base} = 101325 + 343000 = 444325 \text{ Pa} \approx 444.3 \text{ kPa} \approx 4.38 \text{ atm}$$

**(b) Fuerza hidrostática total:**

La presión varía con la profundidad: $P(y) = P_{atm} + \rho g (H - y)$ donde $y$ se mide desde la superficie.

La fuerza manométrica (que es la que solicita la estructura) es:
$$F_{man} = \int_0^H \rho g (H-y) \cdot w \, dy = \rho g w \int_0^H (H-y) dy$$

$$F_{man} = \rho g w \left[Hy - \frac{y^2}{2}\right]_0^H = \rho g w \cdot \frac{H^2}{2}$$

$$F_{man} = 1000 \times 9.8 \times 120 \times \frac{35^2}{2} = 1000 \times 9.8 \times 120 \times 612.5$$

$$F_{man} = 720300000 \text{ N} = 7.20 \times 10^8 \text{ N} \approx 720 \text{ MN}$$

Fuerza total incluyendo atmósfera:
$$F_{total} = F_{man} + P_{atm} \cdot A = 7.20 \times 10^8 + 101325 \times (120 \times 35)$$
$$F_{total} = 7.20 \times 10^8 + 4.26 \times 10^8 = 1.15 \times 10^9 \text{ N}$$

> **Nota:** La presión atmosférica actúa también en la cara exterior de la represa, por lo que la fuerza neta debida a la atmósfera se cancela. Solo la presión manométrica solicita la estructura.

**(c) Centro de presión:**

Para una superficie rectangular vertical con el borde superior en la superficie libre:

$$y_{cp} = \frac{2}{3}H \text{ medido desde la superficie}$$

o equivalentemente:
$$h_{cp} = \frac{H}{3} = \frac{35}{3} \approx 11.67 \text{ m desde la base}$$

Verificación con fórmula general:
$$y_{cg} = \frac{H}{2} = 17.5 \text{ m (desde la superficie)}$$
$$I_{cg} = \frac{wH^3}{12} = \frac{120 \times 35^3}{12} = 428750 \text{ m}^4$$
$$A = wH = 120 \times 35 = 4200 \text{ m}^2$$

$$y_{cp} = 17.5 + \frac{428750}{17.5 \times 4200} = 17.5 + 5.83 = 23.33 \text{ m (desde superficie)}$$

Desde la base: $35 - 23.33 = 11.67$ m. **Verificado.**

**(d) Presión a 15 m de profundidad:**
$$P = P_{atm} + \rho g h = 101325 + 1000 \times 9.8 \times 15$$
$$P = 101325 + 147000 = 248325 \text{ Pa} \approx 248.3 \text{ kPa} \approx 2.45 \text{ atm}$$

**3. Discusión Crítica:**
* La forma trapezoidal de las represas reales (mayor ancho en la base) resiste mejor la presión hidrostática que una pared vertical. La presión crece linealmente con la profundidad, pero la fuerza crece con el cuadrado de la altura de agua.
* El centro de presión a 1/3 de la altura desde la base implica que la mitad inferior de la represa soporta 5/6 de la fuerza total (la presión es mayor en la parte baja).
* Las represas modernas incluyen galerías de drenaje para reducir la presión de poros en el concreto y evitar filtraciones que debiliten la estructura.

**4. Análisis de Sensibilidad:**
| Parámetro | Cambio | Efecto en fuerza manométrica |
|-----------|--------|------------------------------|
| Nivel de agua $H$ | +10% | Fuerza +21% ($\propto H^2$) |
| Ancho de represa $w$ | +10% | Fuerza +10% (lineal) |
| Densidad del agua | +3% (sedimentos) | Fuerza +3% (lineal) |

**5. Extensión:**
El embalse de Tinajones (completado en 1989) tiene una capacidad de 320 millones de m³. El análisis de presiones hidrostáticas es fundamental en el diseño de presas de gravedad (resisten por su peso) y presas de arco (transfieren la presión a los flancos del cañón). La presa de Huascacocha (Junín) y la futura presa de Río Grande (Lambayeque) requieren modelos de presión que incluyan sismicidad y crecidas extremas por El Niño.
```
---

### 🧩 Problema N° 2

```{admonition} El Barómetro de Torricelli en el Callao
:class: important
**Situación:** Un estudiante construye un barómetro de Torricelli en el Callao (a nivel del mar, $P_{atm} = 101.3$ kPa) usando mercurio ($\rho_{Hg} = 13600$ kg/m³). Después lo traslada a Cerro de Pasco (4330 msnm) donde la presión atmosférica es $P = 61.5$ kPa. Calcular: (a) la altura de la columna de mercurio en ambas ubicaciones, (b) la altura si usara agua en lugar de mercurio en Lima, (c) la razón entre las densidades del aire en ambas ciudades asumiendo temperatura constante, y (d) la fuerza que ejerce la atmósfera sobre una mesa de $2$ m² en Lima.
```

```{admonition} Solución
:class: dropdown hint
**1. Planteamiento:**
* **Ruta de la solución:** Aplicar el equilibrio hidrostático en el barómetro: la presión atmosférica equilibra la columna de líquido. Para el agua, la altura será mucho mayor debido a su menor densidad. La densidad del aire se relaciona con la presión a temperatura constante.
* **Predicción cualitativa:** La columna de Hg en Cerro de Pasco será ~60% de la de Lima. El barómetro de agua requeriría más de 10 m de tubo, impráctico para uso común.

**2. Resolución:**

**(a) Altura de mercurio:**

**En Lima (Callao):**
$$h_{Lima} = \frac{P_{atm}}{\rho_{Hg} g} = \frac{101300}{13600 \times 9.8} = \frac{101300}{133280} \approx 0.760 \text{ m} = 760 \text{ mm}$$

**En Cerro de Pasco:**
$$h_{Cerro} = \frac{61500}{13600 \times 9.8} = \frac{61500}{133280} \approx 0.461 \text{ m} = 461 \text{ mm}$$

**(b) Barómetro de agua en Lima:**
$$h_{agua} = \frac{P_{atm}}{\rho_{agua} g} = \frac{101300}{1000 \times 9.8} = \frac{101300}{9800} \approx 10.34 \text{ m}$$

> **Nota:** Un barómetro de agua requeriría un tubo de más de 10 m de altura, lo que lo hace impráctico. Por eso Torricelli usó mercurio, 13.6 veces más denso.

**(c) Razón de densidades del aire:**

A temperatura constante, de la ley de los gases ideales $PV = nRT$:
$$\frac{P_1}{\rho_1} = \frac{P_2}{\rho_2} = \frac{RT}{M} = \text{constante}$$

$$\frac{\rho_{Cerro}}{\rho_{Lima}} = \frac{P_{Cerro}}{P_{Lima}} = \frac{61.5}{101.3} \approx 0.607$$

El aire en Cerro de Pasco es ~40% menos denso que en Lima.

**(d) Fuerza sobre la mesa en Lima:**
$$F = P_{atm} \times A = 101325 \times 2 = 202650 \text{ N} \approx 202.7 \text{ kN}$$

Equivalente a una masa de:
$$m = \frac{F}{g} = \frac{202650}{9.8} \approx 20679 \text{ kg} \approx 20.7 \text{ toneladas}$$

> **Asombroso:** La atmósfera ejerce una fuerza de ~20 toneladas sobre una mesa de 2 m², equilibrada por una fuerza igual hacia arriba en la cara inferior.

**3. Discusión Crítica:**
* El barómetro de mercurio es preciso pero tóxico. Los barómetros modernos usan sensores piezoeléctricos o de capacitancia, sin líquidos peligrosos.
* La disminución de presión con la altitud explica por qué el agua hierde a menor temperatura en la sierra (85-90°C en Cerro de Pasco vs. 100°C en Lima), afectando los tiempos de cocción.
* La presión atmosférica varía también con el clima: un día soleado en Lima puede tener 101.5 kPa, mientras que un día nublado de garúa baja a 100.8 kPa.

**4. Análisis de Sensibilidad:**
| Parámetro | Variación | Efecto en altura de Hg |
|-----------|-----------|------------------------|
| Presión atmosférica | -1 kPa | -7.5 mm |
| Temperatura del Hg | +10°C | -1.2 mm (dilatación térmica) |
| Gravedad local | -0.5% (altura) | +3.8 mm |

**5. Extensión:**
La aviación utiliza altímetros barométricos que miden presión y la convierten a altitud usando la atmósfera estándar internacional (ISA). Los buzos usan computadoras de buceo que calculan la presión ambiente para determinar tiempos de descompresión. En medicina hiperbárica, cámaras a 2-3 atm tratan enfermedad por descompresión y intoxicación por CO.
```
---

### 🧩 Problema N° 3

```{admonition} El Manómetro del Sistema de Refrigeración
:class: important
**Situación:** Un técnico de HVAC mide la presión en un sistema de refrigeración con un manómetro de tubo en U que contiene aceite manométrico ($\rho_{aceite} = 850$ kg/m³). El lado conectado al sistema muestra un nivel 45 cm más bajo que el lado abierto a la atmósfera. Calcular: (a) la presión manométrica del sistema, (b) la presión absoluta si $P_{atm} = 100$ kPa, (c) la altura equivalente si el manómetro usara agua, y (d) la lectura si el sistema estuviera al vacío relativo (presión menor que atmosférica) con la misma diferencia de 45 cm.
```

```{admonition} Solución
:class: dropdown hint
**1. Planteamiento:**
* **Ruta de la solución:** En un manómetro de tubo en U, la diferencia de presiones equilibra la columna de fluido manométrico. El lado con nivel más bajo tiene mayor presión. La presión manométrica se calcula directamente de $\rho g h$.
* **Predicción cualitativa:** El sistema está a sobrepresión (presión > atmosférica) porque el nivel del lado del sistema está más bajo. El aceite, menos denso que el agua, requerirá mayor altura para la misma presión.

**2. Resolución:**

**Datos:**
* $\rho_{aceite} = 850$ kg/m³
* $h = 0.45$ m
* $g = 9.8$ m/s²
* $P_{atm} = 100000$ Pa

**(a) Presión manométrica:**
El lado del sistema tiene nivel más bajo: $P_{sistema} > P_{atm}$

$$P_{man} = \rho_{aceite} g h = 850 \times 9.8 \times 0.45$$
$$P_{man} = 3748.5 \text{ Pa} \approx 3.75 \text{ kPa} \approx 0.037 \text{ atm}$$

**(b) Presión absoluta:**
$$P_{abs} = P_{atm} + P_{man} = 100000 + 3748.5 = 103748.5 \text{ Pa} \approx 103.75 \text{ kPa}$$

**(c) Altura equivalente con agua:**
Misma presión manométrica, diferente densidad:
$$\rho_{aceite} g h_{aceite} = \rho_{agua} g h_{agua}$$

$$h_{agua} = h_{aceite} \times \frac{\rho_{aceite}}{\rho_{agua}} = 0.45 \times \frac{850}{1000} = 0.45 \times 0.85 = 0.3825 \text{ m} = 38.25 \text{ cm}$$

> **Verificación:** El agua, más densa, necesita menor altura para equilibrar la misma presión. 38.25 cm de agua = 45 cm de aceite.

**(d) Lectura al vacío relativo:**
Si el sistema estuviera al vacío (presión < atmosférica), el nivel del lado del sistema estaría más alto que el abierto. La diferencia de 45 cm indicaría:

$$P_{man} = -\rho_{aceite} g h = -3748.5 \text{ Pa} \approx -3.75 \text{ kPa}$$

$$P_{abs} = 100000 - 3748.5 = 96251.5 \text{ Pa} \approx 96.25 \text{ kPa}$$

En unidades de vacío: $3.75$ kPa de vacío, o en mmHg: $\frac{3750}{133.3} \approx 28.1$ mmHg de vacío.

**3. Discusión Crítica:**
* Los manómetros de aceite se usan en refrigeración porque el aceite no reacciona con los refrigerantes halogenados (R-134a, R-410A). El agua o el mercurio podrían contaminar el sistema.
* La presión manométrica de 3.75 kPa es típica de un sistema de aire acondicionado en operación normal. En carga de refrigerante, los técnicos usan manómetros de alta precisión (±0.5 kPa).
* El "vacío" en refrigeración no es vacío absoluto (0 Pa), sino presión por debajo de la atmosférica. Un vacío profundo en HVAC es ~-100 kPa (prácticamente 0 Pa absoluto).

**4. Análisis de Sensibilidad:**
| Parámetro | Variación | Efecto en lectura |
|-----------|-----------|-------------------|
| Densidad del aceite | +5% (contaminación) | Lectura +5% (sobreestima presión) |
| Ángulo del tubo | 10° de inclinación | Error de paralaje ±2% |
| Temperatura ambiente | +20°C | Densidad del aceite -2%, lectura -2% |

**5. Extensión:**
Los sistemas de refrigeración automotriz usan manómetros de alta y baja presión simultáneamente. La relación entre ambas presiones indica el estado de carga del refrigerante. En plantas industriales de amoníaco (R-717), los manómetros usan glicerina como fluido amortiguador para proteger el mecanismo de vibraciones. Los transmisores de presión electrónicos (4-20 mA) reemplazan gradualmente los manómetros mecánicos en automatización industrial.
```
---

### 🧩 Problema N° 4

```{admonition} La Compuerta del Canal de Chavimochic
:class: important
**Situación:** El canal de regadio Chavimochic (La Libertad) tiene una compuerta rectangular de $b = 3$ m de ancho y $h = 2.5$ m de altura, inclinada 30° respecto a la horizontal. El agua alcanza la mitad superior de la compuerta (nivel hasta 1.25 m medido verticalmente desde la bisagra inferior). Calcular: (a) la fuerza hidrostática resultante sobre la compuerta, (b) el centro de presión medido desde la bisagra, (c) el torque que debe vencer el mecanismo de apertura, y (d) la fuerza mínima de un actuador hidráulico aplicado en el centro de la compuerta para equilibrar el torque hidrostático.
```

```{admonition} Solución
:class: dropdown hint
**1. Planteamiento:**
* **Ruta de la solución:** La superficie inclinada requiere proyectar la profundidad vertical sobre la normal a la superficie. El centro de gravedad de la porción sumergida determina la fuerza promedio. El torque se calcula respecto a la bisagra usando el brazo de palanca desde el centro de presión.
* **Predicción cualitativa:** La fuerza será menor que si la compuerta estuviera vertical porque la profundidad promedio es menor. El centro de presión estará por debajo del centro geométrico debido al gradiente de presión.

**2. Resolución:**

**Datos:**
* $b = 3$ m (ancho)
* $h_{total} = 2.5$ m (altura de compuerta)
* $\theta = 30°$ (inclinación respecto a horizontal)
* Nivel de agua: $H = 1.25$ m (vertical desde bisagra inferior)
* $\rho = 1000$ kg/m³, $g = 9.8$ m/s²

**(a) Fuerza hidrostática:**

Longitud sumergida medida a lo largo de la compuerta:
$$L_{sum} = \frac{H}{\sin\theta} = \frac{1.25}{\sin(30°)} = \frac{1.25}{0.5} = 2.5 \text{ m}$$

Profundidad del centro de gravedad (vertical):
$$h_{cg} = \frac{H}{2} = \frac{1.25}{2} = 0.625 \text{ m}$$

Área sumergida:
$$A = b \times L_{sum} = 3 \times 2.5 = 7.5 \text{ m}^2$$

Fuerza:
$$F = \rho g h_{cg} \times A = 1000 \times 9.8 \times 0.625 \times 7.5$$
$$F = 45937.5 \text{ N} \approx 45.94 \text{ kN}$$

**(b) Centro de presión desde la bisagra:**

Para una superficie rectangular con el borde superior en la superficie libre:
$$y_{cp} = \frac{2}{3}L_{sum} \text{ medido desde la superficie libre}$$

Desde la bisagra (borde inferior):
$$d_{cp} = L_{sum} - \frac{2}{3}L_{sum} = \frac{1}{3}L_{sum} = \frac{2.5}{3} \approx 0.833 \text{ m}$$

Verificación con fórmula general:
$$y_{cg} = \frac{L_{sum}}{2} = 1.25 \text{ m (desde superficie)}$$
$$I_{cg} = \frac{bL_{sum}^3}{12} = \frac{3 \times 2.5^3}{12} = \frac{46.875}{12} = 3.906 \text{ m}^4$$

$$y_{cp} = 1.25 + \frac{3.906}{1.25 \times 7.5} = 1.25 + 0.417 = 1.667 \text{ m (desde superficie)}$$

Desde la bisagra: $2.5 - 1.667 = 0.833$ m. **Verificado.**

**(c) Torque respecto a la bisagra:**
$$\tau = F \times d_{cp} = 45937.5 \times 0.833 \approx 38264 \text{Nm} \approx 38.3 \text{ kNm}$$

**(d) Fuerza del actuador hidráulico:**

El actuador se aplica en el centro geométrico de la compuerta, a distancia desde la bisagra:
$$d_{act} = \frac{L_{sum}}{2} = 1.25 \text{ m}$$

Para equilibrar el torque:
$$F_{act} \times d_{act} = \tau$$
$$F_{act} = \frac{38264}{1.25} = 30611 \text{ N} \approx 30.6 \text{ kN}$$

> **Nota:** En la práctica, se usa un factor de seguridad de 1.5-2.0, requiriendo un actuador de ~50-60 kN.

**3. Discusión Crítica:**
* La inclinación de 30° reduce la fuerza respecto a una compuerta vertical con la misma altura de agua porque la profundidad promedio es menor. Sin embargo, el brazo de palanca desde la bisagra es mayor, compensando parcialmente.
* Las compuertas reales de Chavimochic usan mecanismos de husillo o cilindros hidráulicos con acumuladores de energía para operación de emergencia ante cortes eléctricos.
* El torque hidrostático varía con el cuadrado del nivel de agua: si el nivel se duplica, la fuerza se cuadruplica y el centro de presión se desplaza, cambiando el brazo de palanca.

**4. Análisis de Sensibilidad:**
| Parámetro | Cambio | Efecto en torque |
|-----------|--------|------------------|
| Nivel de agua $H$ | +20% | Torque +73% ($\propto H^3$ aprox.) |
| Ángulo de inclinación | +10° (más vertical) | Fuerza +8%, brazo -5%, torque neto +2% |
| Ancho de compuerta $b$ | +50% | Torque +50% (lineal) |

**5. Extensión:**
El proyecto Chavimochic transfiere agua del río Santa hacia valles áridos de La Libertad, usando compuertas de control de flujo de hasta 6 m de ancho. Las compuertas Tainter (segmento circular) son preferidas en grandes presas porque el centro de presión pasa cerca del eje de rotación, minimizando el torque de apertura. La presa de Aswan (Egipto) tiene compuertas de 50 toneladas que operan con gatos hidráulicos de 500 kN.
```
---

### 🧩 Problema N° 5

```{admonition} La Prensa Hidráulica del Taller Mecánico
:class: important
**Situación:** Un taller mecánico en Lima tiene una prensa hidráulica con pistón pequeño de diámetro $d_1 = 4$ cm y pistón grande de diámetro $d_2 = 30$ cm. El sistema usa aceite hidráulico ($\rho = 900$ kg/m³). Calcular: (a) la relación de multiplicación de fuerzas, (b) la fuerza máxima en el pistón grande si un operario aplica $F_1 = 200$ N, (c) el desplazamiento del pistón grande si el pequeño desciende $h_1 = 20$ cm, (d) el trabajo realizado en ambos pistones (ideal), y (e) la presión manométrica en el aceite.

```

```{admonition} Solución
:class: dropdown hint
**1. Planteamiento:**
* **Ruta de la solución:** Aplicar el principio de Pascal: la presión se transmite igual en todo el fluido. Las áreas circulares dan la relación de multiplicación. La conservación del volumen relaciona los desplazamientos.
* **Predicción cualitativa:** La relación de áreas será $(30/4)^2 = 56.25$, transformando 200 N en ~11 kN. El desplazamiento será muy pequeño en el pistón grande.

**2. Resolución:**

**Áreas de los pistones:**
$$A_1 = \frac{\pi d_1^2}{4} = \frac{\pi \times (0.04)^2}{4} = 1.257 \times 10^{-3} \text{ m}^2$$
$$A_2 = \frac{\pi d_2^2}{4} = \frac{\pi \times (0.30)^2}{4} = 7.069 \times 10^{-2} \text{ m}^2$$

**(a) Relación de multiplicación:**
$$\frac{F_2}{F_1} = \frac{A_2}{A_1} = \frac{7.069 \times 10^{-2}}{1.257 \times 10^{-3}} = 56.25$$

**(b) Fuerza máxima en el pistón grande:**
$$F_2 = F_1 \times 56.25 = 200 \times 56.25 = 11250 \text{ N} = 11.25 \text{ kN}$$

Equivalente a levantar:
$$m = \frac{11250}{9.8} \approx 1148 \text{ kg} \approx 1.15 \text{ toneladas}$$

**(c) Desplazamiento del pistón grande:**
Conservación de volumen:
$$A_1 h_1 = A_2 h_2$$
$$h_2 = h_1 \times \frac{A_1}{A_2} = 0.20 \times \frac{1}{56.25} = 0.00356 \text{ m} = 3.56 \text{ mm}$$

> **Observación:** El pistón grande avanza solo 3.56 mm mientras el pequeño recorre 20 cm. Este es el "precio" de la multiplicación de fuerzas.

**(d) Trabajo realizado (ideal):**
$$W_1 = F_1 \times h_1 = 200 \times 0.20 = 40 \text{ J}$$
$$W_2 = F_2 \times h_2 = 11250 \times 0.00356 = 40 \text{ J}$$

> **Verificación:** $W_1 = W_2$ (sin pérdidas). La energía se conserva; solo se transforma fuerza en desplazamiento.

**(e) Presión manométrica en el aceite:**
$$P = \frac{F_1}{A_1} = \frac{200}{1.257 \times 10^{-3}} = 159154 \text{ Pa} \approx 159.2 \text{ kPa} \approx 1.57 \text{ atm}$$

Verificación con pistón grande:
$$P = \frac{F_2}{A_2} = \frac{11250}{7.069 \times 10^{-2}} = 159154 \text{ Pa}$$

**3. Discusión Crítica:**
* Las prensas hidráulicas reales tienen rendimientos del 80-90% debido a fugas, compresibilidad del aceite y fricción en sellos. La fuerza útil sería ~9-10 kN en lugar de 11.25 kN.
* La presión de 159 kPa es moderada. Las prensas industriales trabajan a 10-20 MPa (100-200 atm), requiriendo mangueras y cilindros de alta resistencia.
* El aceite hidráulico no se comprime apreciablemente a estas presiones (módulo de compresibilidad ~1.5 GPa), manteniendo la rigidez del sistema.

**4. Análisis de Sensibilidad:**
| Parámetro | Cambio | Efecto en $F_2$ |
|-----------|--------|-----------------|
| Diámetro del pistón grande | +10% | $F_2$ +21% ($\propto d^2$) |
| Fuerza aplicada $F_1$ | +10% | $F_2$ +10% (lineal) |
| Viscosidad del aceite | +50% (frío) | Pérdidas +15%, $F_2$ efectiva -15% |

**5. Extensión:**
Las prensas hidráulicas modernas usan sistemas de acumuladores de nitrógeno para proporcionar flujo rápido sin bombas grandes. Los frenos hidráulicos de automóviles usan el mismo principio: una fuerza pequeña en el pedal se multiplica por el diferencial de áreas entre el cilindro maestro y los cilindros de rueda. Los excavadoras y grúas usan circuitos hidráulicos a 30-40 MPa con control proporcional electrohidráulico para movimientos precisos.
```
---

### 🧩 Problema N° 6
```{admonition} La Balsa de los Pescadores de Puno

:class: important
**Situación:** Los pescadores del lago Titicaca usan balsas tradicionales de totora con forma de plataforma rectangular de $L = 4$ m, $W = 2$ m y espesor promedio $e = 0.5$ m. La totora tiene densidad $\rho_{totora} = 250$ kg/m³. Calcular: (a) el peso máximo de pescadores y carga que puede soportar sin hundirse, (b) la profundidad de hundimiento con 3 pescadores de 70 kg cada uno, (c) la fracción del volumen sumergido en esa condición, y (d) la estabilidad inicial si el centro de gravedad de los pescadores está a 0.3 m sobre la superficie de la balsa.

```

```{admonition} Solución
:class: dropdown hint
**1. Planteamiento:**
* **Ruta de la solución:** Aplicar el principio de Arquímedes: el empuje igual al peso del agua desalojada. En el límite de hundimiento, el volumen sumergido es el total de la balsa. La estabilidad requiere comparar la posición del centro de gravedad con el centro de carena.
* **Predicción cualitativa:** La totora, muy porosa y liviana, permite grandes cargas relativas. La balsa será estable porque el centro de gravedad de la totora está muy bajo (cerca de la línea de flotación).

**2. Resolución:**

**Datos:**
* $\rho_{totora} = 250$ kg/m³
* $\rho_{agua} = 1000$ kg/m³ (agua dulce del Titicaca, ligeramente menor que el mar)
* $L = 4$ m, $W = 2$ m, $e = 0.5$ m
* $g = 9.8$ m/s²

**Volumen total de la balsa:**
$$V_{total} = L \times W \times e = 4 \times 2 \times 0.5 = 4 \text{ m}^3$$

**Masa de la balsa:**
$$m_{balsa} = \rho_{totora} \times V_{total} = 250 \times 4 = 1000 \text{ kg}$$

**(a) Peso máximo de carga (límite de hundimiento):**

En el límite, el volumen sumergido es el total ($V_{sum} = V_{total} = 4$ m³).

Empuje máximo:
$$E_{max} = \rho_{agua} \times V_{total} \times g = 1000 \times 4 \times 9.8 = 39200 \text{ N}$$

Peso de la balsa:
$$W_{balsa} = m_{balsa} \times g = 1000 \times 9.8 = 9800 \text{ N}$$

Peso máximo de carga:
$$W_{carga,max} = E_{max} - W_{balsa} = 39200 - 9800 = 29400 \text{ N}$$

Masa máxima de carga:
$$m_{carga,max} = \frac{29400}{9.8} = 3000 \text{ kg}$$

> **Impresionante:** Una balsa de 1000 kg puede cargar 3000 kg adicionales, gracias a la baja densidad de la totora.

**(b) Profundidad de hundimiento con 3 pescadores:**

Masa total: $m_{total} = 1000 + 3 \times 70 = 1000 + 210 = 1210$ kg

Peso total: $W_{total} = 1210 \times 9.8 = 11858$ N

Volumen sumergido (por equilibrio $E = W_{total}$):
$$V_{sum} = \frac{W_{total}}{\rho_{agua} \times g} = \frac{11858}{1000 \times 9.8} = 1.21 \text{ m}^3$$

Profundidad de hundimiento:
$$h_{sum} = \frac{V_{sum}}{L \times W} = \frac{1.21}{4 \times 2} = \frac{1.21}{8} = 0.151 \text{ m} = 15.1 \text{ cm}$$

**(c) Fracción del volumen sumergida:**
$$\frac{V_{sum}}{V_{total}} = \frac{1.21}{4} = 0.3025 \approx 30.3\%$$

Verificación con densidad equivalente:
$$\frac{\rho_{equiv}}{\rho_{agua}} = \frac{m_{total}/V_{total}}{\rho_{agua}} = \frac{1210/4}{1000} = \frac{302.5}{1000} = 0.3025$$

**Coincide.** La fracción sumergida es igual a la razón de densidades.

**(d) Estabilidad inicial:**

**Centro de carena (B):** Centro de gravedad del volumen sumergido.
$$h_B = \frac{h_{sum}}{2} = \frac{0.151}{2} = 0.0755 \text{ m} \text{ (desde la quilla)}$$

**Centro de gravedad de la balsa (G_balsa):**
Como la totora es uniforme, está en el centro geométrico:
$$h_{G,balsa} = \frac{e}{2} = 0.25 \text{ m (desde la quilla)}$$

**Centro de gravedad de los pescadores (G_pesc):**
$$h_{G,pesc} = e + 0.3 = 0.5 + 0.3 = 0.8 \text{ m (desde la quilla)}$$

**Centro de gravedad combinado (G):**
$$h_G = \frac{m_{balsa} \times h_{G,balsa} + m_{pesc} \times h_{G,pesc}}{m_{total}}$$
$$h_G = \frac{1000 \times 0.25 + 210 \times 0.8}{1210} = \frac{250 + 168}{1210} = \frac{418}{1210} = 0.345 \text{ m}$$

**Altura metacéntrica inicial:**
$$GM = h_B + \frac{I_{waterline}}{V_{sum}} - h_G$$

Momento de inercia de la línea de flotación:
$$I_{waterline} = \frac{LW^3}{12} = \frac{4 \times 2^3}{12} = \frac{32}{12} = 2.667 \text{ m}^4$$

$$GM = 0.0755 + \frac{2.667}{1.21} - 0.345 = 0.0755 + 2.204 - 0.345 = 1.935 \text{ m}$$

> **Conclusión:** $GM > 0$ y muy grande. La balsa es extremadamente estable. El bajo centro de gravedad de la totora y la amplia base compensan la altura de los pescadores.

**3. Discusión Crítica:**
* Las balsas de totora son insumergibles por diseño: incluso llenas de agua, la totora flota por su porosidad. Los pescadores aymara las usan desde hace milenios en el Titicaca.
* La estabilidad disminuye si los pescadores se paran (suben el centro de gravedad) o si la carga se concentra en un lado (escora). La práctica tradicional distribuye el peso uniformemente.
* El agua del Titicaca es dulce ($\rho \approx 1000$ kg/m³), pero su salinidad residual (origen paleolacustre) la hace ligeramente más densa que agua pura, aumentando marginalmente el empuje.

**4. Análisis de Sensibilidad:**
| Parámetro | Cambio | Efecto en carga máxima |
|-----------|--------|------------------------|
| Espesor de totora $e$ | +20% | Carga máxima +20% (más volumen) |
| Densidad de totora | +10% (más compacta) | Carga máxima -13% |
| Número de pescadores | +1 (80 kg) | Hundimiento +2.1 cm |

**5. Extensión:**
Los Uros del Titicaca construyen islas flotantes enteras de totora, algunas de 30 m de diámetro, habitadas por familias completas. La durabilidad de la totora es limitada (se descompone en 6-12 meses en el agua), por lo que se añaden capas nuevas constantemente. En ingeniería naval moderna, los pontones de hormigón celular (densidad 300-500 kg/m³) imitan el principio de la totora, usando celdas de aire para reducir la densidad efectiva. Los submarinos controlan su flotabilidad mediante tanques de lastre, variando su densidad promedio para sumergirse o emerger.
```
---

## 📓 III. Actividades para el Portafolio Digital

Resuelve los siguientes 10 desafíos siguiendo el **Formato de 5-Bloques**. Para el Portafolio digital presenta **4 Desafíos** de tu elección.

---


### 🧠 Desafío 1
**El Depósito de GLP del Vecindario**

Un tanque de gas licuado de petróleo (GLP) doméstico es un cilindro vertical de $H = 1.2$ m y diámetro $D = 0.3$ m, lleno de propano líquido ($\rho = 500$ kg/m³) hasta el 80% de su altura. La parte superior contiene propano gaseoso a presión manométrica $P_{man} = 800$ kPa.

* **El Reto:** Calcula la presión absoluta en el fondo del tanque, la fuerza total sobre la tapa circular superior, y la fuerza sobre la pared cilíndrica.
* **Interpretación:** ¿Por qué los tanques de GLP tienen válvulas de seguridad que se activan a 1.8 MPa? Relaciona con el aumento de presión por expansión térmica.
---

### 🧠 Desafío 2
**El Sifón de la Pileta de Chorrillos**

Un sifón doméstico en Chorrillos (a nivel del mar) debe drenar agua desde una pileta hasta un desagüe situado 80 cm más abajo. El tubo del sifón tiene diámetro uniforme de 2 cm.

* **El Reto:** Calcula la presión mínima en el punto más alto del sifón (40 cm sobre la superficie del agua de la pileta) para que el flujo se mantenga. ¿Puede funcionar el sifón si el punto más alto supera los 10 m sobre el desagüe?
* **Análisis Crítico:** En la sierra peruana (Cerro de Pasco, 4330 msnm), ¿cómo cambia la capacidad del sifón? Calcula la altura máxima teórica del sifón en ambas ubicaciones.
---

### 🧠 Desafío 3
**El Elevador de Autos del Taller**

Un elevador hidráulico de cuatro postes tiene pistones de diámetro $D = 15$ cm cada uno. El sistema trabaja a presión manométrica máxima $P_{man} = 12$ MPa.

* **El Reto:** Calcula la fuerza total que puede ejercer el elevador, la masa máxima de vehículo que puede levantar, y el desplazamiento de cada pistón si la bomba inyecta 2 litros de aceite.
* **Toma de Decisión:** Un SUV pesa 2800 kg y una camioneta 4200 kg. ¿Es seguro levantar la camioneta con este elevador? ¿Qué presión manométrica requeriría? ¿Es factible con la bomba actual?

---

### 🧠 Desafío 4
**La Puerta Submarina del Acuario**

Un acuario marino tiene una ventana de observación rectangular de $2.5$ m $\times$ $1.8$ m, con el borde superior a $0.5$ m bajo la superficie del agua de mar ($\rho = 1025$ kg/m³).

* **El Reto:** Calcula la fuerza hidrostática sobre la ventana, la posición del centro de presión respecto al borde superior, y el torque que ejerce sobre las bisagras inferiores.
* **Análisis Técnico:** El vidrio acrílico tiene resistencia a la tracción de 70 MPa. ¿Es suficiente un espesor de 8 cm? Calcula el esfuerzo máximo usando distribución triangular de presión.

---

### 🧠 Desafío 5
**El Barómetro Casero del Colegio**

Un estudiante construye un barómetro de agua usando un tubo de ensayo de 15 cm invertido en una cubeta. El experimento se realiza en Cusco (3400 msnm).

* **El Reto:** Predice la altura de la columna de agua esperada. Si el tubo mide exactamente 15 cm, ¿qué observará el estudiante? Diseña una modificación usando dos líquidos (agua y aceite) para aumentar la sensibilidad de lectura.
* **Evaluación:** Compara la precisión de este barómetro casero con un barómetro aneroide digital ($\pm 0.1$ hPa). ¿En qué condiciones meteorológicas sería útil el barómetro casero?

---

### 🧠 Desafío 6
**El Submarino de Botellas del Proyecto Escolar**

Un equipo de estudiantes construye un "submarino" usando una botella de 2 litros ($\rho_{PET} = 1380$ kg/m³, paredes de 1 mm de espesor). El volumen interior es 2 litros y la masa de aire atrapado es despreciable.

* **El Reto:** Calcula la masa de la botella vacía, el volumen de agua que debe introducirse para que se sumerja completamente, y la fracción del volumen que debe llenarse para flotar a mitad de profundidad.
* **Extensión Creativa:** Diseña un sistema de lastre usando una jeringa y tubería flexible que permita controlar la profundidad. ¿Qué volumen de agua debe desplazar la jeringa para pasar de flotación a inmersión completa?

---

### 🧠 Desafío 7
**El Tanque Elevado de Agua de Lurín**

Un tanque elevado de concreto alimenta por gravedad a una urbanización. El tanque está a $H = 25$ m sobre las viviendas y contiene agua hasta $h = 4$ m de profundidad. La base del tanque es cuadrada de $L = 6$ m de lado.

* **El Reto:** Calcula la presión manométrica en las tuberías de las casas, la fuerza sobre la base del tanque, y la altura equivalente de una torre de mercurio que produciría la misma presión en la base.
* **Análisis de Sensibilidad:** Si el consumo nocturno reduce el nivel del tanque en 1.5 m, ¿en cuánto disminuye la presión en las viviendas? ¿Es perceptible en el caudal de las duchas?
---

### 🧠 Desafío 8
**El Manómetro Diferencial de la Central Hidroeléctrica**

En la central hidroeléctrica de Mantaro, un manómetro diferencial de tubo en U mide la caída de presión a través de una turbina. El manómetro usa mercurio y está conectado entre la entrada ($P_1$) y salida ($P_2$) de la turbina.

* **El Reto:** La diferencia de niveles de mercurio es $\Delta h = 45$ cm, con el lado de entrada más bajo. Calcula la caída de presión en Pa y en metros de columna de agua. Si el caudal es $Q = 50$ m³/s, ¿qué altura neta de caída representa esta diferencia de presión?
* **Interpretación Profesional:** ¿Por qué se usa mercurio en lugar de agua para medir grandes diferencias de presión? Calcula la altura equivalente si se usara agua y discute la viabilidad práctica.

---

### 🧠 Desafío 9
**La Canoa de los Riberenos del Amazonas**

Una canoa de quinilla (madera liviana) tiene forma aproximadamente semicilíndrica de radio $R = 0.6$ m, longitud $L = 5$ m, y espesor de pared $e = 3$ cm ($\rho_{madera} = 450$ kg/m³).

* **El Reto:** Calcula la línea de flotación sin carga, el calado máximo antes de inundarse, y el número de pasajeros de 75 kg que puede transportar con un margen de seguridad del 20% (sin sumergirse más del 80% del radio).
* **Toma de Decisión:** Los pescadores locales quieren aumentar la capacidad. ¿Es más efectivo alargar la canoa 1 m o aumentar el radio a 0.8 m? Compara el aumento de capacidad de carga en ambos casos.

---

### 🧠 Desafío 10
**El Hidrómetro del Laboratorio de Cerveza Artesanal**

Un hidrómetro casero para medir densidad de mosto de cerveza consiste en un tubo cilíndrico de corcho ($\rho = 240$ kg/m³) de diámetro $d = 1$ cm y longitud $L = 20$ cm, con una escala graduada.

* **El Reto:** Calcula la profundidad de hundimiento en agua pura y en mosto de densidad $1.05$ g/cm³. Diseña la escala de graduación para densidades entre 0.98 y 1.10 g/cm³, indicando la separación entre marcas consecutivas de 0.01 g/cm³.
* **Análisis de Sensibilidad:** Si el diámetro del tubo varía ±0.5 mm por imperfección de fabricación, ¿cuál es el error máximo en la lectura de densidad? ¿Es aceptable para control de calidad cervecero?
