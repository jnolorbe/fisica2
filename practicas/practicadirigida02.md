# Práctica 2: Esfuerzos Cortantes
**Curso:** Física 2 (EG-209)  
**Facultad:** Ingeniería Eléctrica y Electrónica - UNAC  
**Docente:** Juan Neil Mendoza Nolorbe  

---
## 1. El Desafío de la Conexión Asimétrica (Cizalla Simple)
En una inspección de campo, se detecta que una unión de pletinas de acero ha sido ensamblada de forma asimétrica (4 pernos en la sección superior y 2 en la inferior). Para entender el riesgo de colapso, analizamos el comportamiento del sistema bajo tracción.

* **Situación:** Los pernos son de acero estructural con un esfuerzo de fluencia $\tau_{f} = 250 \text{ MPa}$, los pernos de la sección superior tienen un diámetro de $0.5$ pulgadas y los de la sección inferior $1.0$ pulgada.
* **Reto A:** Demuestre mediante el análisis de esfuerzos ¿donde es más probable que ocurra la falla?
* **Reto B:** Calcule la carga máxima $P$ (en kN) que la unión puede soportar antes de que los pernos fallen catastróficamente.
* **Referencia Visual:** [Ver ensayo de laboratorio en YouTube](https://www.youtube.com/watch?v=is9DQOakQhs)

---

## 2. Optimización en el Proceso de Punzonado
Una prensa hidráulica en el taller de prototipado de la FIEE debe perforar placas de conexión. Se sabe que la placa tiene una resistencia a la cizalladura de $40 \text{ ksi}$ y el punzón de acero tiene un límite de compresión de $50 \text{ ksi}$.

* **Problema de Diseño:** Se requiere perforar agujeros de $2.5 \text{ in}$ de diámetro.
* **Pregunta Crítica:** ¿Cuál es el espesor máximo $t$ de la placa que se puede perforar sin que el punzón falle por compresión?
* **Análisis de Seguridad:** Si cambiamos a una placa de $0.25 \text{ in}$ de espesor, ¿cuál sería el diámetro del orificio más pequeño que podemos perforar de forma segura?

---
## 3. Transmisión de Potencia en Motores Eléctricos
Un eje de acero de $2 \text{ in}$ de diámetro se utiliza para transmitir potencia mecánica desde un motor a un generador. El eje gira a una velocidad constante de $240 \text{ rpm}$.

* **Restricción Técnico-Legal:** Por normas de seguridad industrial, la tensión de corte en el eje no debe exceder los $12 \text{ ksi}$.
* **Cálculo de Ingeniería:** Determine la potencia máxima en caballos de fuerza ($hp$) que puede transmitir el sistema.
* **Reflexión:** ¿Cómo afectaría a la potencia máxima si duplicamos la velocidad de rotación pero mantenemos el mismo esfuerzo de corte?

---
## 4. Análisis de Fallas en Mecanismos de Control (Palanca Acodada)
Un mecanismo de control de una subestación utiliza una palanca acodada (ver figura). La varilla $CD$ tiene un diámetro de $10 \text{ mm}$ y el pasador en $B$ tiene un diámetro de $6 \text{ mm}$.

:::{figure} https://github.com/jnolorbe/fisica2/blob/main/figuras/pd2_prob3.png
:width: 60%
:align: center
Figura 1. Palanca acodada
:::

* **Criterios de Falla:**
    * Esfuerzo de tracción admisible en la varilla ($CD$): $175 \text{ MPa}$.
    * Esfuerzo de cizalla admisible en el pasador ($B$): $60 \text{ MPa}$.
* **El Reto:** Determine la magnitud de la máxima fuerza vertical $P$ que puede aplicarse a la palanca sin que ninguno de los dos componentes falle. Identifique cuál es el componente que limita la carga (el "eslabón más débil").

---

## 5. Optimización de Sistemas de Transmisión por Engranajes
En el diseño de actuadores para seguidores solares, se utiliza un sistema de dos ejes conectados por engranajes para multiplicar el torque y orientar los paneles con precisión. En el sistema mostrado en la figura los cilindros estan hecho de una aleación de aluminio ($G = 27 \text{ GPa}$) para reducir el peso de la estructura. El torque de entrada en el extremo libre $E$ de **$T_E = 100 \text{ N}\cdot\text{m}$**. Los ejes $AD$ (con apoyo fijo en $D$) y $BE$ están conectados por engranajes en $C$. Se sabe que:

* La relación de radios de los engranajes es **$r_A = 3 \cdot r_B$**.
* Ambos ejes tienen la misma longitud **$L$**.
* Por normas de seguridad, el esfuerzo cortante en ningún punto de los ejes debe exceder los **$20 \text{ MPa}$**.

:::{figure} https://github.com/jnolorbe/fisica2/blob/main/figuras/pd2_prob5.png
:width: 50%
:align: center
Figura 2. Ejes Acoplados (Beer - Johnston - Dewolf - Mazurek. _Mechanic of Materials_)
:::

### A. Dimensionamiento Estructural
Determine el **diámetro mínimo $d$** (en mm) que deben tener ambos ejes (asumiendo que se fabricarán con el mismo diámetro) para que el sistema opere de forma segura. 
* *Pista de reflexión:* Antes de calcular, analice cuál de los dos ejes experimenta el mayor torque debido a la relación de engranajes.

### B. Análisis de Sensibilidad y Proporcionalidad
Si por requerimientos de espacio la longitud $L$ de los ejes debe duplicarse:
1. ¿Cómo se ve afectado el esfuerzo cortante máximo en los ejes? Justifique su respuesta basándose en la relación: $\tau_{máx} = \frac{16T}{\pi d^3}$.
2. ¿Cómo varía el ángulo de giro total en el extremo $E$ respecto al apoyo $D$? Utilice la relación de proporcionalidad $\phi \propto \frac{TL}{d^4}$ para su explicación.

### C. Aumentación Cognitiva (Uso de IA)
Utilice una herramienta de Inteligencia Artificial para resolver la siguiente interrogante y adjunte su análisis crítico:
> *"Si mantengo el mismo material y longitud, pero el eje A tiene el doble de diámetro que el eje B, ¿cuánto torque adicional puede soportar el eje A para mantener exactamente el mismo ángulo de giro ($\phi$) que el eje B?"*

**Instrucción:** Compare el factor de escala proporcionado por la IA con su deducción matemática a partir de la fórmula directa del ángulo de giro.


## 6. Análisis de Potencia y Esfuerzos en Sistemas de Transmisión

En una planta de procesamiento, un motor eléctrico está acoplado a un sistema de ejes mediante engranajes para accionar una carga pesada. Para fines de mantenimiento, el motor en el punto **A** mantiene el eje fijo (bloqueado) mientras se aplica un torque de prueba en el extremo del segundo eje. Este análisis es vital para asegurar que, al encender el motor a su potencia nominal, los ejes no fallen por fatiga o cizalladura súbita. Considere el sistema de la figura, compuesto por dos ejes de acero macizo con las siguientes especificaciones:

* **Eje AB:** Diámetro $d_{AB} = 30\text{ mm}$.
* **Eje CD:** Diámetro $d_{CD} = 35\text{ mm}$.
* **Engranajes:** El radio del engranaje $E$ es $r_E = 50\text{ mm}$ y el del engranaje $F$ es $r_F = 125\text{ mm}$.
* **Carga de Prueba:** Se aplica un torque $T' = 75\text{ N}\cdot\text{m}$ en el eje $CD$.

:::{figure} https://github.com/jnolorbe/fisica2/blob/main/figuras/pd2_prob6.png
:width: 60%
:align: center
Figura 3. Sistema de Transmisión 
:::

### Retos de Análisis:

1.  **Cálculo de Esfuerzos Críticos:** Determine el esfuerzo cortante máximo absoluto ($\tau_{máx}$) en cada uno de los ejes. 
    
    _Pista: Primero debe determinar cómo se transmite el torque de un eje a otro a través de la relación de radios de los engranajes._

2.  **Dimensionamiento de Potencia:** Suponga que el motor en **A** se libera y opera a una velocidad constante de **$1750\text{ rpm}$** entregando el torque necesario para equilibrar la carga $T'$. Calcule la potencia máxima (en **kW**) que el motor está transmitiendo al sistema.
    *Dato: $1\text{ hp} = 0.746\text{ kW}$. Use la relación $P = T \cdot \omega$.*

3.  **Evaluación de Integridad:** Si el material de ambos ejes tiene un esfuerzo de fluencia por cizalla de $120\text{ MPa}$, ¿cuál de los dos ejes presenta un menor factor de seguridad bajo estas condiciones de operación? Justifique su respuesta técnica.

4. **Aumentación Cognitiva (Uso de IA)**
Para validar su análisis, consulte a una IA con el siguiente *prompt*: *"Tengo un sistema de dos ejes acoplados por engranajes donde el eje conductor tiene un diámetro menor que el eje conducido, pero el torque se multiplica en el segundo eje. ¿Es posible que el esfuerzo cortante sea mayor en el eje que tiene menor torque? Explica la relación entre el diámetro al cubo ($d^3$) y la transmisión de torque ($T$) en la falla por cizalla."*

**Instrucción:** Compare la explicación de la IA con sus resultados numéricos. ¿El aumento del diámetro en el eje $CD$ compensa el aumento del torque transmitido?

---
### Instrucciones para el Portafolio
1.  **Resolución:** Los problemas deben resolverse priorizando el análisis físico y los diagramas de cuerpo libre (DCL).
2.  **Uso de IA:** Se permite el uso de IA para verificar resultados, pero se debe adjuntar el "Prompt" utilizado y una crítica personal a la respuesta entregada por la IA.
3.  **Metacognición:** Al final de su práctica, responda: *¿Cuál fue el concepto físico más difícil de visualizar en estos problemas y cómo logró superarlo?*

---
*Material para uso exclusivo de los estudiantes de Física 2 - FIEE UNAC 2026.*