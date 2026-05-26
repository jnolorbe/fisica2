# Sesión 7: Hidrodinámica II 
## Fluidos Reales y Viscosidad

## 📌 I. Fundamento Teórico

En la sesión anterior analizamos el comportamiento de los fluidos ideales bajo la hipótesis simplificadora de la ausencia de pérdidas energéticas. En esta sesión estudiaremos los fluidos reales, donde las fuerzas de fricción interna o disipativas —denominadas viscosidad— juegan un rol fundamental en la dinámica del flujo. Utilizaremos herramientas de cálculo diferencial e integral para describir matemáticamente estas fuerzas y modelar cómo afectan el transporte de fluidos en tuberías y el movimiento de cuerpos sólidos dentro de ellos.

### 1.1. Viscosidad y la Ley de Newton de la Viscosidad

La viscosidad ($\eta$) es una medida de la resistencia de un fluido a sufrir deformaciones graduales causadas por esfuerzos cortantes o tangenciales. A nivel molecular, surge debido a las fuerzas de cohesión intermoleculares y al intercambio de momento lineal entre las capas de fluido que se desplazan a diferentes velocidades.

Formulación Diferencial de la Ley de Newton

Consideremos un fluido confinado entre dos placas paralelas infinitas de área $A$, separadas por una distancia infinitesimal $dy$. Si la placa superior se desplaza a una velocidad $v + dv$ y la inferior a una velocidad $v$, se establece un perfil de velocidades en el fluido.

Para un fluido newtoniano, el esfuerzo cortante ($\tau$) es directamente proporcional al gradiente de velocidad tangencial:

$$\tau = \frac{F_v}{A} = \eta \frac{dv}{dy}$$

Donde:

$\tau$: Esfuerzo cortante ($\text{N/m}^2$ o $\text{Pa}$).

$F_v$: Fuerza viscosa tangencial ($\text{N}$).

$\eta$: Coeficiente de viscosidad dinámica (o absoluta). En el S.I. se mide en $\text{Pa}\cdot\text{s}$ ($\text{kg}/(\text{m}\cdot\text{s})$). En el sistema CGS se utiliza el Poise ($\text{P}$), donde $1\text{ Pa}\cdot\text{s} = 10\text{ P} = 1000\text{ cP}$ (centipoise).

$\frac{dv}{dy}$: Gradiente de velocidad o tasa de deformación por corte ($\text{s}^{-1}$).

💡 Regla de Oro: La viscosidad de los líquidos disminuye con la temperatura debido al debilitamiento de los enlaces intermoleculares. Por el contrario, la viscosidad de los gases aumenta con la temperatura, ya que la agitación térmica incrementa la tasa de colisiones y la transferencia de momento entre sus moléculas.

### 1.2. Regímenes de Flujo y el Número de Reynolds

El comportamiento dinámico de un fluido real dentro de un conducto depende de la relación entre sus fuerzas de inercia y sus fuerzas viscosas. Esta relación se cuantifica mediante el parámetro adimensional conocido como el Número de Reynolds ($Re$):

$$Re = \frac{\rho v_m D}{\eta}$$

Donde:

$\rho$: Densidad del fluido ($\text{kg/m}^3$).

$v_m$: Velocidad media del flujo en la sección transversal ($\text{m/s}$).

$D$: Diámetro característico de la tubería ($\text{m}$).

$\eta$: Viscosidad dinámica del fluido ($\text{Pa}\cdot\text{s}$).

Regímenes de Flujo en Tuberías:

Flujo Laminar ($Re < 2300$): El fluido se mueve en capas paralelas (láminas) bien definidas que se deslizan suavemente una sobre otra sin mezclarse macroscópicamente. Las fuerzas viscosas dominan el movimiento, amortiguando cualquier perturbación.

Zona de Transición ($2300 \le Re \le 4000$): El flujo es inestable y puede alternar de manera caótica entre laminar y turbulento debido a ligeras perturbaciones en el conducto.

Flujo Turbulento ($Re > 4000$): Las fuerzas de inercia dominan sobre las viscosas. Las partículas del fluido se mueven siguiendo trayectorias altamente desordenadas, caracterizadas por la formación de vórtices, remolinos y una mezcla tridimensional intensa.

### 1.3. Distribución de Velocidades en una Tubería Cilíndrica (Perfil Parabólico)

Cuando un fluido viscoso fluye en régimen laminar a través de una tubería circular de radio interno $R$ y longitud $L$, la capa de fluido en contacto directo con la pared se adhiere a ella debido a las fuerzas de fricción superficial, cumpliendo la condición de no deslizamiento ($v = 0$ en $r = R$).

A partir de un balance de fuerzas sobre un elemento cilíndrico de fluido de radio $r$ y longitud diferencial $dx$, sometido a una caída de presión $\Delta P = P_1 - P_2$:

$$\Delta P \cdot (\pi r^2) = \tau \cdot (2\pi r L)$$

Sustituyendo la ley de Newton de la viscosidad en coordenadas cilíndricas ($\tau = -\eta \frac{dv}{dr}$, donde el signo negativo denota que la velocidad disminuye al alejarse del centro):

$$-\eta \frac{dv}{dr} = \frac{r \Delta P}{2L}$$

Integrando con respecto a $r$ bajo la condición de frontera $v(R) = 0$:

$$v(r) = \frac{\Delta P}{4\eta L} \left(R^2 - r^2\right)$$

Esta ecuación describe un perfil parabólico de velocidades. La velocidad máxima ($v_{\text{máx}}$) ocurre en el eje central del conducto ($r = 0$):

$$v_{\text{máx}} = \frac{\Delta P R^2}{4\eta L}$$

### 1.4. Caudal Volumétrico: Ley de Hagen-Poiseuille

Para determinar el volumen de fluido que atraviesa la sección transversal por unidad de tiempo (caudal $Q$), integramos el perfil de velocidades sobre anillos concéntricos diferenciales de área $dA = 2\pi r \, dr$:

$$Q = \int_{0}^{R} v(r) (2\pi r \, dr) = \int_{0}^{R} \frac{\Delta P}{4\eta L} \left(R^2 - r^2\right) (2\pi r \, dr)$$

Al resolver esta integral definida, obtenemos la Ley de Hagen-Poiseuille:

$$Q = \frac{\pi R^4 \Delta P}{8 \eta L} = \frac{\pi D^4 \Delta P}{128 \eta L}$$

⚡ Analogía Eléctrica (La Ley de Ohm Hidráulica)

Para los estudiantes de Ingeniería Eléctrica y Electrónica, esta relación posee una equivalencia matemática directa con la teoría de circuitos. Podemos reescribir la Ley de Hagen-Poiseuille como:

$$\Delta P = Q \cdot R_H$$

Donde:

$\Delta P$ (Diferencia de presiones) es el análogo de la Tensión o Voltaje ($V$).

$Q$ (Caudal de flujo) es el análogo de la Corriente eléctrica ($I$).

$R_H = \frac{8 \eta L}{\pi R^4}$ es la Resistencia Hidráulica, análoga a la Resistencia Eléctrica ($R = \rho_e \frac{L}{A}$). Nótese que $R_H$ depende fuertemente de la geometría del conducto (inversamente proporcional a $R^4$).

### 1.5. Dinámica de Cuerpos en Medios Viscosos: Ley de Stokes

Cuando un cuerpo sólido se desplaza a través de un fluido viscoso, experimenta una fuerza de arrastre debida al rozamiento viscoso superficial y a la diferencia de presiones inducida por el movimiento. Para una esfera de radio $R$ que se mueve a una velocidad baja (régimen estrictamente laminar, $Re_{\text{esfera}} < 1$), Sir George Stokes dedujo la fuerza de resistencia hidrodinámica:

$$F_D = 6\pi \eta R v$$

Ecuación de Movimiento y Velocidad Terminal

Si dejamos caer una esfera de densidad $\rho_s$ y radio $R$ dentro de un fluido viscoso de densidad $\rho_f$, las fuerzas que actúan sobre ella son: el peso ($W$), el empuje de Arquímedes ($E$) y la fuerza de arrastre de Stokes ($F_D$).

Aplicando la segunda ley de Newton en el eje vertical:

$$\Sigma F_y = m \frac{dv}{dt} \implies W - E - F_D = m \frac{dv}{dt}$$

Expresando la masa y el volumen en términos de la geometría esférica:

$$\rho_s \left(\frac{4}{3}\pi R^3\right) g - \rho_f \left(\frac{4}{3}\pi R^3\right) g - 6\pi \eta R v = \rho_s \left(\frac{4}{3}\pi R^3\right) \frac{dv}{dt}$$

A medida que el cuerpo acelera, la fuerza de arrastre aumenta hasta equilibrar perfectamente las fuerzas gravitacionales y de flotación. En ese instante, la aceleración se anula ($\frac{dv}{dt} = 0$), y la esfera alcanza una velocidad constante llamada velocidad terminal o límite ($v_L$):

$$v_L = \frac{2 R^2 g (\rho_s - \rho_f)}{9\eta}$$

## 🚀 II. Problemas Resueltos

🧩 Problema N° 1

```{admonition} Perfil de velocidad
:class: important
Un fluido newtoniano de viscosidad constante $\eta$ fluye por gravedad en régimen laminar descendiendo por una pared vertical plana, formando una película delgada de espesor constante $h$. El aire adyacente no ejerce esfuerzo cortante sobre la superficie libre del fluido ($\tau = 0$ en $y = h$). Determine de forma analítica el perfil de velocidades $v_z(y)$ y calcule el caudal por unidad de ancho del plano utilizando integración directa.
```

```:class: dropdown hint
**1. Planteamiento:**
Establecemos un sistema de coordenadas donde el eje $z$ apunta verticalmente hacia abajo (dirección del flujo) y el eje $y$ es perpendicular a la pared ($y = 0$ en la pared, $y = h$ en la superficie libre del fluido).

Para una porción de fluido de longitud $L$, ancho $W$ (perpendicular al plano) y espesor $dy$ localizado a una distancia $y$:
Las fuerzas que actúan sobre este elemento de volumen en equilibrio dinámico son:
* La fuerza viscosa neta debida al gradiente de esfuerzos: $dF_v = W L \cdot [\tau(y+dy) - \tau(y)] = W L \frac{d\tau}{dy} dy$.
* La componente del peso propio del elemento de volumen: $dW = \rho g (W L dy)$.

**2. Resolución:**
Para un flujo estacionario no acelerado, la suma de fuerzas en la dirección $z$ debe ser cero:

$$\Sigma F_z = 0 \implies \frac{d\tau}{dy} W L \, dy + \rho g W L \, dy = 0 \implies \frac{d\tau}{dy} = -\rho g$$

Integrando con respecto a $y$:
$$\tau(y) = -\rho g y + C_1$$

Aplicamos la condición de frontera en la superficie libre: en $y = h$, el esfuerzo de cizalla con el aire es nulo ($\tau(h) = 0$):
$$0 = -\rho g h + C_1 \implies C_1 = \rho g h$$
$$\tau(y) = \rho g (h - y)$$

Sustituimos la Ley de Newton de la Viscosidad ($\tau = \eta \frac{dv_z}{dy}$):
$$\eta \frac{dv_z}{dy} = \rho g (h - y) \implies \frac{dv_z}{dy} = \frac{\rho g}{\eta} (h - y)$$

Volvemos a integrar con respecto a $y$ para obtener la velocidad:
$$v_z(y) = \frac{\rho g}{\eta} \left( h y - \frac{y^2}{2} \right) + C_2$$

Aplicamos la condición de no deslizamiento en la pared fija: en $y = 0$, $v_z(0) = 0 \implies C_2 = 0$.
Por lo tanto, el perfil de velocidades es:
$$v_z(y) = \frac{\rho g}{2\eta} (2h y - y^2)$$

Para calcular el caudal por unidad de ancho ($q = Q/W$), integramos la velocidad a través de todo el espesor de la película:
$$q = \int_{0}^{h} v_z(y) \, dy = \int_{0}^{h} \frac{\rho g}{2\eta} (2h y - y^2) \, dy$$
$$q = \frac{\rho g}{2\eta} \left[ h y^2 - \frac{y^3}{3} \right]_{0}^{h} = \frac{\rho g}{2\eta} \left( h^3 - \frac{h^3}{3} \right) = \frac{\rho g h^3}{3\eta}$$

**3. Discusión Crítica:**
El perfil de velocidades es parabólico, alcanzando su valor máximo en la superficie libre del fluido ($y = h$). El caudal por unidad de ancho es proporcional al cubo del espesor de la película ($h^3$). Esto muestra la altísima sensibilidad del flujo de películas delgadas ante variaciones del espesor, un concepto crucial en procesos de recubrimiento y refrigeración líquida de componentes eléctricos.


🧩 Problema N° 2

```{admonition} Pérdida de Carga y Caída de Presión en Conductos FIEE
:class: important
Un transformador de potencia de la subestación eléctrica de la UNAC utiliza aceite dieléctrico ligero a $20^\circ\text{C}$ ($\rho = 880\text{ kg/m}^3$, $\eta = 0.024\text{ Pa}\cdot\text{s}$) para disipar el calor generado en las bobinas. El aceite se bombea a través de un ducto cilíndrico de cobre de $12\text{ mm}$ de diámetro interno y $8\text{ m}$ de longitud. Si el caudal requerido para la refrigeración óptima es de $0.15\text{ L/s}$:

- Determine rigurosamente el régimen del flujo de aceite.

- Calcule la caída de presión en el ducto debido a pérdidas por fricción viscosa.

- Determine la potencia eléctrica que debe consumir el motor de la bomba (con eficiencia del $100\%$) para mantener este flujo de refrigeración.
```
```
:class: dropdown hint
**1. Planteamiento:**
* Convertimos las unidades al S.I.:
  * Caudal: $Q = 0.15\text{ L/s} = 0.15 \times 10^{-3}\text{ m}^3\text{/s} = 1.5 \times 10^{-4}\text{ m}^3\text{/s}$.
  * Diámetro: $D = 12\text{ mm} = 0.012\text{ m}$ (Radio $R = 6 \times 10^{-3}\text{ m}$).
* Calculamos primero la velocidad media ($v_m$) para evaluar el Número de Reynolds ($Re$) y definir el régimen de flujo.
* Si el flujo es laminar ($Re < 2300$), aplicaremos la ley de Hagen-Poiseuille para hallar la pérdida de presión ($\Delta P$).
* La potencia hidráulica de bombeo requerida se calcula como $P_{\text{bomba}} = Q \cdot \Delta P$.

**2. Resolución:**
*Área de la sección transversal de la tubería:*
$$A = \pi R^2 = \pi (6 \times 10^{-3}\text{ m})^2 \approx 1.131 \times 10^{-4}\text{ m}^2$$

*Velocidad media:*
$$v_m = \frac{Q}{A} = \frac{1.5 \times 10^{-4}\text{ m}^3\text{/s}}{1.131 \times 10^{-4}\text{ m}^2} \approx 1.326\text{ m/s}$$

*Cálculo del Número de Reynolds:*
$$Re = \frac{\rho v_m D}{\eta} = \frac{880\text{ kg/m}^3 \cdot 1.326\text{ m/s} \cdot 0.012\text{ m}}{0.024\text{ Pa}\cdot\text{s}} = \frac{14.00}{0.024} \approx 583.4$$

Como $Re = 583.4 < 2300$, **el flujo es estrictamente laminar**, lo cual valida la aplicación directa de la Ley de Hagen-Poiseuille.

*Cálculo de la caída de presión ($\Delta P$):*
$$\Delta P = \frac{8 \eta L Q}{\pi R^4} = \frac{8 \cdot (0.024\text{ Pa}\cdot\text{s}) \cdot 8\text{ m} \cdot (1.5 \times 10^{-4}\text{ m}^3\text{/s})}{\pi \cdot (6 \times 10^{-3}\text{ m})^4}$$
$$\Delta P = \frac{2.304 \times 10^{-4}}{3.1416 \cdot (1.296 \times 10^{-9})} = \frac{2.304 \times 10^{-4}}{4.0715 \times 10^{-9}} \approx 56588.5\text{ Pa} \approx 56.6\text{ kPa}$$

*Cálculo de la potencia eléctrica requerida para el bombeo:*
$$P_{\text{bomba}} = Q \cdot \Delta P = (1.5 \times 10^{-4}\text{ m}^3\text{/s}) \cdot (56588.5\text{ Pa}) \approx 8.49\text{ W}$$

**3. Discusión Crítica:**
La baja potencia de bombeo teórica ($8.49\text{ W}$) se debe a que el flujo opera en un régimen laminar muy estable. Sin embargo, si el transformador opera en climas muy fríos de la sierra peruana donde la temperatura del aceite baje a $0^\circ\text{C}$, su viscosidad podría cuadruplicarse, exigiendo cuatro veces más potencia de bombeo para el mismo caudal. Esto destaca la importancia de considerar variaciones térmicas de la viscosidad en diseños de ingeniería eléctrica.


🧩 Problema N° 3

```{admonition} Dinámica Transitoria de una Partícula Viscosa
:class: important
Una microesfera conductora de silicio ($\rho_s = 2330\text{ kg/m}^3$) de radio $R = 100\ \mu\text{m}$ se suelta desde el reposo en un canal aislante lleno de aceite dieléctrico ($\rho_f = 920\text{ kg/m}^3$, $\eta = 0.15\text{ Pa}\cdot\text{s}$).

- Deduzca analíticamente la ecuación de la velocidad en función del tiempo $v(t)$ resolviendo la ecuación diferencial del movimiento.

- Determine la velocidad límite de la esfera.

- Encuentre el tiempo característico $\tau_c$ en el cual la esfera alcanza el $63.2\%$ de su velocidad límite.
````

```:class: dropdown hint
**1. Planteamiento:**
Escribimos la segunda ley de Newton para la esfera que desciende verticalmente en el líquido viscoso:

$$m \frac{dv}{dt} = W - E - F_D \implies \rho_s V_s \frac{dv}{dt} = (\rho_s - \rho_f) V_s g - 6\pi\eta R v$$

Donde el volumen de la esfera es $V_s = \frac{4}{3}\pi R^3$ y su masa es $m = \rho_s V_s$. Dividiendo toda la ecuación entre $m$:

$$\frac{dv}{dt} = \left( 1 - \frac{\rho_f}{\rho_s} \right) g - \frac{6\pi\eta R}{\rho_s \left(\frac{4}{3}\pi R^3\right)} v \implies \frac{dv}{dt} = g_{\text{efectivo}} - \frac{9\eta}{2\rho_s R^2} v$$

Definimos la constante de amortiguamiento viscoso como:
$$\gamma = \frac{9\eta}{2\rho_s R^2} \quad \text{y el término constante} \quad a = g \left(1 - \frac{\rho_f}{\rho_s}\right)$$

La ecuación diferencial lineal de primer orden resulta:
$$\frac{dv}{dt} = a - \gamma v$$

**2. Resolución:**
Separando variables para integrar bajo las condiciones iniciales de reposo ($v(0) = 0$ en $t = 0$):
$$\int_{0}^{v} \frac{dv'}{a - \gamma v'} = \int_{0}^{t} dt'$$

Haciendo cambio de variable $u = a - \gamma v' \implies du = -\gamma \, dv'$:
$$-\frac{1}{\gamma} \ln\left(\frac{a - \gamma v}{a}\right) = t \implies 1 - \frac{\gamma}{a} v = e^{-\gamma t} \implies v(t) = \frac{a}{\gamma} \left( 1 - e^{-\gamma t} \right)$$

Analizando el comportamiento asintótico cuando $t \to \infty$, la velocidad límite es:
$$v_L = \frac{a}{\gamma} = \frac{g \left(1 - \frac{\rho_f}{\rho_s}\right)}{\frac{9\eta}{2\rho_s R^2}} = \frac{2 R^2 g (\rho_s - \rho_f)}{9\eta}$$

Sustituyendo el valor de $v_L$ y el tiempo característico $\tau_c = \frac{1}{\gamma}$:
$$v(t) = v_L \left(1 - e^{-t/\tau_c}\right)$$

*Cálculos numéricos con los datos:*
* Densidad de la esfera: $\rho_s = 2330\text{ kg/m}^3$
* Densidad del fluido: $\rho_f = 920\text{ kg/m}^3$
* Radio: $R = 100\ \mu\text{m} = 10^{-4}\text{ m}$
* Viscosidad: $\eta = 0.15\text{ Pa}\cdot\text{s}$

*Velocidad Límite:*
$$v_L = \frac{2 \cdot (10^{-4}\text{ m})^2 \cdot (9.81\text{ m/s}^2) \cdot (2330 - 920)\text{ kg/m}^3}{9 \cdot (0.15\text{ Pa}\cdot\text{s})}$$
$$v_L = \frac{2 \times 10^{-8} \cdot 9.81 \cdot 1410}{1.35} = \frac{2.767 \times 10^{-4}}{1.35} \approx 2.05 \times 10^{-4}\text{ m/s} = 0.205\text{ mm/s}$$

*Tiempo característico ($\tau_c$):*
$$\tau_c = \frac{1}{\gamma} = \frac{2\rho_s R^2}{9\eta} = \frac{2 \cdot 2330\text{ kg/m}^3 \cdot (10^{-4}\text{ m})^2}{9 \cdot 0.15\text{ Pa}\cdot\text{s}} = \frac{0.0466}{1.35} \approx 0.0345\text{ s} = 34.5\text{ ms}$$

**3. Discusión Crítica:**
La velocidad límite obtenida es sumamente pequeña ($0.205\text{ mm/s}$), y el tiempo transitorio para alcanzar el $63.2\%$ de este valor es de apenas $34.5\text{ milisegundos}$. Esto significa que para la escala micro-métrica de partículas conductoras en aceites dieléctricos, los efectos transitorios inerciales son casi despreciables y el movimiento está gobernado casi inmediatamente por el arrastre viscoso equilibrado de Stokes.
```

## 📓 III. Actividades para el Portafolio Digital

🧠 Desafío 1

**Caída de Presión en Redes de Distribución de Agua FIEE**

Un tubo horizontal de metal cuyo diámetro interno es de $3\text{ cm}$ y cuya longitud total es de $60\text{ m}$ transporta agua de consumo doméstico a una tasa de flujo de $40\text{ litros/min}$ en la FIEE-UNAC. Tomando la viscosidad del agua como $\eta = 1.005 \times 10^{-3}\text{ Pa}\cdot\text{s}$ y densidad $\rho = 1000\text{ kg/m}^3$.

El Reto: 1. Determine rigurosamente si el flujo es verdaderamente laminar o si se ha desarrollado turbulencia calculando el número de Reynolds.
2. Calcule la pérdida neta de presión requerida entre los extremos de la tubería utilizando el modelo físico correspondiente. Si el flujo es turbulento, investigue y aplique la fórmula de pérdida de presión por fricción turbulenta con un coeficiente de fricción promedio de Darcy de $f_D \approx 0.025$.

Análisis de Sensibilidad: Evalúe cómo se altera el comportamiento del flujo y la pérdida de carga si la temperatura del agua se incrementa hasta los $80^\circ\text{C}$ (donde $\eta$ cae a $3.5 \times 10^{-4}\text{ Pa}\cdot\text{s}$).

🧠 Desafío 2

**El Efecto de la Estenosis y Obstrucciones en Conductos de Enfriamiento**

El radio interno de un conducto cilíndrico de cobre que transporta refrigerante en un alternador de potencia sufre una reducción localizada del $5\%$ en su sección transversal debido a incrustaciones y depósitos de óxido calcáreo.

El Reto: Si se desea mantener el caudal volumétrico perfectamente constante a través del conducto obstruido para evitar el sobrecalentamiento del equipo eléctrico, ¿en qué porcentaje se debe incrementar la diferencia de presiones impuesta entre sus extremos?

Interpretación Biomédica: Utilice este mismo modelo de caída de presión hidrodinámica (Ley de Hagen-Poiseuille) para explicar cuantitativamente las consecuencias de la arteriosclerosis y la estenosis arterial en el sistema cardiovascular humano, detallando el esfuerzo cardiaco adicional requerido ante una obstrucción.

🧠 Desafío 3

**Capacidad de Conducción Máxima en Régimen Laminar**

Se requiere operar una línea de transporte de agua destilada ($\eta = 1.00 \times 10^{-3}\text{ Pa}\cdot\text{s}$, $\rho = 1000\text{ kg/m}^3$) a través de una tubería industrial de $3\text{ cm}$ de diámetro de manera que el fluido nunca experimente perturbaciones turbulentas para evitar ruido acústico e interferencias mecánicas en sensores piezoeléctricos adyacentes.

El Reto: Determina el caudal volumétrico máximo absoluto (en $\text{L/s}$) que puede admitir la tubería bajo un régimen puramente laminar. Considera el límite crítico superior de estabilidad de Reynolds $Re = 2300$.

Análisis Crítico: Si duplicamos el diámetro de la tubería para el mismo caudal máximo de régimen laminar, ¿cómo cambia la pérdida de presión por unidad de longitud? Justifique empleando la relación analítica.

🧠 Desafío 4

**Velocidad Límite de Caída en Medios Viscosos Industriales**

Una pequeña esfera de hierro refinado ($\rho_s = 7800\text{ kg/m}^3$) que posee un radio de $5\text{ mm}$ es liberada desde el reposo en el interior de un gran estanque de almacenamiento de glicerina industrial ($\rho_f = 1260\text{ kg/m}^3$, $\eta = 1.49\text{ Pa}\cdot\text{s}$).

El Reto: 1. Dibuje el Diagrama de Cuerpo Libre (DCL) de la esfera y derive el balance de fuerzas clásico para obtener la velocidad límite (o terminal) alcanzada durante su descenso.
2. Calcule el valor numérico de dicha velocidad límite y determine el número de Reynolds de la esfera ($Re_{\text{esfera}} = \frac{\rho_f v_L D}{\eta}$) para verificar si el uso de la ley de Stokes fue físicamente válido ($Re_{\text{esfera}} < 1$).

🧠 Desafío 5

**Dinámica Transitoria de Stokes con Fuerza Constante**

Retomando de manera analítica el escenario físico planteado en el Desafío 4 (la esfera de hierro descendiendo en el tanque de glicerina):

El Reto: 1. Formule la ecuación diferencial del movimiento derivada de la segunda ley de Newton: $m \frac{dv}{dt} = W - E - 6\pi\eta R v$.
2. Resuelva formalmente la ecuación diferencial por separación de variables para demostrar que la velocidad en función del tiempo es $v(t) = v_L (1 - e^{-t/\tau_c})$.
3. Determine de forma analítica y numérica el instante de tiempo preciso en el cual la esfera alcanza exactamente el $99\%$ de su velocidad límite de descenso.

🧠 Desafío 6

**Pérdida de Carga de Lubricación en Maquinaria Rotativa**
Una porción de aceite dieléctrico y lubricante para máquina pesada de la FIEE ($\eta = 1.13\text{ poise} = 0.113\text{ Pa}\cdot\text{s}$, $\rho = 900\text{ kg/m}^3$) se bombea continuamente a lo largo de un conducto horizontal de interconexión interna de $2\text{ cm}$ de diámetro y $50\text{ m}$ de longitud. El caudal de lubricación nominal está establecido en $2\text{ litros/min}$.

El Reto:

Determine el número de Reynolds y verifique que el flujo opere en el rango laminar.

Calcule de forma rigurosa la caída de presión exacta que experimenta el lubricante debido exclusivamente a la resistencia viscosa interna.

Encuentre la potencia mecánica que debe transferir la bomba para vencer la fricción en este tramo.

🧠 Desafío 7

**Clasificación de Regímenes de Flujo de Aceite en Subestaciones**

Se dispone de una tubería de distribución de fluidos en una planta generadora que posee un diámetro interno de $4\text{ cm}$ para transportar aceite térmico a una temperatura de $15^\circ\text{C}$ ($\eta = 6.60\text{ poise}$, $\rho \approx 900\text{ kg/m}^3$).

El Reto: Determine matemáticamente los intervalos de velocidad media ($v_m$) del flujo dentro de la tubería cilíndrica que corresponden inequívocamente a:

Régimen estrictamente laminar ($Re < 2300$).

Régimen de transición ($2300 \le Re \le 4000$).

Régimen completamente turbulento ($Re > 4000$).

🧠 Desafío 8

**Flotabilidad, Ascenso Viscoso y Sensores Marinos**

Un sensor esférico de monitoreo oceanográfico (fabricado con resina impermeable ligera, masa $m = 1\text{ g}$ y diámetro $D = 4\text{ cm}$) se libera de forma accidental en el fondo de un canal de agua salada de alta densidad ($\rho_f = 1030\text{ kg/m}^3$, $\eta = 1.2 \times 10^{-3}\text{ Pa}\cdot\text{s}$).

El Reto: Sabiendo que el agua ejerce un empuje hidrostático y una fuerza de oposición viscosa regida por la ley de Stokes:

Calcule la densidad de la esfera y verifique que experimentará un empuje neto de ascenso.

Deduzca el balance dinámico y calcule analíticamente la velocidad límite de ascenso vertical del sensor.

¿Será válido el uso de la fórmula de Stokes en este escenario? Evalúe el Número de Reynolds de la esfera para sustentar su respuesta física.

🧠 Desafío 9

**Descenso de Columnas Fluidas en Tubos Capilares**

Una columna de aceite viscoso de $10\text{ cm}$ de longitud ($\eta = 6.60\text{ poise} = 0.66\text{ Pa}\cdot\text{s}$, $\rho = 900\text{ kg/m}^3$) se encuentra dentro de un tubo capilar vertical de $0.5\text{ cm}$ de diámetro interno. La columna líquida desciende lentamente por la acción neta de la gravedad y descarga de forma abierta en su extremo inferior.

El Reto: 1. Equipare el peso efectivo de la columna fluida con la resistencia hidráulica de Poiseuille para deducir una expresión analítica de la velocidad media de descenso.
2. Calcule numéricamente la velocidad con la que fluye la columna a través del capilar.
3. Explique por qué el fenómeno de la tensión superficial en los meniscos podría alterar significativamente este resultado teórico en la práctica.

🧠 Desafío 10

**Caída Libre con Resistencia de Arrastre Cuadrática del Aire**

A velocidades altas (altos números de Reynolds), la fuerza de arrastre ejercida por el aire sobre cuerpos de gran sección transversal deja de ser lineal y pasa a depender cuadráticamente de la rapidez: $F_R = b v^2$. Consideremos un paracaidista de masa $m = 100\text{ kg}$ que se encuentra en caída vertical libre.

El Reto:

Escriba la ecuación diferencial del movimiento bajo esta ley de arrastre: $m \frac{dv}{dt} = mg - bv^2$.

Resuelva analíticamente la ecuación diferencial mediante separación de variables e integración hiperbólica para deducir la velocidad como función del tiempo $v(t)$, asumiendo que parte del reposo.

Encuentre la expresión analítica para la velocidad límite ($v_L$) cuando $t \to \infty$.

Si se desea que el paracaidista alcance una rapidez segura de impacto terrestre de $4\text{ m/s}$ al equilibrarse sus fuerzas, ¿cuál debe ser el valor exacto de la constante de arrastre aerodinámico $b$?