# Sesión 4: Ondas Mecánicas

## 📌 I. Fundamento Teórico

En esta sesión se estudia la propagación de perturbaciones mecánicas a través de medios materiales, el análisis matemático de ondas armónicas, la velocidad de propagación en diferentes medios, y los fenómenos de superposición que dan origen a ondas estacionarias en cuerdas y tubos.

---

### 1.1. Ondas Mecánicas. Tipos de Ondas. Elementos de una Onda

**Onda mecánica:** Es una perturbación que se propaga a través de un medio material, transportando energía y momento sin transportar materia.

**Clasificación según la dirección de propagación:**

| Tipo de onda | Característica | Ejemplo |
|-------------|----------------|---------|
| **Transversal** | La perturbación es perpendicular a la dirección de propagación | Onda en cuerda, onda S sísmica |
| **Longitudinal** | La perturbación es paralela a la dirección de propagación | Sonido en aire, onda P sísmica |
| **Superficial** | Se propagan en la interfaz entre dos medios | Ondas en el agua, ondas de Rayleigh |

**Elementos de una onda:**

* **Amplitud ($A$):** Máximo desplazamiento respecto a la posición de equilibrio.
* **Longitud de onda ($\lambda$):** Distancia entre dos puntos equivalentes consecutivos.
* **Período ($T$):** Tiempo para completar un ciclo.
* **Frecuencia ($f$):** Número de ciclos por unidad de tiempo. $f = \frac{1}{T}$
* **Número de onda ($k$):** $k = \frac{2\pi}{\lambda}$
* **Frecuencia angular ($\omega$):** $\omega = 2\pi f = \frac{2\pi}{T}$
* **Velocidad de propagación ($v$):** $v = \lambda f = \frac{\lambda}{T} = \frac{\omega}{k}$

> **💡 Regla de Oro:** La velocidad de una onda mecánica depende exclusivamente de las propiedades del medio (tensión, densidad, elasticidad), no de la amplitud ni la frecuencia.

---

### 1.2. Función de Onda Armónica

Una onda armónica que se propaga en la dirección $+x$ tiene la forma:

$$y(x,t) = A\sin(kx - \omega t + \phi_0)$$

o equivalentemente:

$$y(x,t) = A\sin\left[\frac{2\pi}{\lambda}(x - vt) + \phi_0\right]$$

donde:
* $y(x,t)$: elongación en la posición $x$ y tiempo $t$
* $\phi_0$: fase inicial
* El signo $(kx - \omega t)$ indica propagación hacia $+x$
* El signo $(kx + \omega t)$ indica propagación hacia $-x$

**Relaciones fundamentales:**

$$v = \frac{\omega}{k} = \lambda f$$

---

### 1.3. Velocidad de Propagación de una Onda en una Cuerda

Para una cuerda de densidad lineal de masa $\mu$ (kg/m) sometida a una tensión $F_T$:

$$v = \sqrt{\frac{F_T}{\mu}}$$

**Factores que afectan la velocidad:**

| Factor | Efecto en $v$ | Justificación |
|--------|---------------|---------------|
| Aumentar tensión $F_T$ | $v$ aumenta | Mayor fuerza restauradora |
| Aumentar densidad $\mu$ | $v$ disminuye | Mayor inercia del medio |
| Aumentar temperatura | $v$ aumenta (ligeramente) | Expansión térmica reduce $\mu$ |

> **💡 Regla de Oro:** En una cuerda, la velocidad de la onda no depende de la frecuencia. Todas las frecuencias viajan a la misma velocidad (medio no dispersivo).

---

### 1.4. Ondas Sonoras. Propagación del Sonido en Diferentes Medios

El sonido es una onda longitudinal que se propaga mediante compresiones y rarefacciones del medio.

**Ecuación de onda sonora (variación de presión):**

$$\Delta P(x,t) = \Delta P_{max}\sin(kx - \omega t)$$

**Velocidad del sonido en diferentes medios:**

| Medio | Velocidad aproximada (m/s) | Condiciones |
|-------|---------------------------|-------------|
| Aire (20°C) | 343 | A nivel del mar |
| Agua | 1482 | A 20°C |
| Acero | 5960 | A temperatura ambiente |
| Vidrio | 5640 | A temperatura ambiente |
| Madera (roble) | 3850 | A lo largo de la fibra |

**Dependencia con la temperatura (en gases):**

$$v = 331 + 0.6T_c$$

donde $T_c$ es la temperatura en °C.

**Intensidad sonora:**

$$I = \frac{P}{A} = \frac{1}{2}\rho v \omega^2 A^2$$

**Nivel de intensidad en decibelios:**

$$\beta = 10\log\left(\frac{I}{I_0}\right)$$

donde $I_0 = 10^{-12}$ W/m² es el umbral de audición.

---

### 1.5. Superposición de Ondas. Ondas Estacionarias

**Principio de superposición:** Cuando dos o más ondas se encuentran en un mismo punto del espacio, el desplazamiento resultante es la suma algebraica de los desplazamientos individuales.

$$y_{total}(x,t) = y_1(x,t) + y_2(x,t)$$

**Ondas estacionarias:** Resultan de la superposición de dos ondas armónicas de igual amplitud, frecuencia y longitud de onda que viajan en direcciones opuestas:

$$y_1 = A\sin(kx - \omega t)$$
$$y_2 = A\sin(kx + \omega t)$$

$$y = y_1 + y_2 = 2A\sin(kx)\cos(\omega t)$$

**Características:**

* **Nodos:** Puntos de amplitud cero (desplazamiento siempre nulo). Ocurren donde $\sin(kx) = 0$, es decir, $x = n\frac{\lambda}{2}$ con $n = 0, 1, 2, ...$
* **Vientres (antinodos):** Puntos de máxima amplitud ($2A$). Ocurren donde $|\sin(kx)| = 1$, es decir, $x = (2n+1)\frac{\lambda}{4}$

> **💡 Regla de Oro:** En una onda estacionaria no hay propagación de energía neta. La energía se intercambia entre energía cinética (máxima en los nodos) y energía potencial (máxima en los vientres).

---

### 1.6. Ondas Estacionarias en Cuerdas

Para una cuerda de longitud $L$ fija en ambos extremos, las condiciones de frontera imponen nodos en $x = 0$ y $x = L$.

**Longitudes de onda permitidas:**

$$\lambda_n = \frac{2L}{n} \quad \text{con } n = 1, 2, 3, ...$$

**Frecuencias naturales (armónicos):**

$$f_n = \frac{v}{\lambda_n} = \frac{nv}{2L} = nf_1$$

donde $f_1 = \frac{v}{2L}$ es la **frecuencia fundamental**.

| Modo ($n$) | Nombre | Nodos | Vientres | Frecuencia |
|-----------|--------|-------|----------|------------|
| 1 | Fundamental | 2 | 1 | $f_1$ |
| 2 | Segundo armónico | 3 | 2 | $2f_1$ |
| 3 | Tercer armónico | 4 | 3 | $3f_1$ |
| $n$ | $n$-ésimo armónico | $n+1$ | $n$ | $nf_1$ |

---

### 1.7. Ondas Estacionarias en Tubos Abiertos

En un tubo abierto en ambos extremos, hay vientres de desplazamiento en cada extremo.

**Longitudes de onda permitidas:**

$$\lambda_n = \frac{2L}{n} \quad \text{con } n = 1, 2, 3, ...$$

**Frecuencias naturales:**

$$f_n = \frac{nv}{2L} = nf_1$$

> **Nota:** Un tubo abierto-abierto tiene el mismo espectro de frecuencias que una cuerda fija en ambos extremos. Todos los armónicos están presentes.

---

### 1.8. Ondas Estacionarias en Tubos Cerrados

En un tubo cerrado en un extremo y abierto en el otro, hay un nodo en el extremo cerrado y un vientre en el extremo abierto.

**Longitudes de onda permitidas:**

$$\lambda_n = \frac{4L}{n} \quad \text{con } n = 1, 3, 5, ... \text{ (solo impares)}$$

**Frecuencias naturales:**

$$f_n = \frac{nv}{4L} = nf_1$$

donde $f_1 = \frac{v}{4L}$ es la frecuencia fundamental.

| Modo ($n$) | Nombre | Nodos | Vientres | Frecuencia |
|-----------|--------|-------|----------|------------|
| 1 | Fundamental | 1 | 1 | $f_1$ |
| 3 | Tercer armónico | 2 | 2 | $3f_1$ |
| 5 | Quinto armónico | 3 | 3 | $5f_1$ |
| $n$ (impar) | $n$-ésimo armónico | $\frac{n+1}{2}$ | $\frac{n+1}{2}$ | $nf_1$ |

> **💡 Regla de Oro:** Un tubo cerrado-abierto solo produce armónicos impares. Esto le da un timbre característico "hueco" comparado con un tubo abierto.

---

## 🚀 II. Problemas Resueltos

---

### 🧩 Problema N° 1

```{admonition} La Cuerda del Violín
:class: important
**Situación:** Una cuerda de violín de longitud $L = 33$ cm tiene una densidad lineal de masa $\mu = 0.65$ g/m. El violinista necesita producir la nota La₃ (frecuencia fundamental $f_1 = 440$ Hz). Calcular: (a) la velocidad de propagación de la onda en la cuerda, (b) la tensión requerida, (c) la longitud de onda del sonido emitido en el aire, y (d) la frecuencia del segundo armónico.
````

```{admonition} Solución
:class: dropdown hint
**1. Planteamiento:**
* **Ruta de la solución:** Usar las relaciones de ondas estacionarias en cuerdas fijas en ambos extremos. La frecuencia fundamental determina la velocidad, y de ella la tensión. La frecuencia del sonido emitido coincide con la frecuencia de vibración de la cuerda.
* **Predicción cualitativa:** La tensión será considerable (decenas de newtons) para lograr la alta frecuencia de 440 Hz en una cuerda corta y ligera.

**2. Resolución:**

**Datos:**
* $L = 0.33$ m
* $\mu = 0.65 \times 10^{-3}$ kg/m
* $f_1 = 440$ Hz
* $v_{aire} = 343$ m/s

**(a) Velocidad de propagación en la cuerda:**
De $f_1 = \frac{v}{2L}$:
$$v = 2Lf_1 = 2 \times 0.33 \times 440 = 290.4 \text{ m/s}$$

**(b) Tensión requerida:**
De $v = \sqrt{\frac{F_T}{\mu}}$:
$$F_T = \mu v^2 = 0.65 \times 10^{-3} \times (290.4)^2$$
$$F_T = 0.65 \times 10^{-3} \times 84332.2 \approx 54.8 \text{ N}$$

**(c) Longitud de onda del sonido en el aire:**
La frecuencia del sonido es igual a la frecuencia de vibración de la cuerda ($f = 440$ Hz):
$$\lambda_{aire} = \frac{v_{aire}}{f} = \frac{343}{440} \approx 0.78 \text{ m} = 78 \text{ cm}$$

**(d) Segundo armónico:**
$$f_2 = 2f_1 = 2 \times 440 = 880 \text{ Hz}$$

**3. Discusión Crítica:**
* La longitud de onda en la cuerda ($\lambda_1 = 2L = 66$ cm) es diferente de la longitud de onda en el aire (78 cm). La frecuencia se conserva al cambiar de medio, pero la velocidad y la longitud de onda cambian.
* La tensión de 54.8 N (~5.6 kgf) es razonable para una cuerda de acero de violín. Las cuerdas graves (La, Mi) tienen mayor masa y requieren mayor tensión.
* Si la temperatura aumenta, la cuerda se dilata (aumenta $L$, disminuye $\mu$ ligeramente). El efecto dominante es el aumento de $L$, que reduce $f_1$: el violín se desafina gravemente.

**4. Análisis de Sensibilidad:**
| Parámetro | Cambio | Efecto en $f_1$ |
|-----------|--------|-----------------|
| Longitud $L$ | -1% (presionar traste) | $f_1$ aumenta 1% (~4.4 Hz) |
| Tensión $F_T$ | +1% (afinar más agudo) | $f_1$ aumenta 0.5% (~2.2 Hz) |
| Densidad $\mu$ | +1% (cuerda más gruesa) | $f_1$ disminuye 0.5% (~2.2 Hz) |

**5. Extensión:**
Los violines modernos usan cuerdas de núcleo de acero o materiales sintéticos (perlon) recubiertos de aluminio o plata. Las cuerdas de tripa (tradicionales) son más sensibles a la humedad, cambiando $\mu$ y desafinando el instrumento. Los afinadores electrónicos miden $f_1$ con precisión de 0.1 Hz, detectando cambios de tensión menores a 0.01 N.
```
---

### 🧩 Problema N° 2

```{admonition} El Eco en el Cañón
:class: important
**Situación:** Un excursionista grita frente a una pared de roca en el Cañón del Colca (Perú). El eco regresa después de $\Delta t = 4.2$ s. La temperatura ambiente es $T_c = 15$°C. Calcular: (a) la velocidad del sonido en esas condiciones, (b) la distancia a la pared, (c) la longitud de onda del grito si su frecuencia es $f = 850$ Hz, y (d) la frecuencia mínima audible a esa distancia si la intensidad del grito a 1 m es $I_0 = 10^{-3}$ W/m² y el umbral de audición es $10^{-12}$ W/m².
```

```{admonition} Solución
:class: dropdown hint
**1. Planteamiento:**
* **Ruta de la solución:** Calcular la velocidad del sonido con la corrección por temperatura. La distancia al obstáculo es la mitad de la distancia total recorrida por el sonido (ida y vuelta). La atenuación sigue la ley del cuadrado inverso para intensidad.
* **Predicción cualitativa:** La distancia será de varios cientos de metros. La atenuación por distancia reducirá significativamente la intensidad percibida en el regreso.

**2. Resolución:**

**(a) Velocidad del sonido a 15°C:**
$$v = 331 + 0.6T_c = 331 + 0.6 \times 15 = 331 + 9 = 340 \text{ m/s}$$

**(b) Distancia a la pared:**
El sonido recorre ida y vuelta en 4.2 s:
$$d_{total} = v \times \Delta t = 340 \times 4.2 = 1428 \text{ m}$$
$$d_{pared} = \frac{d_{total}}{2} = 714 \text{ m}$$

**(c) Longitud de onda:**
$$\lambda = \frac{v}{f} = \frac{340}{850} = 0.4 \text{ m} = 40 \text{ cm}$$

**(d) Intensidad del eco y frecuencia mínima audible:**
La intensidad disminuye con el cuadrado de la distancia:
$$\frac{I_1}{I_2} = \frac{r_2^2}{r_1^2}$$

Intensidad a 714 m (ida):
$$I_{ida} = I_0 \times \left(\frac{1}{714}\right)^2 = 10^{-3} \times 1.96 \times 10^{-6} = 1.96 \times 10^{-9} \text{ W/m}^2$$

La pared refleja parte de la energía (coeficiente de reflexión $\approx 0.8$ para roca). El eco de regreso sufre nueva atenuación:
$$I_{eco} \approx 0.8 \times I_{ida} \times \left(\frac{1}{714}\right)^2 \times (714)^2 = 0.8 \times I_{ida} = 1.57 \times 10^{-9} \text{ W/m}^2$$

Nivel de intensidad del eco:
$$\beta = 10\log\left(\frac{1.57 \times 10^{-9}}{10^{-12}}\right) = 10\log(1570) \approx 10 \times 3.2 = 32 \text{ dB}$$

> **Nota:** El oído humano puede detectar frecuencias desde 20 Hz hasta 20 kHz. A 32 dB, todas las frecuencias audibles son perceptibles, aunque con menor claridad. La pregunta sobre "frecuencia mínima audible" se refiere al umbral de frecuencia (20 Hz), no de intensidad.

**3. Discusión Crítica:**
* El eco es perceptible (32 dB equivale a un susurro suave). En un cañón real con múltiples paredes, pueden producirse ecos múltiples y reverberación.
* La velocidad del sonido varía con la altitud. En el Cañón del Colca (a ~3600 msnm), la presión atmosférica es menor, pero la temperatura también lo es. El modelo $v = 331 + 0.6T_c$ sigue siendo válido si se mide la temperatura local.
* La absorción atmosférica atenúa frecuencias altas más que bajas. Un grito agudo (850 Hz) se atenúa más que un grave por absorción molecular del aire.

**4. Análisis de Sensibilidad:**
| Parámetro | Variación | Efecto en distancia |
|-----------|-----------|---------------------|
| Temperatura | +10°C | Distancia aparente +1.8% (+13 m) |
| Tiempo de eco | +0.1 s | Distancia +17 m |
| Humedad relativa | +50% | Atenuación adicional -2 dB |

**5. Extensión:**
Los murciélagos utilizan ecolocalización con ultrasonidos (20-200 kHz) para navegar. Su sistema es tan preciso que pueden detectar insectos de 2 mm de diámetro a 5 m de distancia. Los sistemas de sonar marino usan el mismo principio con ondas de baja frecuencia (1-50 kHz) que se propagan mejor en el agua ($v \approx 1500$ m/s). Los sismólogos usan la diferencia de tiempos de llegada entre ondas P (longitudinales, más rápidas) y ondas S (transversales, más lentas) para localizar epicentros.
```
---

### 🧩 Problema N° 3

```{admonition} La Guitarra Eléctrica
:class: important
**Situación:** Una guitarra eléctrica tiene una cuerda de acero de longitud escala $L = 64.8$ cm. El guitarrista presiona la cuerda en el traste 12 (a la mitad de la longitud) para producir una nota una octava más aguda. Calcular: (a) la relación entre la frecuencia fundamental presionada y la al aire libre, (b) la nueva frecuencia fundamental si la nota al aire libre es Mi₂ ($f = 82.4$ Hz), (c) las frecuencias de los tres primeros armónicos en ambas configuraciones, y (d) la posición donde debe presionar para obtener el Do ($f = 130.8$ Hz) si la frecuencia al aire libre es La ($f = 110$ Hz).
```
```{admonition} Solución
:class: dropdown hint
**1. Planteamiento:**
* **Ruta de la solución:** La frecuencia de una cuerda fija-fija es inversamente proporcional a su longitud vibrante ($f \propto 1/L$). Presionar en el traste 12 reduce $L$ a la mitad, duplicando la frecuencia (octava superior).
* **Predicción cualitativa:** Los armónicos de la cuerda presionada serán el doble de los de la cuerda al aire libre. Para obtener Do desde La, se necesita una relación de frecuencias de 130.8/110 ≈ 1.189, que corresponde a una reducción de longitud.

**2. Resolución:**

**(a) Relación de frecuencias:**
Al presionar en el traste 12, la longitud vibrante es $L' = L/2$:
$$\frac{f'}{f} = \frac{L}{L'} = \frac{L}{L/2} = 2$$

La frecuencia se duplica (sube una octava).

**(b) Nueva frecuencia fundamental:**
$$f' = 2 \times 82.4 = 164.8 \text{ Hz}$$

> **Nota:** Mi₃ tiene frecuencia 164.8 Hz, confirmando el cálculo.

**(c) Armónicos:**

| Modo | Al aire libre ($L = 64.8$ cm) | Presionada ($L' = 32.4$ cm) |
|------|------------------------------|------------------------------|
| Fundamental ($n=1$) | 82.4 Hz | 164.8 Hz |
| 2° armónico ($n=2$) | 164.8 Hz | 329.6 Hz |
| 3° armónico ($n=3$) | 247.2 Hz | 494.4 Hz |

**(d) Posición para obtener Do desde La:**
$$\frac{f_{Do}}{f_{La}} = \frac{130.8}{110} = 1.189 = \frac{L}{L''}$$

$$L'' = \frac{L}{1.189} = \frac{64.8}{1.189} \approx 54.5 \text{ cm}$$

La posición del traste medida desde el puente:
$$x = L - L'' = 64.8 - 54.5 = 10.3 \text{ cm}$$

> **Verificación:** En una guitarra estándar, el traste 2 está aproximadamente a 10.3 cm del cejillo (inicio de la cuerda), lo cual coincide con la posición calculada para obtener Si (no Do exactamente, debido a la afinación temperada).

**3. Discusión Crítica:**
* La afinación temperada divide la octava en 12 semitonos iguales (relación de frecuencias $2^{1/12} \approx 1.059$). La relación Do/La = 130.8/110 = 1.189 no es exactamente una relación temperada simple, lo que introduce pequeñas discrepancias.
* Los armónicos superiores determinan el timbre del instrumento. Una guitarra eléctrica con distorsión enfatiza los armónicos impares, dando su sonido característico "grueso".
* La posición de los trastes sigue una progresión geométrica: $x_n = L(1 - 2^{-n/12})$.

**4. Análisis de Sensibilidad:**
| Error en posición del traste | Efecto en frecuencia | Desafinación perceptible |
|------------------------------|----------------------|--------------------------|
| +1 mm | +0.3 Hz | Sí (umbral ~0.5 Hz) |
| +2 mm | +0.6 Hz | Sí, claramente |
| +5 mm | +1.5 Hz | Muy desafinado |

**5. Extensión:**
Las guitarras eléctricas usan pastillas (bobinas magnéticas) que detectan la vibración de la cuerda de acero. Las pastillas "humbucker" usan dos bobinas en oposición para cancelar el zumbido de la red eléctrica (60 Hz en América, 50 Hz en Europa). El efecto "wah-wah" modula electrónicamente el filtro de frecuencias, enfatizando diferentes armónicos a lo largo de la nota.
```
---

### 🧩 Problema N° 4

```{admonition} El Órgano de Tubos
:class: important
**Situación:** Un órgano de tubos tiene un tubo abierto de longitud $L_a = 1.2$ m y un tubo cerrado de longitud $L_c = 1.8$ m, ambos a temperatura ambiente ($v_{sonido} = 343$ m/s). Calcular: (a) la frecuencia fundamental de cada tubo, (b) las frecuencias de los primeros cuatro armónicos audibles de cada tubo, (c) el armónico común más bajo entre ambos tubos, y (d) la longitud que debería tener un tubo cerrado para que su fundamental coincida con la fundamental del tubo abierto.
```

```{admonition} Solución
:class: dropdown hint
**1. Planteamiento:**
* **Ruta de la solución:** Aplicar las fórmulas de frecuencias naturales para tubos abiertos ($f_n = nv/2L$, todos los $n$) y cerrados ($f_n = nv/4L$, solo $n$ impares). Comparar espectros para encontrar coincidencias.
* **Predicción cualitativa:** El tubo cerrado más largo tendrá fundamental más grave que el abierto más corto. Los espectros serán diferentes: el abierto tiene todos los armónicos, el cerrado solo los impares.

**2. Resolución:**

**(a) Frecuencias fundamentales:**

**Tubo abierto:**
$$f_{1a} = \frac{v}{2L_a} = \frac{343}{2 \times 1.2} = \frac{343}{2.4} \approx 142.9 \text{ Hz}$$

**Tubo cerrado:**
$$f_{1c} = \frac{v}{4L_c} = \frac{343}{4 \times 1.8} = \frac{343}{7.2} \approx 47.6 \text{ Hz}$$

**(b) Armónicos audibles (hasta ~20 kHz):**

**Tubo abierto ($f_{na} = n \times 142.9$ Hz):**
| $n$ | Frecuencia (Hz) | Nota aproximada |
|-----|-----------------|-----------------|
| 1 | 142.9 | Re#₃ |
| 2 | 285.8 | Re#₄ |
| 3 | 428.7 | La#₄ |
| 4 | 571.6 | Re#₅ |

**Tubo cerrado ($f_{nc} = n \times 47.6$ Hz, $n$ impar):**
| $n$ | Frecuencia (Hz) | Nota aproximada |
|-----|-----------------|-----------------|
| 1 | 47.6 | Sol#₁ |
| 3 | 142.9 | Re#₃ |
| 5 | 238.1 | La#₃ |
| 7 | 333.3 | Mi#₄ |

**(c) Armónico común más bajo:**
Comparando las tablas, ambos tubos comparten **142.9 Hz**:
* Tubo abierto: $n = 1$ (fundamental)
* Tubo cerrado: $n = 3$ (tercer armónico)

**(d) Longitud del tubo cerrado para igualar fundamental del abierto:**
$$f_{1c}' = f_{1a} = 142.9 \text{ Hz}$$

$$L_c' = \frac{v}{4f_{1c}'} = \frac{343}{4 \times 142.9} = \frac{343}{571.6} \approx 0.6 \text{ m} = 60 \text{ cm}$$

> **Verificación:** Un tubo cerrado debe tener la mitad de longitud que uno abierto para producir la misma fundamental ($L_c = L_a/2$).

**3. Discusión Crítica:**
* El tubo cerrado de 1.8 m produce una fundamental muy grave (47.6 Hz, cerca del límite inferior de audición). Los tubos graves de órgano pueden medir más de 5 m.
* La ausencia de armónicos pares en tubos cerrados les da un timbre "hueco" o "flautado" característico. Los tubos abiertos suenan más "brillantes" por la presencia de todos los armónicos.
* En la práctica, los tubos de órgano no son cilindros perfectos; su forma cónica o sus bocales modifican el espectro de armónicos.

**4. Análisis de Sensibilidad:**
| Parámetro | Cambio | Efecto en $f_1$ |
|-----------|--------|-----------------|
| Longitud del tubo | +10% | $f_1$ disminuye 10% |
| Temperatura ambiente | +10°C | $f_1$ aumenta 1.8% |
| Densidad del aire (altitud) | -20% | $f_1$ aumenta 0.5% (pequeño efecto) |

**5. Extensión:**
El órgano de la catedral de Passau (Alemania) tiene 17,974 tubos, el mayor órgano de iglesia del mundo. Sus tubos graves miden más de 10 m y producen frecuencias de 16 Hz (infrasonido perceptible como vibración más que como sonido). Los órganos modernos usan transductores electromagnéticos para simular tubos inexistentes, reduciendo costos y espacio.
```
---

### 🧩 Problema N° 5

```{admonition} Interferencia en el Lago
:class: important
**Situación:** Dos fuentes de ondas idénticas en un lago generan ondas circulares de $\lambda = 0.8$ m y amplitud $A = 5$ cm. Las fuentes están separadas $d = 3.2$ m y oscilan en fase. Calcular: (a) la posición de las líneas nodales (destructiva) en la línea que une las fuentes, (b) la posición de las líneas antinodales (constructiva) en esa misma línea, (c) el número total de nodos en el plano del lago, y (d) la amplitud resultante en el punto medio entre las fuentes.
```

```{admonition} Solución
:class: dropdown hint
**1. Planteamiento:**
* **Ruta de la solución:** Aplicar el principio de superposición. La interferencia constructiva ocurre cuando la diferencia de caminos es múltiplo entero de $\lambda$. La destructiva ocurre cuando es semientero.
* **Predicción cualitativa:** Habrá múltiples nodos y antinodos entre las fuentes. El patrón será simétrico respecto al punto medio.

**2. Resolución:**

**Condiciones de interferencia:**

**Constructiva (antinodos):**
$$\Delta r = r_2 - r_1 = m\lambda \quad \text{con } m = 0, \pm 1, \pm 2, ...$$

**Destructiva (nodos):**
$$\Delta r = r_2 - r_1 = \left(m + \frac{1}{2}\right)\lambda \quad \text{con } m = 0, \pm 1, \pm 2, ...$$

**(a) Nodos en la línea que une las fuentes:**
Tomamos el origen en la fuente 1, fuente 2 en $x = 3.2$ m. Para un punto $x$ entre las fuentes:
$$r_1 = x, \quad r_2 = 3.2 - x$$
$$\Delta r = (3.2 - x) - x = 3.2 - 2x$$

Condición de nodo:
$$3.2 - 2x = \left(m + \frac{1}{2}\right) \times 0.8$$

Para $m = 0$: $3.2 - 2x = 0.4 \Rightarrow x = 1.4$ m
Para $m = 1$: $3.2 - 2x = 1.2 \Rightarrow x = 1.0$ m
Para $m = 2$: $3.2 - 2x = 2.0 \Rightarrow x = 0.6$ m
Para $m = 3$: $3.2 - 2x = 2.8 \Rightarrow x = 0.2$ m

Por simetría, también hay nodos en $x = 1.8$ m, $x = 2.2$ m, $x = 2.6$ m, $x = 3.0$ m.

**Nodos en la línea:** $x = 0.2, 0.6, 1.0, 1.4, 1.8, 2.2, 2.6, 3.0$ m (8 nodos)

**(b) Antinodos en la línea que une las fuentes:**
$$3.2 - 2x = m \times 0.8$$

Para $m = 0$: $x = 1.6$ m (punto medio)
Para $m = 1$: $x = 1.2$ m
Para $m = 2$: $x = 0.8$ m
Para $m = 3$: $x = 0.4$ m
Para $m = 4$: $x = 0$ m (fuente 1)

Por simetría: $x = 2.0, 2.4, 2.8, 3.2$ m

**Antinodos en la línea:** $x = 0, 0.4, 0.8, 1.2, 1.6, 2.0, 2.4, 2.8, 3.2$ m (9 antinodos, incluyendo fuentes)

**(c) Número total de nodos en el plano:**
La condición de nodo define hipérbolas en el plano. El número máximo de nodos está limitado por:
$$|\Delta r| \leq d \Rightarrow \left|m + \frac{1}{2}\right| \leq \frac{d}{\lambda} = \frac{3.2}{0.8} = 4$$

$$|m + 0.5| \leq 4 \Rightarrow -4.5 \leq m \leq 3.5$$

Valores de $m$: $-4, -3, -2, -1, 0, 1, 2, 3$ (8 valores)

Cada valor de $m$ corresponde a una hipérbola nodal (una rama a cada lado del eje). En total hay **16 líneas nodales** (8 pares simétricos).

**(d) Amplitud en el punto medio:**
En $x = 1.6$ m, $r_1 = r_2 = 1.6$ m. Las ondas llegan en fase (constructiva).

$$y_{total} = y_1 + y_2 = A\sin(kr_1 - \omega t) + A\sin(kr_2 - \omega t)$$

Como $r_1 = r_2$:
$$y_{total} = 2A\sin(kr_1 - \omega t)$$

La amplitud resultante es:
$$A_{total} = 2A = 2 \times 5 = 10 \text{ cm}$$

**3. Discusión Crítica:**
* El patrón de interferencia es estacionario en el espacio (nodos y antinodos fijos) aunque las ondas individuales se propagan. Esto es característico de ondas coherentes.
* Si las fuentes no oscilaran en fase (diferencia de fase $\phi \neq 0$), las posiciones de nodos y antinodos se desplazarían, pero el patrón seguiría siendo periódico.
* En el lago real, la amplitud disminuye con la distancia por atenuación (viscosidad del agua), por lo que la interferencia perfecta solo ocurre cerca de las fuentes.

**4. Análisis de Sensibilidad:**
| Parámetro | Cambio | Efecto en el patrón |
|-----------|--------|---------------------|
| Separación $d$ | +50% | Más nodos, más cercanos |
| Longitud de onda $\lambda$ | +50% | Menos nodos, más separados |
| Diferencia de fase | $\pi$ rad | Nodos y antinodos intercambiados |

**5. Extensión:**
La interferencia de ondas es fundamental en óptica (interferómetros de Michelson, holografía), acústica (cancelación activa de ruido en auriculares), y física cuántica (experimento de la doble rendija). Los sistemas de sonar multihaz usan arreglos de fuentes para crear haces direccionales mediante interferencia constructiva en ángulos específicos.
```
---

### 🧩 Problema N° 6
```{admonition} La Soga del Tendero

:class: important
**Situación:** Un tendero cuelga ropa en una soga de lavar de longitud $L = 6$ m, tensión $F_T = 50$ N y densidad lineal $\mu = 0.04$ kg/m. Un niño agita un extremo transversalmente con frecuencia variable. Calcular: (a) las frecuencias de los tres primeros modos normales, (b) la velocidad de propagación en la cuerda, (c) la frecuencia que debe aplicar el niño para excitar el segundo modo y la posición donde debe tocar para no perturbar ese modo, y (d) la longitud de onda del sonido emitido al aire por la cuerda vibrando en su fundamental.
```

```{admonition} Solución
:class: dropdown hint
**1. Planteamiento:**
* **Ruta de la solución:** La soga es una cuerda fija en ambos extremos (los postes del tendedero). Los modos normales cumplen la condición de nodos en los extremos. La excitación resonante requiere coincidir con una frecuencia natural.
* **Predicción cualitativa:** Los modos serán graves (cuerda larga y pesada). El segundo modo tendrá un nodo en el centro, por lo que tocar el centro no lo excitaría.

**2. Resolución:**

**(a) y (b) Velocidad y frecuencias naturales:**

**Velocidad de propagación:**
$$v = \sqrt{\frac{F_T}{\mu}} = \sqrt{\frac{50}{0.04}} = \sqrt{1250} \approx 35.36 \text{ m/s}$$

**Frecuencias naturales:**
$$f_n = \frac{nv}{2L} = \frac{n \times 35.36}{2 \times 6} = \frac{35.36n}{12} \approx 2.947n \text{ Hz}$$

| Modo ($n$) | Frecuencia (Hz) | Longitud de onda en cuerda (m) |
|-----------|-----------------|--------------------------------|
| 1 | 2.95 | 12.0 |
| 2 | 5.89 | 6.0 |
| 3 | 8.84 | 4.0 |

**(c) Excitación del segundo modo:**
El niño debe agitar con $f = 5.89$ Hz.

Para no perturbar el segundo modo, debe tocar en un **nodo** de ese modo. El segundo modo ($n=2$) tiene nodos en:
$$x = 0, \frac{L}{2}, L$$

Es decir, en $x = 0$ m (extremo), $x = 3$ m (centro), y $x = 6$ m (extremo).

> **Nota práctica:** Agitar un extremo excita todos los modos. Para excitar selectivamente el segundo modo, el niño debería tocar el centro ($x = 3$ m) mientras agita, forzando un nodo allí y suprimiendo los modos impares.

**(d) Longitud de onda del sonido emitido:**
La frecuencia del sonido es igual a la frecuencia de vibración de la cuerda ($f_1 = 2.95$ Hz).

$$\lambda_{aire} = \frac{v_{aire}}{f_1} = \frac{343}{2.95} \approx 116.3 \text{ m}$$

> **Observación:** Esta longitud de onda es enorme (más de 100 m), correspondiente a un sonido grave casi infrasónico. La soga emite poca energía acústica a esta frecuencia.

**3. Discusión Crítica:**
* La soga del tendero es un ejemplo de sistema continuo con infinitos modos normales. En la práctica, la fricción del aire y la rigidez de la cuerda limitan el número de modos observables.
* La tensión de 50 N es moderada. Si la ropa mojada aumenta la carga, la soga se deforma verticalmente, cambiando la tensión efectiva y desafinando los modos.
* El sonido emitido por la cuerda es ineficiente a 2.95 Hz porque la longitud de onda en el aire (116 m) es mucho mayor que la longitud de la cuerda (6 m). Hay desacoplamiento de impedancias.

**4. Análisis de Sensibilidad:**
| Parámetro | Cambio | Efecto en $f_1$ |
|-----------|--------|-----------------|
| Tensión $F_T$ | +10% | $f_1$ aumenta 4.9% ($\propto \sqrt{F_T}$) |
| Longitud $L$ | +10% | $f_1$ disminuye 10% ($\propto 1/L$) |
| Carga (masa) | +10% | $f_1$ disminuye 4.9% ($\mu$ aumenta) |

**5. Extensión:**
Los puentes colgantes (Golden Gate, Puente de Brooklyn) pueden oscilar en modos normales bajo viento o tráfico peatonal. El colapso del Puente de Tacoma Narrows (1940) ocurrió por resonancia aeroelástica: el viento excitó un modo de torsión de la cubierta. Los ingenieros civiles ahora diseñan puentes con amortiguadores y formas aerodinámicas para evitar la excitación resonante. Los cables de suspensión se prueban en túneles de viento para identificar y suprimir modos peligrosos.
```
---

## 📓 III. Actividades para el Portafolio Digital

Resuelve los siguientes 10 desafíos siguiendo el **Formato de 5-Bloques**. Para el Portafolio digital presenta **4 Desafíos** de tu elección.

---

### 🧠 Desafío 1
**El Diapasón del Afinador**

Un diapasón de acero vibra con frecuencia $f = 440$ Hz, generando una onda sonora en el aire a 20°C. La amplitud de presión máxima es $\Delta P_{max} = 0.2$ Pa y la densidad del aire es $\rho = 1.2$ kg/m³.

* **El Reto:** Calcula la longitud de onda del sonido, la amplitud de desplazamiento de las moléculas de aire, y la intensidad del sonido a 1 m del diapasón.
* **Interpretación:** ¿Por qué los afinadores electrónicos detectan la frecuencia fundamental aunque el oído humano perciba múltiples armónicos?
* **Simulación GeoGebra:** [Simulación de Onda Sonora](https://www.geogebra.org/m/XKfpRjQH) - Visualiza la propagación de la onda de presión.

---

### 🧠 Desafío 2
**El Puente de Cuerdas del Charango**

Un charango tiene una cuerda de longitud $L = 37$ cm y densidad lineal $\mu = 0.8$ g/m. El luthier necesita que suene La₄ ($f = 440$ Hz).

* **El Reto:** Determina la tensión requerida y la velocidad de propagación de la onda en la cuerda. Si el músico presiona el traste 5 (reduciendo la longitud vibrante en 1/4), ¿cuál es la nueva frecuencia?
* **Análisis Crítico:** ¿Por qué las cuerdas de charango se rompen con frecuencia en climas secos? Relaciona con los cambios de tensión por contracción térmica.
* **Simulación GeoGebra:** [Simulación de Cuerda Vibrante](https://www.geogebra.org/m/W7KdWvYv) - Observa los modos normales al variar la tensión.

---

### 🧠 Desafío 3
**La Flauta de Pan Andina**

Una flauta de pan tiene tubos abiertos de longitudes variables. El tubo más largo mide $L_1 = 40$ cm y el más corto $L_2 = 10$ cm, a temperatura de 25°C.

* **El Reto:** Calcula las frecuencias fundamentales de ambos tubos y el intervalo musical que forman. ¿Cuántos armónicos audibles (hasta 20 kHz) tiene cada tubo?
* **Toma de Decisión:** Un artesano quiere construir una flauta de pan pentatónica (5 notas). ¿Qué longitudes de tubos necesita para las notas Do ($262$ Hz), Re ($294$ Hz), Mi ($330$ Hz), Sol ($392$ Hz) y La ($440$ Hz)?
* **Simulación GeoGebra:** [Simulación de Tubos Sonoros](https://www.geogebra.org/m/XKfpRjQH) - Visualiza los modos de vibración en tubos abiertos.

---

### 🧠 Desafío 4
**El Sonar del Delfín**

Un delfín emite clics de ultrasonido con frecuencia $f = 120$ kHz en agua de mar ($v = 1530$ m/s). El eco de un pez retorna después de $\Delta t = 0.04$ s.

* **El Reto:** Calcula la longitud de onda del sonido en el agua, la distancia al pez, y la frecuencia del eco percibida si el pez se aleja a $v_p = 2$ m/s (efecto Doppler).
* **Análisis Técnico:** ¿Por qué los delfines usan frecuencias tan altas? Compara la resolución espacial (capacidad de distinguir dos objetos cercanos) con la de un sonar humano de 20 kHz.
* **Simulación GeoGebra:** [Simulación de Ecolocalización](https://www.geogebra.org/m/W7KdWvYv) - Modela la propagación y reflexión de la onda.

---

### 🧠 Desafío 5
**La Cuerda del Telégrafo**

En el siglo XIX, los cables telegráficos tendidos entre postes formaban una cuerda vibrante de longitud $L = 50$ m, tensión $F_T = 2000$ N y densidad lineal $\mu = 0.5$ kg/m. El viento excitaba oscilaciones.

* **El Reto:** Calcula la frecuencia fundamental del cable y las velocidades de los tres primeros modos normales. Si el viento sopla con frecuencia de 2 Hz, ¿qué modo excita resonantemente?
* **Análisis de Sensibilidad:** El cable se dilata con el calor solar (coeficiente $\alpha = 12 \times 10^{-6}$ /°C). ¿En cuánto cambia la frecuencia fundamental si la temperatura aumenta 20°C? ¿Es peligroso para la estabilidad del cable?
* **Simulación GeoGebra:** [Simulación de Cuerda con Tensión Variable](https://www.geogebra.org/m/XKfpRjQH) - Observa cómo cambian los modos al variar la tensión.

---

### 🧠 Desafío 6
**El Tubo de Kundt**

En un tubo de Kundt, un diapasón de $f = 2400$ Hz vibra en el extremo de un tubo cilíndrico con polvo de corcho en su interior. Se observa que el polvo se acumula en montículos separados 6.8 cm.

* **El Reto:** Calcula la velocidad del sonido en el gas del tubo y la longitud de onda. Si el tubo mide 80 cm, ¿cuántos nodos de desplazamiento hay? ¿Es un tubo abierto o cerrado?
* **Interpretación Profesional:** ¿Por qué este método histórico para medir la velocidad del sonido en gases es tan preciso? Compara con métodos modernos de tiempo de vuelo.
* **Simulación GeoGebra:** [Simulación de Ondas Estacionarias en Tubos](https://www.geogebra.org/m/W7KdWvYv) - Visualiza los nodos y vientres de presión y desplazamiento.

---

### 🧠 Desafío 7
**El Clarinete y el Flautín**

Un clarinete (tubo cerrado-abierto) de longitud $L_c = 66$ cm y un flautín (tubo abierto-abierto) de longitud $L_f = 32$ cm tocan a la misma temperatura.

* **El Reto:** Calcula las frecuencias fundamentales de ambos instrumentos y compara sus espectros de armónicos hasta el 6° armónico. ¿Qué armónicos tienen en común?
* **Análisis Crítico:** El clarinete se considera un instrumento "de caña" con timbre "oscuro". ¿Cómo explica la ausencia de armónicos pares esta característica sonora?
* **Simulación GeoGebra:** [Simulación de Espectros de Instrumentos](https://www.geogebra.org/m/XKfpRjQH) - Compara la serie armónica de tubos abiertos y cerrados.

---

### 🧠 Desafío 8
**La Red de Pesca Flotante**

Una red de pesca flota en el mar formando una cuadrícula. Las olas del mar tienen $\lambda = 2.5$ m y amplitud $A = 0.3$ m. Los flotadores están separados $d = 1.25$ m.

* **El Reto:** Calcula la frecuencia angular de las olas si su velocidad es $v = 4$ m/s. ¿Los flotadores oscilan en fase o en oposición de fase? Calcula la diferencia de fase entre flotadores adyacentes.
* **Evaluación:** Si la red tiene 20 flotadores en línea, ¿cuál es la diferencia de fase entre el primero y el último? ¿Bajo qué condición todos los flotadores se moverían en fase?
* **Simulación GeoGebra:** [Simulación de Ondas en Red Periódica](https://www.geogebra.org/m/W7KdWvYv) - Observa la propagación de fase a través de la cuadrícula.

---

### 🧠 Desafío 9
**El Martillo Neumático**

Un martillo neumático de construcción genera ondas sonoras con intensidad $I = 10^{-2}$ W/m² a 10 m de distancia. Un trabajador usa protectores auditivos que reducen el nivel en 25 dB.

* **El Reto:** Calcula el nivel de intensidad sin protección, el nivel con protección, y la intensidad resultante. ¿A qué distancia debería estar el trabajador para que el nivel con protección sea igual al umbral de dolor (120 dB sin protección)?
* **Toma de Decisión:** La normativa OSHA limita la exposición a 85 dB durante 8 horas. ¿Es seguro trabajar a 15 m del martillo durante una jornada completa? Propón medidas adicionales si es necesario.
* **Simulación GeoGebra:** [Simulación de Atenuación Sonora](https://www.geogebra.org/m/XKfpRjQH) - Modela la disminución de intensidad con la distancia.

---

### 🧠 Desafío 10
**La Cuerda de Teléfono de Dos Latas**

Dos niños comunican dos latas con una cuerda de nailon de $L = 15$ m, $\mu = 2.5$ g/m, tensada con $F_T = 30$ N. Un niño golpea su lata produciendo una perturbación.

* **El Reto:** Calcula la velocidad de propagación del pulso, el tiempo que tarda en llegar al otro extremo, y la forma del pulso reflejado si el otro niño mantiene su lata fija. ¿Y si la deja libre?
* **Extensión Creativa:** Diseña un "teléfono" que transmita el pulso en menos de 0.5 s usando el mismo material de cuerda. ¿Qué parámetros modificas y cómo afectan la atenuación del pulso?
* **Simulación GeoGebra:** [Simulación de Pulso en Cuerda](https://www.geogebra.org/m/W7KdWvYv) - Observa la propagación y reflexión del pulso en los extremos.

---
