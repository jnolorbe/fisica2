# Sesión 6: Hidrodinámica I

## 📌 I. Fundamento Teórico

En esta sesión se estudia el movimiento de fluidos ideales (incompresibles y no viscosos), las leyes de conservación que gobiernan su comportamiento, y las aplicaciones tecnológicas fundamentales derivadas de la ecuación de Bernoulli.

---

### 1.1. Flujo Ideal

**Fluido ideal:** Fluido que cumple tres condiciones simplificadoras:
* **Incompresible:** La densidad $\rho$ es constante en todo el fluido.
* **No viscoso:** No hay fricción interna; no se disipa energía mecánica por calor.
* **Estacionario (laminar):** La velocidad en cada punto del espacio no cambia con el tiempo.

**Línea de corriente:** Trayectoria seguida por una partícula fluida. En flujo estacionario, las líneas de corriente no se cruzan.

**Tubo de flujo:** Conjunto de líneas de corriente que forman una especie de "tubo" imaginario.

> **💡 Regla de Oro:** El modelo de fluido ideal es una aproximación válida para líquidos a velocidades moderadas y para gases a bajas velocidades (Mach < 0.3). En flujos rápidos o con obstáculos, aparecen efectos de viscosidad y turbulencia que requieren modelos más complejos.

---

### 1.2. Ecuación de Continuidad

Principio de conservación de la masa para un fluido incompresible en flujo estacionario.

Para un tubo de flujo con secciones $A_1$ y $A_2$:

$$A_1 v_1 = A_2 v_2 = Q = \text{constante}$$

donde:
* $A$: área de la sección transversal
* $v$: velocidad del fluido
* $Q$: caudal volumétrico (m³/s)

**Interpretación:** El fluido se acelera al pasar por secciones estrechas y se desacelera en secciones anchas.

**Caudal másico (masa por unidad de tiempo):**

$$\dot{m} = \rho A v = \rho Q$$

> **💡 Regla de Oro:** La ecuación de continuidad implica que en una tubería, la velocidad es inversamente proporcional al área de la sección. Una manguera estrecha expulsa agua con mayor velocidad que una ancha.

---

### 1.3. Ecuación de Bernoulli

Teorema de conservación de energía mecánica para un fluido ideal en flujo estacionario.

Para dos puntos de una misma línea de corriente:

$$P_1 + \frac{1}{2}\rho v_1^2 + \rho g h_1 = P_2 + \frac{1}{2}\rho v_2^2 + \rho g h_2 = \text{constante}$$

**Términos:**
* $P$: presión de estancamiento (presión estática)
* $\frac{1}{2}\rho v^2$: presión dinámica (asociada a la velocidad)
* $\rho g h$: presión hidrostática (asociada a la altura)

**Interpretación física:** A lo largo de una línea de corriente, la suma de presión estática, presión dinámica y presión hidrostática se conserva. Si una aumenta, otra debe disminuir.

**Caso particular: fluido en reposo ($v_1 = v_2 = 0$)**

$$P_1 + \rho g h_1 = P_2 + \rho g h_2$$

Recupera la ecuación de la hidrostática.

> **💡 Regla de Oro:** Donde la velocidad es mayor, la presión es menor (efecto Venturi). Donde la altura es mayor, la presión es menor (efecto sifón). La presión total (suma de los tres términos) permanece constante a lo largo de una línea de corriente.

---

### 1.4. Tubo de Venturi

Dispositivo para medir caudal basado en la caída de presión en una constricción.

**Configuración:** Tubo con sección estrecha central, conectado a un manómetro diferencial.

Aplicando Bernoulli entre la sección ancha (1) y la estrecha (2), a la misma altura:

$$P_1 + \frac{1}{2}\rho v_1^2 = P_2 + \frac{1}{2}\rho v_2^2$$

Usando continuidad ($A_1 v_1 = A_2 v_2$):

$$v_2 = v_1 \frac{A_1}{A_2}$$

La diferencia de presión medida permite calcular el caudal:

$$Q = A_1 \sqrt{\frac{2(P_1 - P_2)}{\rho\left[\left(\frac{A_1}{A_2}\right)^2 - 1\right]}}$$

**Aplicaciones:** Medición de caudal en tuberías industriales, carburadores de motores, aspiradores de polvo, inyectores de riego.

---

### 1.5. Tubo de Pitot

Dispositivo para medir la velocidad de un fluido mediante la presión de estancamiento.

**Principio:** Un tubo orientado contra el flujo trae el fluido al reposo ($v = 0$), convirtiendo toda la presión dinámica en presión estática.

**Presión de estancamiento (total):**

$$P_{total} = P_{estatica} + \frac{1}{2}\rho v^2$$

**Velocidad del fluido:**

$$v = \sqrt{\frac{2(P_{total} - P_{estatica})}{\rho}}$$

**Configuración típica:** Tubo de Pitot conectado a un manómetro diferencial que mide $P_{total} - P_{estatica}$.

**Aplicaciones:** Velocímetros de aviones (medición de velocidad respecto al aire), anemómetros, medición de velocidad en canales de agua.

---

### 1.6. Vaciado de un Tanque (Ecuación de Torricelli)

Tiempo de vaciado de un recipiente con orificio en su base.

**Velocidad de effluencia:** Aplicando Bernoulli entre la superficie libre (1) y el orificio (2), ambos a presión atmosférica:

$$v = \sqrt{2gh}$$

donde $h$ es la altura de la superficie libre sobre el orificio.

**Tiempo de vaciado:** Integrando la ecuación diferencial que resulta de relacionar la velocidad de descenso del nivel con el caudal de salida:

$$t = \frac{A_{tanque}}{A_{orificio}} \sqrt{\frac{2H}{g}}$$

para un tanque cilíndrico de área $A_{tanque}$ y altura inicial $H$, con orificio de área $A_{orificio}$.

**Caso general (geometrías arbitrarias):**

$$t = \int_0^H \frac{A(h)}{A_{orificio}\sqrt{2gh}} dh$$

> **💡 Regla de Oro:** La velocidad de effluencia es la misma que tendría un objeto cayendo libremente desde la altura $h$ (teorema de Torricelli). El tiempo de vaciado depende fuertemente de la relación de áreas; un orificio pequeño vacía lentamente.

---

## 🚀 II. Problemas Resueltos

---

### 🧩 Problema N° 1

```{admonition} La Tubería del Sistema de Riego de Chavimochic
:class: important
**Situación:** El sistema de riego Chavimochic (La Libertad) transporta agua a través de una tubería principal de diámetro $D_1 = 1.2$ m que se bifurca en dos tuberías secundarias de $D_2 = 0.8$ m cada una. El caudal total es $Q = 2.5$ m³/s. Calcular: (a) la velocidad en la tubería principal, (b) la velocidad en cada tubería secundaria si el flujo se divide equitativamente, (c) la velocidad si una de las secundarias se cierra, y (d) la presión manométrica en la principal si la presión en las secundarias es $P_2 = 150$ kPa y la tubería es horizontal.

```

```{admonition} Solución
:class: dropdown hint
**1. Planteamiento:**
* **Ruta de la solución:** Aplicar la ecuación de continuidad para relacionar velocidades y caudales. Usar Bernoulli para relacionar presiones cuando se conoce la velocidad.
* **Predicción cualitativa:** La velocidad en la tubería principal será moderada (~2 m/s). Al cerrar una secundaria, la velocidad en la abierta se duplicará, reduciendo la presión según Bernoulli.

**2. Resolución:**

**Áreas:**
$$A_1 = \frac{\pi D_1^2}{4} = \frac{\pi \times (1.2)^2}{4} = 1.131 \text{ m}^2$$
$$A_2 = \frac{\pi D_2^2}{4} = \frac{\pi \times (0.8)^2}{4} = 0.503 \text{ m}^2$$

**(a) Velocidad en la principal:**
$$v_1 = \frac{Q}{A_1} = \frac{2.5}{1.131} = 2.21 \text{ m/s}$$

**(b) Velocidad en secundarias (flujo equitativo):**
$$Q_2 = \frac{Q}{2} = 1.25 \text{ m}^3\text{/s}$$
$$v_2 = \frac{Q_2}{A_2} = \frac{1.25}{0.503} = 2.49 \text{ m/s}$$

**(c) Velocidad con una secundaria cerrada:**
Todo el caudal por una sola tubería:
$$v_2' = \frac{Q}{A_2} = \frac{2.5}{0.503} = 4.97 \text{ m/s}$$

**(d) Presión en la principal (Bernoulli, horizontal):**
$$P_1 + \frac{1}{2}\rho v_1^2 = P_2 + \frac{1}{2}\rho v_2^2$$

$$P_1 = P_2 + \frac{1}{2}\rho(v_2^2 - v_1^2)$$

Con $\rho = 1000$ kg/m³ y $v_2 = 2.49$ m/s:
$$P_1 = 150000 + \frac{1}{2} \times 1000 \times (2.49^2 - 2.21^2)$$
$$P_1 = 150000 + 500 \times (6.20 - 4.88) = 150000 + 500 \times 1.32$$
$$P_1 = 150000 + 660 = 150660 \text{ Pa} \approx 150.7 \text{ kPa}$$

**3. Discusión Crítica:**
* La diferencia de presión es pequeña (0.7 kPa) porque las velocidades son similares. En diseño de tuberías, estas pérdidas de presión por aceleración se suman a las pérdidas por fricción (que Bernoulli no considera).
* El cierre de una tubería secundaria no solo duplica la velocidad, sino que aumenta la pérdida de carga por fricción (proporcional a $v^2$), reduciendo la presión disponible para riego.
* Los sistemas reales de Chavimochic usan bombas intercaladas para compensar pérdidas de presión a lo largo de los 200 km de canal.

**4. Análisis de Sensibilidad:**
| Parámetro | Cambio | Efecto en $v_1$ | Efecto en $P_1$ |
|-----------|--------|-----------------|-----------------|
| Caudal $Q$ | +20% | +20% | -0.8% |
| Diámetro principal | +10% | -17% | +0.5% |
| Densidad (agua salada) | +3% | 0% | +3% (directo) |

**5. Extensión:**
Los sistemas de riego por goteo requieren presiones controladas (20-50 kPa). Los sistemas de riego por aspersión necesitan 200-400 kPa. La ecuación de Bernoulli ideal es insuficiente para diseñar tuberías largas; se usa la ecuación de Darcy-Weisbach que incluye factor de fricción $f$ y rugosidad de la tubería. Los CFD (Computational Fluid Dynamics) modelan flujos complejos con turbulencia, viscosidad y geometrías irregulares.
```
---

### 🧩 Problema N° 2
 
```{admonition} El Carburador del Mototaxi
:class: important
**Situación:** Un carburador de mototaxi usa un tubo Venturi donde el aire entra por una sección $A_1 = 4$ cm² y pasa por una garganta de $A_2 = 1$ cm². La presión atmosférica es $P_{atm} = 100$ kPa y la densidad del aire $\rho = 1.2$ kg/m³. Calcular: (a) la velocidad del aire en la garganta si la velocidad de entrada es $v_1 = 15$ m/s, (b) la presión en la garganta, (c) la diferencia de presión disponible para succionar gasolina del carburador, y (d) la altura máxima a la que puede estar el nivel de gasolina para que sea succionada.
```

```{admonition} Solución
:class: dropdown hint
**1. Planteamiento:**
* **Ruta de la solución:** Aplicar continuidad para encontrar la velocidad en la garganta. Usar Bernoulli horizontal para calcular la caída de presión. La presión reducida en la garganta crea succión que eleva la gasolina.
* **Predicción cualitativa:** La velocidad se cuadruplicará en la garganta (relación de áreas 4:1). La presión caerá significativamente, creando suficiente succión para elevar gasolina varios centímetros.

**2. Resolución:**

**(a) Velocidad en la garganta:**
$$A_1 v_1 = A_2 v_2$$
$$v_2 = v_1 \frac{A_1}{A_2} = 15 \times \frac{4}{1} = 60 \text{ m/s}$$

**(b) Presión en la garganta (Bernoulli horizontal):**
$$P_1 + \frac{1}{2}\rho v_1^2 = P_2 + \frac{1}{2}\rho v_2^2$$

$$P_2 = P_1 + \frac{1}{2}\rho(v_1^2 - v_2^2)$$
$$P_2 = 100000 + \frac{1}{2} \times 1.2 \times (225 - 3600)$$
$$P_2 = 100000 + 0.6 \times (-3375) = 100000 - 2025 = 97975 \text{ Pa}$$

$$P_2 \approx 98.0 \text{ kPa}$$

**(c) Diferencia de presión para succión:**
$$\Delta P = P_1 - P_2 = 100000 - 97975 = 2025 \text{ Pa} \approx 2.0 \text{ kPa}$$

Equivalente en columna de agua:
$$h_{agua} = \frac{\Delta P}{\rho_{agua} g} = \frac{2025}{1000 \times 9.8} = 0.207 \text{ m} = 20.7 \text{ cm}$$

**(d) Altura máxima de gasolina ($\rho_{gas} \approx 750$ kg/m³):**
$$h_{gas} = \frac{\Delta P}{\rho_{gas} g} = \frac{2025}{750 \times 9.8} = \frac{2025}{7350} = 0.276 \text{ m} = 27.6 \text{ cm}$$

> **Nota:** En la práctica, la altura real es menor debido a pérdidas por fricción y a que el flujo no es ideal. Los carburadores típicos usan alturas de 5-15 cm.

**3. Discusión Crítica:**
* La velocidad de 60 m/s en la garganta corresponde a Mach ~0.18, dentro del rango válido para fluido incompresible. A velocidades mayores (Mach > 0.3), la compresibilidad del aire modifica los resultados.
* Los carburadores modernos han sido reemplazados por inyección electrónica, que usa bombas de alta presión (300 kPa) para atomizar el combustible con mayor precisión.
* El efecto Venturi también explica por qué las cortinas de ducha se succionan hacia dentro cuando se abre el grifo: el flujo de agua reduce la presión del aire entre la cortina y el agua.

**4. Análisis de Sensibilidad:**
| Parámetro | Cambio | Efecto en $\Delta P$ |
|-----------|--------|---------------------|
| Velocidad de entrada | +20% | $\Delta P$ +44% ($\propto v^2$) |
| Relación de áreas | +50% | $\Delta P$ +78% |
| Densidad del aire | +10% (frío) | $\Delta P$ +10% |

**5. Extensión:**
Los inyectores de combustible modernos usan presiones de 100-200 bar (MPa) para atomizar el combustible en gotas de 10-20 micras, mejorando la combustión y reduciendo emisiones. Los nebulizadores médicos usan el efecto Venturi con aire comprimido a 200 kPa para generar aerosoles de medicamentos de 1-5 micras que llegan a los alvéolos pulmonares.
```
---

### 🧩 Problema N° 3

```{admonition} El Anemómetro del Observatorio de Huancayo
:class: important
**Situación:** El observatorio geofísico de Huancayo (3300 msnm) usa un tubo de Pitot para medir la velocidad del viento. Un día de verano, el manómetro diferencial conectado al Pitot indica $\Delta h = 12$ mm de columna de agua. La densidad del aire a esa altitud es $\rho_{aire} = 0.85$ kg/m³. Calcular: (a) la velocidad del viento, (b) la presión dinámica, (c) la presión total en el punto de estancamiento, y (d) la velocidad que indicaría el mismo Pitot en Lima (a nivel del mar, $\rho_{aire} = 1.2$ kg/m³) con la misma lectura de manómetro.

```

```{admonition} Solución
:class: dropdown hint
**1. Planteamiento:**
* **Ruta de la solución:** Convertir la lectura del manómetro (diferencia de altura de agua) a diferencia de presión. Aplicar la fórmula de Pitot para obtener velocidad. Comparar con condiciones al nivel del mar.
* **Predicción cualitativa:** A menor densidad del aire (Huancayo), la misma velocidad produce menor presión dinámica. Por tanto, para la misma lectura de manómetro, el viento en Huancayo debe ser más rápido que en Lima.

**2. Resolución:**

**(a) Velocidad del viento:**

Diferencia de presión del manómetro:
$$\Delta P = \rho_{agua} g \Delta h = 1000 \times 9.8 \times 0.012 = 117.6 \text{ Pa}$$

De la ecuación de Pitot:
$$\Delta P = \frac{1}{2}\rho_{aire} v^2$$
$$v = \sqrt{\frac{2\Delta P}{\rho_{aire}}} = \sqrt{\frac{2 \times 117.6}{0.85}} = \sqrt{\frac{235.2}{0.85}} = \sqrt{276.7}$$

$$v \approx 16.6 \text{ m/s} \approx 59.8 \text{ km/h}$$

**(b) Presión dinámica:**
$$P_{din} = \frac{1}{2}\rho v^2 = \frac{1}{2} \times 0.85 \times (16.6)^2 = 0.425 \times 275.6 = 117.1 \text{ Pa}$$

Verificación: coincide con $\Delta P$ (error por redondeo).

**(c) Presión total:**
$$P_{total} = P_{estatica} + P_{din}$$

La presión estática a 3300 msnm es ~67 kPa:
$$P_{total} = 67000 + 117.1 = 67117.1 \text{ Pa} \approx 67.1 \text{ kPa}$$

**(d) Velocidad equivalente en Lima:**

Misma $\Delta P = 117.6$ Pa, pero $\rho_{aire} = 1.2$ kg/m³:
$$v_{Lima} = \sqrt{\frac{2 \times 117.6}{1.2}} = \sqrt{\frac{235.2}{1.2}} = \sqrt{196} = 14.0 \text{ m/s}$$

$$v_{Lima} = 14.0 \text{ m/s} \approx 50.4 \text{ km/h}$$

> **Conclusión:** La misma lectura de manómetro corresponde a viento 18% más lento en Lima que en Huancayo debido a la mayor densidad del aire al nivel del mar.

**3. Discusión Crítica:**
* Los anemómetros de Pitot requieren corrección por densidad del aire, que depende de altitud, temperatura y humedad. Los anemómetros modernos incluyen sensores de temperatura y presión para compensar automáticamente.
* A velocidades cercanas a la velocidad del sonido (Mach > 0.3), aparecen efectos de compresibilidad que hacen que la presión de estancamiento sea mayor que la predicha por Bernoulli. Se usa entonces la fórmula de Rayleigh para Pitot.
* El observatorio de Huancayo, fundado en 1920 por Carnegie Institution, ha contribuido a la comprensión del fenómeno El Niño mediante monitoreo meteorológico continuo.

**4. Análisis de Sensibilidad:**
| Parámetro | Cambio | Efecto en velocidad medida |
|-----------|--------|----------------------------|
| Densidad del aire | +10% | Velocidad -4.9% |
| Lectura de manómetro | +10% | Velocidad +4.9% |
| Temperatura (altitud) | +10°C | Densidad -3.5%, velocidad +1.8% |

**5. Extensión:**
Los aviones comerciales usan tubos de Pitot en el exterior del fuselaje para medir velocidad respecto al aire (IAS, Indicated Airspeed). El hielo en los tubos de Pitot ha causado accidentes aéreos (Air France 447, 2009), llevando a sistemas de calentamiento eléctrico y redundancia triple. Los drones modernos usan Pitot virtuales basados en GPS y modelos de viento, eliminando el tubo físico.
```
---

### 🧩 Problema N° 4
```{admonition} El Tanque Elevado de Agua de Lurín
:class: important
**Situación:** Un tanque elevado de concreto cilíndrico de diámetro $D = 3$ m y altura de agua $H = 4$ m alimenta por gravedad a una urbanización. En su base tiene un orificio circular de diámetro $d = 5$ cm. Calcular: (a) la velocidad inicial de effluencia, (b) el caudal inicial, (c) el tiempo de vaciado completo, (d) la velocidad y caudal cuando el nivel ha descendido a la mitad, y (e) la altura del chorro de agua medida desde el orificio.

```

```{admonition} Solución
:class: dropdown hint
**1. Planteamiento:**
* **Ruta de la solución:** Aplicar la ecuación de Torricelli para la velocidad de effluencia. El caudal es el producto de velocidad por área del orificio. El tiempo de vaciado requiere integrar la ecuación diferencial del nivel descendiente. La altura del chorro se calcula con cinemática de proyectiles.
* **Predicción cualitativa:** La velocidad inicial será ~9 m/s (equivalente a caída libre de 4 m). El vaciado será lento debido a la pequeña relación de áreas (~1:3600). El chorro alcanzará casi la altura original (sin fricción).

**2. Resolución:**

**Datos:**
* $D = 3$ m $\Rightarrow$ $A_{tanque} = \frac{\pi D^2}{4} = 7.069$ m²
* $d = 0.05$ m $\Rightarrow$ $A_{orificio} = \frac{\pi d^2}{4} = 1.963 \times 10^{-3}$ m²
* $H = 4$ m

**(a) Velocidad inicial de effluencia:**
$$v_0 = \sqrt{2gH} = \sqrt{2 \times 9.8 \times 4} = \sqrt{78.4} = 8.85 \text{ m/s}$$

**(b) Caudal inicial:**
$$Q_0 = A_{orificio} \times v_0 = 1.963 \times 10^{-3} \times 8.85 = 0.0174 \text{ m}^3\text{/s} = 17.4 \text{ L/s}$$

**(c) Tiempo de vaciado completo:**

Para tanque cilíndrico:
$$t = \frac{A_{tanque}}{A_{orificio}} \sqrt{\frac{2H}{g}}$$

$$t = \frac{7.069}{1.963 \times 10^{-3}} \times \sqrt{\frac{2 \times 4}{9.8}}$$
$$t = 3601 \times \sqrt{0.816} = 3601 \times 0.903 = 3252 \text{ s}$$

$$t \approx 54.2 \text{ minutos}$$

**(d) Velocidad y caudal a mitad de altura ($h = 2$ m):**

$$v = \sqrt{2gh} = \sqrt{2 \times 9.8 \times 2} = \sqrt{39.2} = 6.26 \text{ m/s}$$

$$Q = A_{orificio} \times v = 1.963 \times 10^{-3} \times 6.26 = 0.0123 \text{ m}^3\text{/s} = 12.3 \text{ L/s}$$

> **Observación:** A mitad de altura, la velocidad es $1/\sqrt{2} \approx 0.707$ de la inicial, y el caudal también. El vaciado se ralentiza progresivamente.

**(e) Altura del chorro:**

El agua sale horizontalmente (suponiendo orificio lateral en la base) con velocidad $v_0 = 8.85$ m/s. Usando la ecuación de proyectiles para alcance vertical con caída libre:

El tiempo de caída desde el orificio al suelo (si el tanque está a altura $y_0$ sobre el suelo) depende de la altura del tanque. Si el orificio está a nivel del suelo ($y_0 = 0$), el chorro no asciende.

Suponiendo que la pregunta se refiere a la altura máxima que alcanzaría el chorro si se dirigiera verticalmente hacia arriba:

$$v^2 = v_0^2 - 2gy_{max} = 0$$
$$y_{max} = \frac{v_0^2}{2g} = \frac{78.4}{19.6} = 4 \text{ m}$$

> **Resultado notable:** El chorro alcanzaría exactamente la altura original del agua en el tanque (conservación de energía). En la práctica, pérdidas por fricción y contracción del vena contracta reducen esta altura a ~60-70% del valor teórico.

**3. Discusión Crítica:**
* El tiempo de vaciado de 54 minutos es largo debido a la pequeña relación de áreas. Los tanques reales de distribución de agua usan orificios de drenaje más grandes o bombas para vaciado rápido en mantenimiento.
* La contracción del chorro (vena contracta) reduce el área efectiva del orificio a ~0.6-0.7 del área geométrica. Se introduce un coeficiente de descarga $C_d \approx 0.62$ para correcciones prácticas.
* Los tanques de torre modernos usan válvulas de flotador que mantienen el nivel constante, eliminando la variación de presión con el tiempo.

**4. Análisis de Sensibilidad:**
| Parámetro | Cambio | Efecto en tiempo de vaciado |
|-----------|--------|----------------------------|
| Diámetro de orificio | +20% | Tiempo -36% ($\propto 1/d^2$) |
| Altura inicial $H$ | +50% | Tiempo +22% ($\propto \sqrt{H}$) |
| Diámetro del tanque | +50% | Tiempo +125% ($\propto D^2$) |

**5. Extensión:**
Los relojes de agua (clepsidras) de la antigüedad usaban el principio de Torricelli para medir tiempo, controlando el nivel constante con un flotador. Los sistemas de riego por gravedad (andenería inca) usaban canales con pendiente controlada para mantener velocidad constante. Los modernos sistemas de distribución de agua potable usan redes de tuberías modeladas con software EPANET que resuelve ecuaciones de Bernoulli extendidas con pérdidas por fricción (ecuación de Hazen-Williams o Darcy-Weisbach).
```
---

### 🧩 Problema N° 5

```{admonition} La Válvula de Seguridad del Depósito de GLP
:class: important
**Situación:** Un depósito de GLP doméstico tiene una válvula de seguridad conectada a un tubo de Venturi de sección $A_1 = 0.5$ cm² que se estrecha a $A_2 = 0.1$ cm². Si el gas (propano, $\rho = 2.0$ kg/m³ a 20°C) escapa por una fuga interna a $v_1 = 25$ m/s, calcular: (a) la velocidad en la garganta del Venturi, (b) la presión en la garganta si la presión de entrada es $P_1 = 200$ kPa manométrica, (c) si la presión cae por debajo de 50 kPa se activa el cierre de emergencia, ¿se activará la válvula?, y (d) la velocidad del sonido en el propano a 20°C si $\gamma = 1.13$ y $R_{especifica} = 189$ J/(kg·K), verificando si el flujo es subsónico.

```

```{admonition} Solución
:class: dropdown hint
**1. Planteamiento:**
* **Ruta de la solución:** Aplicar continuidad para la velocidad en la garganta. Usar Bernoulli para la presión. Calcular la velocidad del sonido en el gas para verificar la hipótesis de flujo incompresible.
* **Predicción cualitativa:** La velocidad en la garganta será muy alta (~125 m/s). La presión caerá significativamente, posiblemente activando el cierre de emergencia. La velocidad del sonido en propano será ~250 m/s, manteniendo flujo subsónico.

**2. Resolución:**

**(a) Velocidad en la garganta:**
$$v_2 = v_1 \frac{A_1}{A_2} = 25 \times \frac{0.5}{0.1} = 25 \times 5 = 125 \text{ m/s}$$

**(b) Presión en la garganta (Bernoulli horizontal):**
$$P_2 = P_1 + \frac{1}{2}\rho(v_1^2 - v_2^2)$$
$$P_2 = 200000 + \frac{1}{2} \times 2.0 \times (625 - 15625)$$
$$P_2 = 200000 + 1.0 \times (-15000) = 200000 - 15000 = 185000 \text{ Pa}$$

$$P_2 = 185 \text{ kPa (manométrica)}$$

**(c) ¿Se activa el cierre de emergencia?**

Umbral de activación: $P_{min} = 50$ kPa manométrica.

La presión en la garganta es 185 kPa > 50 kPa.

> **Conclusión:** No se activa el cierre de emergencia. La caída de presión es de solo 15 kPa, insuficiente para alcanzar el umbral de 50 kPa.

**Verificación de escenario crítico:**
¿Qué velocidad de entrada causaría $P_2 = 50$ kPa?

$$50000 = 200000 + \frac{1}{2} \times 2.0 \times (v_1^2 - 25v_1^2)$$
$$-150000 = v_1^2(1 - 25) = -24v_1^2$$
$$v_1^2 = \frac{150000}{24} = 6250$$
$$v_1 = 79.1 \text{ m/s}$$

A $v_1 = 79.1$ m/s, la válvula se activaría.

**(d) Velocidad del sonido en propano:**
$$a = \sqrt{\gamma R T} = \sqrt{1.13 \times 189 \times 293}$$
$$a = \sqrt{62600} \approx 250.2 \text{ m/s}$$

**Número de Mach en la garganta:**
$$M = \frac{v_2}{a} = \frac{125}{250.2} = 0.50$$

> **Conclusión:** $M = 0.50 < 0.3$ límite estricto para incompresible, pero < 1 (subsónico). La aproximación de Bernoulli para fluido incompresible es marginalmente válida; para mayor precisión se usaría la ecuación de flujo compresible isentrópico.

**3. Discusión Crítica:**
* Los sistemas de GLP reales usan válvulas de exceso de flujo (excess flow valves) que se cierran automáticamente si el caudal supera un umbral, independientemente de la presión. Esto protege contra roturas de tubería.
* El propano líquido en el tanque está a presión de vapor saturado (~0.8 MPa a 20°C). La fuga de gas es desde la fase vapor en la parte superior del tanque.
* Los códigos de seguridad (NFPA 58 en EE.UU., OSINERGMIN en Perú) exigen válvulas de seguridad múltiples y pruebas de estanqueidad periódicas.

**4. Análisis de Sensibilidad:**
| Parámetro | Cambio | Efecto en caída de presión |
|-----------|--------|----------------------------|
| Velocidad de entrada | +20% | $\Delta P$ +44% |
| Relación de áreas | +20% | $\Delta P$ +44% |
| Densidad del gas (temperatura) | +10% | $\Delta P$ +10% |

**5. Extensión:**
Los sistemas de distribución de gas natural usan reguladores de presión de dos etapas: primero reducen de 1.5 MPa (red principal) a 50 kPa (domiciliaria), luego a 2.5 kPa (aparatos). Los medidores de gas domésticos usan diafragmas que miden volumen a presión constante, compensando temperatura. Las fugas de gas se detectan con sensores de semiconductor de óxido de estaño (SnO₂) que cambian resistencia en presencia de hidrocarburos.
```
---

### 🧩 Problema N° 6

```{admonition} : El Sifón de la Pileta de Chorrillos
:class: important
**Situación:** Un sifón doméstico en Chorrillos (a nivel del mar) drena agua desde una pileta hasta un desagüe situado 80 cm más abajo. El tubo del sifón tiene diámetro uniforme de 2 cm y longitud total de 1.5 m. La altura máxima del punto más alto del sifón respecto a la superficie del agua en la pileta es 40 cm. Calcular: (a) la velocidad de salida del agua aplicando Bernoulli, (b) el caudal, (c) la presión en el punto más alto del sifón, y (d) la altura máxima teórica que podría tener el punto más alto antes de que el agua se vaporice (presión de vapor del agua a 20°C es 2.3 kPa).

```

```{admonition} Solución
:class: dropdown hint
**1. Planteamiento:**
* **Ruta de la solución:** Aplicar Bernoulli entre la superficie libre de la pileta (punto 1, $v \approx 0$, $P = P_{atm}$) y la salida del sifón (punto 3, $P = P_{atm}$, velocidad $v$). Luego aplicar Bernoulli entre la superficie y el punto más alto (punto 2) para encontrar la presión allí.
* **Predicción cualitativa:** La velocidad dependerá solo de la diferencia de altura entre pileta y desagüe (80 cm). La presión en el punto más alto será menor que atmosférica (vacío parcial), posiblemente cercana a la presión de vapor.

**2. Resolución:**

**Datos:**
* $h_1 = 0$ (referencia: superficie de la pileta)
* $h_3 = -0.80$ m (desagüe 80 cm abajo)
* $h_2 = +0.40$ m (punto más alto, 40 cm arriba)
* $D = 0.02$ m $\Rightarrow$ $A = \frac{\pi D^2}{4} = 3.1416 \times 10^{-4}$ m²

**(a) Velocidad de salida:**

Bernoulli entre superficie (1) y salida (3):
$$P_{atm} + 0 + \rho g h_1 = P_{atm} + \frac{1}{2}\rho v_3^2 + \rho g h_3$$

$$0 = \frac{1}{2}v_3^2 + g(-0.80)$$
$$v_3 = \sqrt{2g \times 0.80} = \sqrt{2 \times 9.8 \times 0.80} = \sqrt{15.68} = 3.96 \text{ m/s}$$

> **Nota:** La velocidad es la misma que tendría un objeto cayendo 80 cm.

**(b) Caudal:**
$$Q = A \times v_3 = 3.1416 \times 10^{-4} \times 3.96 = 1.24 \times 10^{-3} \text{ m}^3\text{/s} = 1.24 \text{ L/s}$$

**(c) Presión en el punto más alto (2):**

Bernoulli entre superficie (1) y punto más alto (2):
$$P_{atm} + 0 + 0 = P_2 + \frac{1}{2}\rho v_2^2 + \rho g h_2$$

Por continuidad, $v_2 = v_3 = 3.96$ m/s (mismo diámetro).

$$P_{atm} = P_2 + \frac{1}{2} \times 1000 \times (3.96)^2 + 1000 \times 9.8 \times 0.40$$
$$101325 = P_2 + 500 \times 15.68 + 3920$$
$$101325 = P_2 + 7840 + 3920 = P_2 + 11760$$

$$P_2 = 101325 - 11760 = 89565 \text{ Pa} \approx 89.6 \text{ kPa}$$

Presión manométrica:
$$P_{2,man} = 89565 - 101325 = -11760 \text{ Pa} \approx -11.8 \text{ kPa}$$

> **Interpretación:** Hay un vacío parcial de 11.8 kPa en el punto más alto. Esto es lo que mantiene el agua subiendo por el sifón.

**(d) Altura máxima antes de la cavitación:**

El límite ocurre cuando $P_2 = P_{vapor} = 2300$ Pa (absoluta).

$$P_{atm} = P_{vapor} + \frac{1}{2}\rho v^2 + \rho g h_{max}$$

$$101325 = 2300 + 7840 + 9800 \times h_{max}$$
$$101325 - 2300 - 7840 = 9800 \times h_{max}$$
$$91185 = 9800 \times h_{max}$$

$$h_{max} = \frac{91185}{9800} = 9.30 \text{ m}$$

> **Nota teórica:** A nivel del mar, un sifón podría elevar agua hasta ~10 m antes de que se formen burbujas de vapor (cavitación). En la práctica, por pérdidas de carga y liberación de gases disueltos, el límite es ~7-8 m.

**3. Discusión Crítica:**
* El sifón funciona porque la presión atmosférica en la pileta empuja el agua hacia arriba por el tubo, compensando el vacío parcial en la cima. La energía potencial del agua que desciende por el lado largo "tira" del agua que asciende por el lado corto.
* En la sierra peruana (Cerro de Pasco, 4330 msnm, $P_{atm} \approx 61$ kPa), la altura máxima del sifón se reduce a:
  $$h_{max} = \frac{61000 - 2300 - 7840}{9800} = \frac{50860}{9800} = 5.19 \text{ m}$$
  
  La menor presión atmosférica reduce drásticamente la capacidad del sifón.

* Los sifones reales tienen pérdidas por fricción en el tubo (proporcionales a la longitud y a $v^2$), que reducen la velocidad real y la altura máxima efectiva.

**4. Análisis de Sensibilidad:**
| Parámetro | Cambio | Efecto en presión en cima |
|-----------|--------|---------------------------|
| Altura del punto más alto | +10 cm | Presión -0.98 kPa |
| Velocidad (diferencia de altura) | +20% | Presión -3.1 kPa |
| Presión atmosférica (altitud) | -10% | Presión en cima -10.1 kPa |

**5. Extensión:**
Los acueductos romanos usaban sifones invertidos para cruzar valles profundos. El sifón de Gier (Francia, siglo I d.C.) cruzaba un valle de 20 m de profundidad con tubos de plomo de 25 cm de diámetro. Los modernos oleoductos usan sifones para cruzar ríos y cañones. El sifón de Alaskan Way Viaduct (Seattle) drena agua de lluvia bajo el nivel del mar mediante bombas de vacío que mantienen la presión negativa. En medicina, los sifones nasogástricos usan el mismo principio para drenaje gástrico.
```
---

## 📓 III. Actividades para el Portafolio Digital

Resuelve los siguientes 10 desafíos siguiendo el **Formato de 5-Bloques**. Para el Portafolio digital presenta **4 Desafíos** de tu elección.

---

### 🧠 Desafío 1: El Acueducto de Cumbe Mayo

El acueducto preinca de Cumbe Mayo (Cajamarca, ~1500 a.C.) transporta agua a través de un canal de piedra con pendiente mínima. En un tramo, el canal tiene sección rectangular de $w = 1.2$ m de ancho y agua fluyendo a $h = 0.4$ m de profundidad con velocidad $v = 0.8$ m/s.

* **El Reto:** Calcula el caudal volumétrico, la velocidad si el canal se estrecha a $w = 0.8$ m manteniendo la misma profundidad, y la diferencia de presión entre ambas secciones si el canal es horizontal.
* **Interpretación:** ¿Cómo lograron los constructores preincas mantener el flujo constante sin conocer la ecuación de Bernoulli? Relaciona con el principio de nivelación por pendiente constante.

---

### 🧠 Desafío 2: El Inyector de Riego por Aspersión

Un sistema de riego usa inyectores Venturi para mezclar fertilizante líquido. El agua entra al inyector a $P_1 = 300$ kPa y $v_1 = 2$ m/s. La garganta del Venturi tiene la mitad del diámetro de entrada.

* **El Reto:** Calcula la presión en la garganta, el caudal de agua si el diámetro de entrada es 2.5 cm, y la altura a la que puede succionar el fertilizante ($\rho = 1200$ kg/m³) desde un depósito abierto.
* **Análisis Crítico:** Si el fertilizante es más denso que el agua, ¿aumenta o disminuye la altura de succión respecto a usar agua pura? Justifica con la ecuación de Bernoulli.

---

### 🧠 Desafío 3: El Velocímetro del Avión de Línea

Un Boeing 737 vuela a 9000 m de altitud donde $\rho_{aire} = 0.47$ kg/m³. El tubo de Pitot mide $P_{total} = 32.5$ kPa y la presión estática ambiente es $P_{est} = 30.8$ kPa.

* **El Reto:** Calcula la velocidad del avión respecto al aire en km/h, el número de Mach si la velocidad del sonido a esa altitud es 325 m/s, y la lectura equivalente que mostraría el Pitot en Lima a nivel del mar con la misma velocidad.
* **Toma de Decisión:** Si el Pitot se congela parcialmente, reduciendo la lectura de $P_{total}$ en un 15%, ¿qué velocidad indicaría erróneamente el instrumento? ¿Es peligrosa esta lectura subestimada?

---

### 🧠 Desafío 4: El Tanque de Agua de la Olla de Moyobamba

Un tanque cilíndrico de $D = 2$ m y $H = 3$ m alimenta un sistema de agua potable en Moyobamba. Tiene dos orificios de drenaje: uno inferior de $d_1 = 3$ cm y uno lateral a 1 m del fondo de $d_2 = 2$ cm.

* **El Reto:** Calcula el tiempo de vaciado por cada orificio por separado, el tiempo si ambos abren simultáneamente, y la altura del chorro del orificio lateral medida desde el nivel del suelo (el tanque está sobre una torre de 8 m).
* **Análisis de Sensibilidad:** Durante la estación seca, la temperatura del agua sube de 20°C a 28°C. ¿Cómo afecta esto al tiempo de vaciado? Considera la variación de viscosidad y densidad.

---

### 🧠 Desafío 5: La Manguera de los Bomberos

Una manguera de bomberos tiene diámetro $D_1 = 10$ cm en la sección de suministro desde el camión. La boquilla de salida tiene $D_2 = 2.5$ cm. El agua sale a $v_2 = 25$ m/s.

* **El Reto:** Calcula la velocidad en la manguera de suministro, la presión manométrica requerida en el camión (asumiendo altura constante), y la altura máxima a la que puede llegar el chorro vertical.
* **Toma de Decisión:** Para incendios en edificios altos, ¿es más efectivo aumentar la presión en la bomba o reducir el diámetro de la boquilla? Compara ambas estrategias usando Bernoulli.

---

### 🧠 Desafío 6: El Medidor de Gas Doméstico

Un medidor de gas natural usa un diafragma que se desplaza por diferencia de presión. El gas fluye por un tubo de $D = 2$ cm con velocidad $v = 3$ m/s a $P = 2.5$ kPa manométrica y $\rho = 0.7$ kg/m³.

* **El Reto:** Calcula el caudal volumétrico y másico, la presión dinámica, y la presión total en la tubería. Si el medidor introduce una restricción que reduce la sección a la mitad, ¿cuál es la nueva presión a la salida?
* **Interpretación Profesional:** ¿Por qué los medidores de gas miden volumen a condiciones estándar (0°C, 1 atm) en lugar de volumen real? Explica la corrección por temperatura y presión.

---

### 🧠 Desafío 7: El Sifón de la Fuente de la Plaza de Armas

La fuente central de la Plaza de Armas de Lima usa un sifón oculto para recircular agua desde un reservorio inferior hasta una copa decorativa a 3 m de altura. El tubo tiene $D = 5$ cm.

* **El Reto:** Calcula la velocidad mínima de salida necesaria para que el sifón funcione, el caudal correspondiente, y la presión en la cima del sifón. Verifica si es mayor que la presión de vapor del agua a 20°C.
* **Análisis Crítico:** Si la temperatura del agua sube a 35°C en verano ($P_{vapor} = 5.6$ kPa), ¿se mantiene estable el sifón? ¿Qué altura máxima podría tener en esas condiciones?

---

### 🧠 Desafío 8: La Tubería del Oleoducto Norperuano

El oleoducto norperuano transporta petróleo ($\rho = 850$ kg/m³, $\mu = 0.25$ Pa·s) a través de una tubería de $D = 50$ cm. En un tramo horizontal, la presión cae de $P_1 = 4$ MPa a $P_2 = 3.5$ MPa en $L = 10$ km.

* **El Reto:** Aplica Bernoulli ideal para estimar la velocidad del flujo. Luego calcula el número de Reynolds ($Re = \frac{\rho v D}{\mu}$) y determina si el flujo es laminar ($Re < 2000$) o turbulento.
* **Evaluación:** Bernoulli ideal predice velocidad constante en tubería horizontal con igual diámetro, pero la presión cae. ¿De dónde proviene esta "pérdida" de energía? Introduce el concepto de pérdida por fricción.

---

### 🧠 Desafío 9: El Pulverizador Agrícola de la Chacra

Un pulverizador de mochila usa una boquilla Venturi conectada a una manguera de presión. El líquido insecticida ($\rho = 1050$ kg/m³) debe mezclarse con aire a $v_{aire} = 15$ m/s en una garganta de $A_2 = 0.3$ cm².

* **El Reto:** Calcula la presión en la garganta si la sección de entrada es $A_1 = 1.2$ cm² y la presión atmosférica es 100 kPa. ¿Puede succionar el insecticida desde un depósito a 30 cm debajo de la boquilla?
* **Extensión Creativa:** Diseña una boquilla mejorada que permita succionar desde 50 cm de profundidad manteniendo la misma velocidad de aire. ¿Qué parámetros modificas y cuáles son las limitaciones prácticas?

---

### 🧠 Desafío 10: El Reloj de Agua del Museo Larco

Un reloj de agua (clepsidra) del Museo Larco tiene forma cónica invertida: radio superior $R = 10$ cm, radio inferior $r = 2$ cm, altura $H = 30$ cm. El agua sale por un orificio de 3 mm de diámetro en la base.

* **El Reto:** Deriva la expresión del tiempo de vaciado para geometría cónica (el área del tanque varía con la altura). Calcula el tiempo de vaciado completo y compárelo con un cilindro de igual altura y volumen.
* **Análisis de Sensibilidad:** Los relojes de agua antiguos usaban flotadores para mantener nivel constante. ¿Cuánto se adelantaría o atrasaría este reloj en 1 hora si la temperatura del agua varía de 15°C a 25°C?
s
---
