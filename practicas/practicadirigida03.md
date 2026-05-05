# Práctica 3: Oscilaciones Libres, Amortiguadas y Forzadas

**Curso:** Física 2 (EG-209)  
**Facultad:** Ingeniería Eléctrica y Electrónica - UNAC  
**Docente:** Juan Neil Mendoza Nolorbe  

---

## 1. El Dilema del Soporte Antivibratorio (Oscilaciones Libres)
Un equipo de ingenieros de la FIEE está diseñando un soporte para un equipo de medición sensible. El sistema se modela como un cuerpo de $2.0 \text{ kg}$ unido a un resorte horizontal de constante $k = 5.0 \text{ kN/m}$. Para probar su respuesta, el resorte se alarga $10.0 \text{ cm}$ y se deja libre desde el reposo.

* **Reto A:** Determine la frecuencia ($f$) y el período ($T$) del movimiento. ¿Qué tan rápido debe ser el sistema de adquisición de datos para capturar el pico de aceleración máxima?
* **Reto B:** Calcule el tiempo que tarda el cuerpo en alcanzar por primera vez su posición de equilibrio y demuestre analíticamente el valor de su velocidad en ese instante.
* **Situación de Análisis:** Si el sistema se suspendiera verticalmente, ¿en cuánto cambiaría la posición de equilibrio respecto a la longitud natural del resorte? (Considere $g = \pi^2 \text{ m/s}^2$).

---

## 2. Monitoreo de Integridad en Ejes Rotativos
En un generador eléctrico, una partícula en la periferia de un componente circular de $40.0 \text{ cm}$ de radio se mueve con una rapidez constante de $80.0 \text{ cm/s}$. Su proyección sobre el eje $X$ realiza un Movimiento Armónico Simple (MAS).

* **Problema de Modelamiento:** Escriba la ecuación de la posición $x(t)$ para la proyección de esta partícula, asumiendo que en $t = 0 \text{ s}$ se encuentra en el origen ($x = 0$).
* **Análisis de Energía:** Si la masa asociada a esta oscilación fuera de $3.0 \text{ kg}$, calcule la energía total del sistema. ¿En qué posición la energía cinética es exactamente igual a la energía potencial elástica?

---

## 3. Estabilidad en el Transporte de Componentes
Un bloque de masa $M$ se desliza sobre una superficie horizontal lisa sujeto a un resorte, oscilando con un período de $0.80 \text{ s}$. Un segundo bloque de masa $m$ descansa sobre el primero. El coeficiente de fricción estática entre ambos es $\mu_s = 0.25$.

* **Pregunta Crítica:** Si la amplitud de oscilación es de $1.0 \text{ cm}$, ¿deslizará el bloque superior? Justifique su respuesta comparando la aceleración máxima del sistema con la aceleración crítica de fricción.
* **Diseño de Seguridad:** Determine la amplitud máxima permitida para que el bloque superior se mantenga solidario al inferior sin deslizar. (Considere $g = 2\pi^2 \text{ m/s}^2$ para simplificar cálculos).

---

## 4. El Oscilador en el Mundo Real (Amortiguamiento Viscoso)
Un objeto de $0.4 \text{ kg}$ se conecta a un resorte de $k = 1000 \text{ N/m}$. El sistema se sumerge en un líquido viscoso con un coeficiente de amortiguamiento $b = 5.6 \text{ kg/s}$. El objeto se desplaza $10 \text{ cm}$ y se suelta.

* **Análisis del Sistema:** Determine si el sistema es subamortiguado, críticamente amortiguado o sobreamortiguado calculando el parámetro de amortiguamiento $\gamma = \frac{b}{2m}$ y la frecuencia natural $\omega_0$.
* **Reto de Ingeniería:** Escriba la ecuación de la posición $x(t)$ y calcule el "Tiempo de Extinción", definido como el tiempo necesario para que la amplitud se reduzca al $36.8\%$ ($e^{-1}$) de su valor inicial.

---

## 5. Resonancia en Sistemas Electromecánicos
Un sistema de transmisión consiste en una masa $M$ conectada a un resorte de constante $k$, la cual es impulsada por una fuerza externa $F(t) = F_0 \cos(\omega t)$.

* **El Fenómeno:** Si el sistema presenta el amortiguamiento del problema anterior, determine la frecuencia de resonancia $\omega_R$