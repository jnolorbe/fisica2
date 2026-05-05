# Práctica 6: Hidrodinámica I

**Curso:** Física 2 (EG-209)  
**Facultad:** Ingeniería Eléctrica y Electrónica - UNAC  
**Docente:** Juan Neil Mendoza Nolorbe  

---
Resuelve los siguientes 10 desafíos siguiendo el **Formato de 5-Bloques**. Para el Portafolio digital presenta **4 Desafíos** de tu elección.
---

### 🧠 Desafío 1: El Acueducto de Cumbe Mayo

El acueducto preinca de Cumbe Mayo (Cajamarca, ~1500 a.C.) transporta agua a través de un canal de piedra con pendiente mínima. En un tramo, el canal tiene sección rectangular de $w = 1.2$ m de ancho y agua fluyendo a $h = 0.4$ m de profundidad con velocidad $v = 0.8$ m/s.

* **El Reto:** Calcula el caudal volumétrico, la velocidad si el canal se estrecha a $w = 0.8$ m manteniendo la misma profundidad, y la diferencia de presión entre ambas secciones si el canal es horizontal.
* **Interpretación:** ¿Cómo lograron los constructores preincas mantener el flujo constante sin conocer la ecuación de Bernoulli? Relaciona con el principio de nivelación por pendiente constante.
* **Simulación GeoGebra:** [Simulación de Flujo en Canales Abiertos](https://www.geogebra.org/m/XKfpRjQH) - Visualiza la conservación de caudal en estrechamientos.

---

### 🧠 Desafío 2: El Inyector de Riego por Aspersión

Un sistema de riego usa inyectores Venturi para mezclar fertilizante líquido. El agua entra al inyector a $P_1 = 300$ kPa y $v_1 = 2$ m/s. La garganta del Venturi tiene la mitad del diámetro de entrada.

* **El Reto:** Calcula la presión en la garganta, el caudal de agua si el diámetro de entrada es 2.5 cm, y la altura a la que puede succionar el fertilizante ($\rho = 1200$ kg/m³) desde un depósito abierto.
* **Análisis Crítico:** Si el fertilizante es más denso que el agua, ¿aumenta o disminuye la altura de succión respecto a usar agua pura? Justifica con la ecuación de Bernoulli.
* **Simulación GeoGebra:** [Simulación de Inyector Venturi](https://www.geogebra.org/m/W7KdWvYv) - Ajusta la relación de áreas y observa la succión generada.

---

### 🧠 Desafío 3: El Velocímetro del Avión de Línea

Un Boeing 737 vuela a 9000 m de altitud donde $\rho_{aire} = 0.47$ kg/m³. El tubo de Pitot mide $P_{total} = 32.5$ kPa y la presión estática ambiente es $P_{est} = 30.8$ kPa.

* **El Reto:** Calcula la velocidad del avión respecto al aire en km/h, el número de Mach si la velocidad del sonido a esa altitud es 325 m/s, y la lectura equivalente que mostraría el Pitot en Lima a nivel del mar con la misma velocidad.
* **Toma de Decisión:** Si el Pitot se congela parcialmente, reduciendo la lectura de $P_{total}$ en un 15%, ¿qué velocidad indicaría erróneamente el instrumento? ¿Es peligrosa esta lectura subestimada?
* **Simulación GeoGebra:** [Simulación de Tubo de Pitot](https://www.geogebra.org/m/XKfpRjQH) - Modela la relación entre velocidad y presión de estancamiento.

---

### 🧠 Desafío 4: El Tanque de Agua de la Olla de Moyobamba

Un tanque cilíndrico de $D = 2$ m y $H = 3$ m alimenta un sistema de agua potable en Moyobamba. Tiene dos orificios de drenaje: uno inferior de $d_1 = 3$ cm y uno lateral a 1 m del fondo de $d_2 = 2$ cm.

* **El Reto:** Calcula el tiempo de vaciado por cada orificio por separado, el tiempo si ambos abren simultáneamente, y la altura del chorro del orificio lateral medida desde el nivel del suelo (el tanque está sobre una torre de 8 m).
* **Análisis de Sensibilidad:** Durante la estación seca, la temperatura del agua sube de 20°C a 28°C. ¿Cómo afecta esto al tiempo de vaciado? Considera la variación de viscosidad y densidad.
* **Simulación GeoGebra:** [Simulación de Vaciado de Tanque](https://www.geogebra.org/m/W7KdWvYv) - Observa la variación de velocidad y caudal con el nivel descendiente.

---

### 🧠 Desafío 5: La Manguera de los Bomberos

Una manguera de bomberos tiene diámetro $D_1 = 10$ cm en la sección de suministro desde el camión. La boquilla de salida tiene $D_2 = 2.5$ cm. El agua sale a $v_2 = 25$ m/s.

* **El Reto:** Calcula la velocidad en la manguera de suministro, la presión manométrica requerida en el camión (asumiendo altura constante), y la altura máxima a la que puede llegar el chorro vertical.
* **Toma de Decisión:** Para incendios en edificios altos, ¿es más efectivo aumentar la presión en la bomba o reducir el diámetro de la boquilla? Compara ambas estrategias usando Bernoulli.
* **Simulación GeoGebra:** [Simulación de Chorro de Manguera](https://www.geogebra.org/m/XKfpRjQH) - Visualiza la conversión de presión en velocidad.

---

### 🧠 Desafío 6: El Medidor de Gas Doméstico

Un medidor de gas natural usa un diafragma que se desplaza por diferencia de presión. El gas fluye por un tubo de $D = 2$ cm con velocidad $v = 3$ m/s a $P = 2.5$ kPa manométrica y $\rho = 0.7$ kg/m³.

* **El Reto:** Calcula el caudal volumétrico y másico, la presión dinámica, y la presión total en la tubería. Si el medidor introduce una restricción que reduce la sección a la mitad, ¿cuál es la nueva presión a la salida?
* **Interpretación Profesional:** ¿Por qué los medidores de gas miden volumen a condiciones estándar (0°C, 1 atm) en lugar de volumen real? Explica la corrección por temperatura y presión.
* **Simulación GeoGebra:** [Simulación de Medidor de Flujo](https://www.geogebra.org/m/W7KdWvYv) - Modela la caída de presión en restricciones.

---

### 🧠 Desafío 7: El Sifón de la Fuente de la Plaza de Armas

La fuente central de la Plaza de Armas de Lima usa un sifón oculto para recircular agua desde un reservorio inferior hasta una copa decorativa a 3 m de altura. El tubo tiene $D = 5$ cm.

* **El Reto:** Calcula la velocidad mínima de salida necesaria para que el sifón funcione, el caudal correspondiente, y la presión en la cima del sifón. Verifica si es mayor que la presión de vapor del agua a 20°C.
* **Análisis Crítico:** Si la temperatura del agua sube a 35°C en verano ($P_{vapor} = 5.6$ kPa), ¿se mantiene estable el sifón? ¿Qué altura máxima podría tener en esas condiciones?
* **Simulación GeoGebra:** [Simulación de Sifón Hidráulico](https://www.geogebra.org/m/XKfpRjQH) - Observa el límite de altura por presión de vapor.

---

### 🧠 Desafío 8: La Tubería del Oleoducto Norperuano

El oleoducto norperuano transporta petróleo ($\rho = 850$ kg/m³, $\mu = 0.25$ Pa·s) a través de una tubería de $D = 50$ cm. En un tramo horizontal, la presión cae de $P_1 = 4$ MPa a $P_2 = 3.5$ MPa en $L = 10$ km.

* **El Reto:** Aplica Bernoulli ideal para estimar la velocidad del flujo. Luego calcula el número de Reynolds ($Re = \frac{\rho v D}{\mu}$) y determina si el flujo es laminar ($Re < 2000$) o turbulento.
* **Evaluación:** Bernoulli ideal predice velocidad constante en tubería horizontal con igual diámetro, pero la presión cae. ¿De dónde proviene esta "pérdida" de energía? Introduce el concepto de pérdida por fricción.
* **Simulación GeoGebra:** [Simulación de Flujo en Tuberías](https://www.geogebra.org/m/W7KdWvYv) - Compara flujo laminar y turbulento.

---

### 🧠 Desafío 9: El Pulverizador Agrícola de la Chacra

Un pulverizador de mochila usa una boquilla Venturi conectada a una manguera de presión. El líquido insecticida ($\rho = 1050$ kg/m³) debe mezclarse con aire a $v_{aire} = 15$ m/s en una garganta de $A_2 = 0.3$ cm².

* **El Reto:** Calcula la presión en la garganta si la sección de entrada es $A_1 = 1.2$ cm² y la presión atmosférica es 100 kPa. ¿Puede succionar el insecticida desde un depósito a 30 cm debajo de la boquilla?
* **Extensión Creativa:** Diseña una boquilla mejorada que permita succionar desde 50 cm de profundidad manteniendo la misma velocidad de aire. ¿Qué parámetros modificas y cuáles son las limitaciones prácticas?
* **Simulación GeoGebra:** [Simulación de Pulverizador Venturi](https://www.geogebra.org/m/XKfpRjQH) - Optimiza la geometría para máxima succión.

---

### 🧠 Desafío 10: El Reloj de Agua del Museo Larco

Un reloj de agua (clepsidra) del Museo Larco tiene forma cónica invertida: radio superior $R = 10$ cm, radio inferior $r = 2$ cm, altura $H = 30$ cm. El agua sale por un orificio de 3 mm de diámetro en la base.

* **El Reto:** Deriva la expresión del tiempo de vaciado para geometría cónica (el área del tanque varía con la altura). Calcula el tiempo de vaciado completo y compárelo con un cilindro de igual altura y volumen.
* **Análisis de Sensibilidad:** Los relojes de agua antiguos usaban flotadores para mantener nivel constante. ¿Cuánto se adelantaría o atrasaría este reloj en 1 hora si la temperatura del agua varía de 15°C a 25°C?
* **Simulación GeoGebra:** [Simulación de Clepsidra](https://www.geogebra.org/m/W7KdWvYv) - Modela el vaciado de recipientes con geometría variable.
