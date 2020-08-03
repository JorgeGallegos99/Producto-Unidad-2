# Producto-Unidad-2
## Informe

### 1. PLANTEAMIENTO DEL PROBLEMA

En la rama de los circuitos digitales se emplean operaciones aritméticas binarias en el diseño de diversos circuitos, entre estas operaciones se encuentra la suma y resta. Si bien se conoce que existen compuertas lógicas que permiten realizar este proceso como es el caso del circuito integrado 74LS32 que posee cuatro compuertas en su estructura (para la suma) junto con 74LS04 (para la resta), existen otros integrados que realizan la misma operación y se denominan sumadores.

Cuando se utilizan compuertas lógicas OR (suma) se tiene un número limitado de variables de entrada puesto que si se desea trabajar con un número elevado de estas variables, el proceso de obtención de las funciones lógicas resultantes y la implementación del diseño van a complicarse debido al elevado número de circuitos integrados que se utilizarán y por consecuencia no habrá una optimización de diseño y su construcción será más costosa.

Para esta limitante se emplean los circuitos integrados sumadores; un solo integrado de este tipo realiza la suma de hasta 8 variables de entrada (dos números 4 bits) lo cual facilita el diseño, interpretación, optimización e implementación para el caso de 8bits por número ingresado, con dos integrados sumadores el proceso suma estará resuelto; 4 integrados sumadores junto con copuertas XOR, OR y NOT permiten el proceso de resta con signo.

Considerando las operaciones de suma y resta se tiene la idea de una calculadora binaria que debe tener una sola salida, para este proceso existen los multiplexores, integrados que agrupan cierto número de variables de entrada y la llevan a una única salida dependiendo de un selector.

En base los puntos planteados se pretende implementar una calculadora básica de dos números de 8 bits (16 variables de entrada) utilizando un circuito integrado sumador: LS74283 y el concepto de multiplexores para diseñar una configuración que permita multiplexar las salidas de suma y resta para visualizar su resultado en displays de 7 segmentos.


### 2. OBJETIVOS
**Objetivo General**

● Diseñar una Calculadora binaria de dos números de 8 bits cada uno el resultado debe mostrarse en Display de 7 segmentos, para su comprobación se requiere la simulación e implementación correspondiente.

**Objetivos Específicos**

●	Analizar el funcionamiento de los sumadores para en base a ellos obtener el restador mediante la teoría recibida en clase.

● Construir un circuito que permita multiplexar las operaciones de la calculadora binaria de modo que se pueda decidir la operación al utilizarla.

* Utilizar los integrados 74283 para la suma y resta, el decodificador 4511 de bcd a display de 7 segmentos para mostrar el resultado y la compuertas necesarias.

●	Simular la Calculadora Binaria, en la herramienta de software Proteus.

* Implementar el circuito de la Calculadora Binaria en un laboratorio virtual.

### 3. ESTADO DEL ARTE

1) **Diseño y optimización de ALU de 8 bits utilizando lógica reversible.**

En el articulo  diseñañ una ALU reversible de 8 bits, está diseñada en cascada ALU de 1 bit. Las dos unidades principales de una ALU de 1 bit son la unidad de control y la unidad sumadora. Para la unidad de control, se ha utilizado la puerta de salida de control (COG) y para la unidad sumadora se ha utilizado la puerta Haghparast y Navi (HNG). El aspecto más significativo de este documento es que, en comparación con otros documentos, este diseño ALU ha reducido el recuento de puertas y el recuento de transistores. 

**Autores**

- Un Deeptha

Departamento de Electrónica y Comunicación, RV College of Engineering, Bangalore, India

- Drishika Muthanna

Departamento de Electrónica y Comunicación, RV College of Engineering, Bangalore, India

- M Dhrithi

Departamento de Electrónica y Comunicación, RV College of Engineering, Bangalore, India

- M Pratiksha

Departamento de Electrónica y Comunicación, RV College of Engineering, Bangalore, India

- BS Kariyappa

Departamento de Electrónica y Comunicación, RV College of Engineering, Bangalore, India

**Fecha y lugar de publicación:**

**Fecha:** 20-21 de mayo de 2016

**Lugar:** 2016 Conferencia Internacional IEEE sobre Tendencias Recientes en Electrónica, Tecnología de Información y Comunicación (RTEICT), en  Bangalore, India

Se relaciona con el presente trabajo ya que hace un diseño semejante al presente trabajo utilizan el mismo número bits y en uno de ellos realizan la suma que es una operación que si consta en el presente sin embargo  emplean una lógica reversible y los componentes electrónicos son de otra tegnología. Lo cual los hace totalmente diferentes sin embargo en esencia se relacionan bastante.

2) **Diseño de ALU usando lógica de modo dual con potencia y velocidad optimizadas**

En este articulo se ha implementado un diseño de una Unidad de lógica aritmética (ALU) aprovechando el concepto de técnica de lógica de modo dual (DML). Para el diseño se hace uso de  multiplexor 4 × 1, 2 entradas y unidad, 2 entradas o unidad, unidad exor de 2 entradas y un sumador completo diseñado para implementar operaciones lógicas, como y, o, operación exor y aritmética de suma usando un sumador completo. La técnica DML se ha utilizado para diseñar multiplexores, sumadores completos y unidades, o unidades y unidades exor que luego se asocian para realizar la ALU basada en DML.

**Autores**

- Neetika Yadav

Departamento de VLSI, CDAC, Noida, India

-Preeti Kumari

Departamento de VLSI, CDAC, Noida, India

**Fecha y lugar de publicación:**

**Fecha:** 24-26 de noviembre de 2017

**Lugar:** 2017 Conferencia internacional sobre tecnologías de comunicación, procesamiento de señales y multimedia (IMPACT)  en Aligarh, India.

La ALU realizada en el articulo guarda realción con el nuestro trabajo ya que es un diseño con las caracterisiticas muy parecidas ya que permite sumar, restar, funición or y y funcion and incluso para su implementacion hacen uso de multiplexores sin embargo tienen un sistema avanzado y para la manipulación de datos se basan en DML.

**3) ALU eficiente de baja potencia con sumador completo de baja potencia**

Este artículo presenta una ALU eficiente de bajo consumo de energía usando la lógica XNOR.El sumador completo es el componente básico para una ALU se intodujo uno de baja potencia, que consiste en 8T que se genera usando la lógica 3T XNOR y el multiplexor. Se lo diseño con  4 bits y se compara con varios modelos de implementación de ALU con respecto a su consumo de energía y área. 

**Autores**

- S. Usha

Departamento de ECE, Chettinad College of Engineering and Technology, Karur, India

- M. Rajendiran

ECE, Chettinad College of Engineering and Technology, Karur, India

- A. Kavitha

ECE, Chettinad College of Engineering and Technology, Karur, India


**Fecha y lugar de publicación:**

**Fecha:** 16-18 de marzo de 2016

**Lugar:** 2016 Tercera Conferencia Internacional sobre Informática para el Desarrollo Global Sostenible (INDIACom) en Nueva Delhi, India

La Alu diseñada en el articulo concuerda con el presente trabajo ya que su diseño se basa en la función lógica XNOR pero con la utilzacion de sumadores como el presente trabajo sin embargo ellos usan un sumador completo con una tegnología diferente y mas avanzada  a la que se usa en el presente trabajo.


### 4. MARCO TEÓRICO

**Multiplexación**

La multiplexación es la combinación de dos o máscanales de información en un solo medio de transmisión usando un dispositivo llamado multiplexor.
Es una forma de enviar múltiples señales o flujos de información a través de un medio de comunicaciones compartido al mismo tiempo. Para ello se envía una única señal compleja que el receptor recupera y separa en un proceso llamado demultiplexación.

La multiplexación se originó como una técnica utilizada en la telegrafía (1870) y hoy en día se utiliza ampliamente en todas las formas de telecomunicaciones. Un dispositivo que realiza la multiplexación se conoce como multiplexor o MUX. Un dispositivo que realiza la operación inversa se denomina demultiplexor, DEMUX o DMX.

En la transmisión de radio analógica, las señales son comúnmente multiplexadas usando la multiplexación por división de frecuencia (FDM), en la cual el ancho de banda de un enlace de comunicaciones se divide en subcanales de diferentes anchos de frecuencia, cada uno llevando una señal al mismo tiempo en paralelo. La televisión por cable analógica funciona de la misma manera, enviando múltiples canales de material por las mismas hebras de cable coaxial.

De manera similar, en algunas redes ópticas, los datos de los diferentes canales de comunicaciones se envían en ondas de luz de diferentes longitudes de onda, una variedad de multiplexación llamada multiplexación por división de longitudes de onda (WDM).

Todas estas técnicas utilizan básicamente el mismo concepto. La FDM se usa en la radiodifusión y la televisión, mientras que la WDM se utiliza en las telecomunicaciones y las redes informáticas que utilizan sistemas láser (que generan las señales enviadas a través de cables de fibra óptica).

![multiplexacion](https://github.com/JorgeGallegos99/Producto-Unidad-2/blob/master/Img/Multiplexacion.gif)

**Figura 1.** Multiplexacion 

**Multiplexor**

Un multiplexor, abreviado como “MUX” o “MPX”, es un dispositivo, circuito lógico combinatorio, que permite seleccionar una o más señales de entrada analógicas o digitales de baja velocidad, combinarlas y transmitirlas a mayor velocidad en un único medio compartido o dentro de un único dispositivo compartido.
Así, varias señales pueden compartir un único dispositivo o conductor de transmisión, como un cable de cobre o un cable de fibra óptica. Un MUX funciona como un conmutador de entrada múltiple y salida única.

Los multiplexores funcionan como interruptores rotativos de posición múltiple de acción muy rápida que conectan o controlan varias líneas de entrada llamadas “canales”, una a una, a la salida. Los multiplexores, o MUX, pueden ser circuitos digitales hechos de puertas lógicas de alta velocidad usadas para conmutar datos digitales o binarios o pueden ser de tipo analógico usando transistores, MOSFET o relés para conmutar una de las entradas de voltaje o corriente a través de una sola salida.

Un multiplexor requiere un demultiplexor para completar el proceso, es decir, para separar las señales de multiplexación transportadas por el único medio o dispositivo compartido. A menudo un multiplexor y un demultiplexor se combinan en un solo dispositivo (también llamado a menudo simplemente multiplexor) permitiendo que el dispositivo procese tanto las señales entrantes como las salientes. Alternativamente, la salida única de un multiplexor puede conectarse a la entrada única de un demultiplexor a través de un solo canal. Cualquiera de los dos métodos se utiliza a menudo como medida de ahorro de costes. Dado que la mayoría de los sistemas de comunicación transmiten en ambas direcciones, se necesitará el dispositivo único combinado, o dos dispositivos separados (en el último ejemplo), en ambos extremos de la línea de transmisión.

![Multiplexor](https://github.com/JorgeGallegos99/Producto-Unidad-2/blob/master/Img/Multiplexor.png)

**Figura 2.** Multiplexor

Se denomina multiplexor 2:1 a aquel que como su propio nombre indica, tiene dos entradas de datos 2n= 2 y una entrada de selección n = 1.

El multiplexor más simple es el que sólo tiene una entrada de selección, S, que permite seleccionar entre dos entradas de datos, según que S = 0 ó S = 1.

Su aspecto es el siguiente:

![multiplexor2a1]()

**Figura. ** Mutilpexor 2 a 1

¿Cómo podemos expresar la función de salida F, usando el Algebra de Boole?.

Existe una manera muy sencilla y que ya conocemos: hacer la tabla de verdad y obtener la función más simplificada.

Construyamos la tabla de verdad; lo primero que nos preguntamos es, ¿cuántas entradas tengo en este circuito?, en total hay tres entradas: dos son de datos:I0 e I1 y una es de selección: S.

La tabla de verdad tendrá en total 23 = 8 filas. Para construir esta tabla de verdad sólo hay que entender el funcionamiento del multiplexor e ir caso por caso rellenando la tabla.

¿qué ocurre si S = 0?. Pues que a la salida del multiplexor obtendremos los datos que entren por la entrada I0. Si aplicamos la definición de multiplexor, se está seleccionando la entrada de datos 0, es decir, la entrada I0. Por tanto, lo que entre por la entrada I1 será ignorado por el multiplexor. Si la entrada seleccionada es la I1, la salida tendrá su mismo valor.

De esta forma, su tabla de verdad será:

  Tabla de Verdad     

   | **S** | **M ** | **N** | **F** | 
   | -----|---------| ------| ----------- |
   | 0 | 0 | 0 | 0                  |
   | 0 | 0 | 1 | 0          |      
   | 0 | 1 | 0 | 1     |       
   | 0 | 1 | 1 | 1     |       
   | 1 | 0 | 0 | 0     |
   | 1 | 0 | 1 | 1    |
   | 1 | 1 | 0 | 0      |
   | 1 | 1 | 1 | 1       |


**Circuitos Aritméticos**

Dentro de la variada gama de circuitos digitales, tenemos los denominados circuitos aritméticos que son dispositivos que pueden realizar operaciones aritméticas (suma, 
resta, multiplicación y división) en formato binario o BCD, punto fijo o punto flotante. 

Dependiendo de la función a realizar, tenemos sumadores, restadores, multiplicadores, divisores y funciones combinadas de los mismos para realizar operaciones complejas como por 
ejemplo el cálculo de raíz cuadrada, exponenciales, etc.

Si bien es posible generar funciones complejas en base al uso de un microprocesador, a través de algoritmos que se corren en un programa, la posibilidad de generar dichas 
funciones en hardware, en muchos casos, presentan ventajas en cuanto a velocidad y/o el empleo de menores recursos lógicos, como es el caso de la ausencia de un micro para realizarlas (Hoyos Padilla, 2010).

**Sumadores**

La suma o adición binaria es análoga a la de los números decimales. La diferencia radica en que en los números binarios se produce un acarreo (carry) cuando la suma excede de uno mientras en decimal se produce un acarreo cuando la suma excede de nueve (Hoyos Padilla, 2010).

 ![jf1](https://github.com/JorgeGallegos99/Trabajo-de-investigacion-2/blob/master/Img/jf1.jpg)

**Figura 3.** Reglas de la Suma Binaria

**Semisumador**

Se denomina semisumador a un circuito que admite dos bits como entrada y genera  como salida  un bit que representa la suma de los dos bits de entrada y otro bit que representa 
el acarreo generado por la suma.

La tabla de verdad de este circuito puede deducirse a partir de las La tabla de verdad de este circuito puede deducirse a partir de las reglas de la suma binaria (Véase Fig.2).

![jf2](https://github.com/JorgeGallegos99/Trabajo-de-investigacion-2/blob/master/Img/jf2.png)

**Figura 4.** Tabla de verdad del Semisumador.

A partir de esta tabla de verdad se puede observar que la suma puede implementarse con una operación XOR y el acarreo de salida con una operación AND(Canaria, 2012).

![jf3](https://github.com/JorgeGallegos99/Trabajo-de-investigacion-2/blob/master/Img/jf3.png)

**Figura 5.** Esquema del Semisumador

**Sumador Completo**

La principal diferencia diferencia entre un sumador completo y un semisumador es que el sumador completo admite un valor que representa un acarreo de entrada.

 ![jf4](https://github.com/JorgeGallegos99/Trabajo-de-investigacion-2/blob/master/Img/jf4.png)
 
 **Figura 6.** Tabla de verdad del Sumador Completo

Dado que la suma de dos bits está dada la operación XOR, también podemos expresar dicha suma  con un acarreo de la siguiente forma:

![jf5](https://github.com/JorgeGallegos99/Trabajo-de-investigacion-2/blob/master/Img/jf5.png)

**Figura 7.** Expresión lógica del Sumador Completo

El acarreo de salida sera 1 entonces cuando A y B sean 1 o cuando A+B sea 1 al igual que el acarreo de entrada.

![jf6](https://github.com/JorgeGallegos99/Trabajo-de-investigacion-2/blob/master/Img/jf6.png)

**Figura 8.** Expresión Lógica

De esta forma se puede implementar el circuito sumador completo usando dos compuertas XOR, dos compuestas AND y una compuerta OR.

![jf7](https://github.com/JorgeGallegos99/Trabajo-de-investigacion-2/blob/master/Img/jf7.png)

**Figura 9.** Esquema del Sumador Completo

También es posible implementar el sumador completo utilizando dos circuitos semisumadores, el primer semisumador suma los dos bits, el segundo suma el resultado con el acarreo 
de entrada y habrá acarreo de salida si cualquiera  de los dos semisumadores genera un acarreo.

![jf8](https://github.com/JorgeGallegos99/Trabajo-de-investigacion-2/blob/master/Img/jf8.png)

**Figura 10.** Sumador COmpleto a Partir de Semisumadores en Cascada

**Sumadores con Acarreo en Cascada**

El circuito sumador completo permite sumar dos números de un bit con un acarreo de entrada y generar un acarreo de salida. Como regla general, un sumador binario de cualquier número de bits puede realizarse conectando en cascada varios sumadores completos de un bit.

El proceso puede extenderse usando cuaquier sumador como elemento básico: por ejemplo puede hacerse un suamdor de 4 bits a partir de dos sumadores de 2 bits.

![jf9](https://github.com/JorgeGallegos99/Trabajo-de-investigacion-2/blob/master/Img/jf9.png)

**Figura 11.** Sumadore de 4 bits

El principal problema de esta conexión en serie de sumadores es que el retardo del circuito depende de la propagación del acarreo a lo largo de todo el sumador.

![jf10](https://github.com/JorgeGallegos99/Trabajo-de-investigacion-2/blob/master/Img/jf10.png)

**Figura 12.** Sumador de 8 bits 

Para la implementación del sumador de 8 bits se dio uso al integrado 74283

![jf11](https://github.com/JorgeGallegos99/Trabajo-de-investigacion-2/blob/master/Img/jf11.jpg)

**Figura 13.** Integrado 74283

La resta se implementa mediante un sumador. El método consiste en llevar al minuendo a una de las entradas y el sustraendo en complemento 2 a la otra entrada.

Un medio restador es un circuito combinacional que sustrae dos bits y produce su diferencia. También tiene la salida para especificar si se ha tomado un 1. Se designa el bit minuendo por x y el bit sustraendo mediante y. Para llevar a cabo x – y, tienen que verificarse las magnitudes relativas de x y y. Si x >= y, se tienen tres posibilidades; 0 - 0 = 0, 1 – 0 = 1 y, 1 - 1 = 0. El resultado se denomina bit de diferencia. Si x < y, tenemos 0 – 1 y es necesario tomar un 1 de la siguiente etapa más alta. El 1 que se toma de la siguiente etapa más alta añade dos al bit minuendo, de la misma forma que en el sistema decimal lo que se toma añade 10 a un dígito minuendo. Con el minuendo igual a 2, la diferencia llega a ser 2 – 1 = 1. El medio restador requiere dos salidas. Una salida genera la diferencia y se denotará por el símbolo D. La segunda salida, denotada B para lo que se toma, genera la señal binaria que informa a la siguiente etapa que se ha tomado un 1. 

![Restador Completo](https://github.com/JorgeGallegos99/Producto-Unidad-2/blob/master/Img/Restador%20Completo.gif)

**Figura 14.** Restador Completo

### 5. DIAGRAMAS
#### 5.1 Diagrama de Funcionamiento

![bloques_Funcionamiento.JPG](https://github.com/JorgeGallegos99/Producto-Unidad-2/blob/master/Img/bloques_Funcionamiento.JPG)

**Figura 15.** Funcionamiento del Circuito.

![restador.JPG](https://github.com/JorgeGallegos99/Producto-Unidad-2/blob/master/Img/restador.JPG)

**Figura 15.1.** Diagrma de bloques del Restador

![sumador.png)](https://github.com/JorgeGallegos99/Producto-Unidad-2/blob/master/Img/sumador.png)

**Figura 15.2.** Diagrma de bloques del Restador


#### 5.2 Diagrama de Variables

![variables.JPG](https://github.com/JorgeGallegos99/Producto-Unidad-2/blob/master/Img/variables.JPG)

**Figura 16.** Variables de entrada y de Salida del circuito Calculadora Binaria


#### 5.3 DiagramasElectrónicos.

![circuitoProteus.png](https://github.com/JorgeGallegos99/Producto-Unidad-2/blob/master/Img/circuitoProteus.png)

**Figura 17.**  Circuito en Proteus.


**Implementacion del circuito  en el Constructor virtual**

![IMPLEM1.JPG](https://github.com/JorgeGallegos99/Producto-Unidad-2/blob/master/Img/IMPLEM1.JPG)

**Figura 18.** Parte 1

![IMPLEM2.JPG](https://github.com/JorgeGallegos99/Producto-Unidad-2/blob/master/Img/IMPLEM2.JPG)

**Figura 19.** Parte 2

![IMPLEM3.JPG](https://github.com/JorgeGallegos99/Producto-Unidad-2/blob/master/Img/IMPLEM3.JPG)

**Figura 20.** Parte 3

![IMPLEM4.JPG](https://github.com/JorgeGallegos99/Producto-Unidad-2/blob/master/Img/IMPLEM4.JPG)

**Figura 21.** Parte 4

### 6. LISTA DE COMPONENTES

En la Tabla 1 se muestra las herramientas  de software usadas para la simulacion del circuito se utilizó un simulador y la plataforma para la implementación.

**Tabla 1: Herramientas de Software usadas para el diseño de los 3 circuitos.**

   |     **Herramientas de Software**      |                 
   |---------------------------------------|
   |            Proteus                    | 
   |           Constructor Virtual         |
  
   
**Tabla 2: Datos de los integrados usados para el diseño de Circuito Sumador de 8 bits**

   | **N°**  |   **Integrados** |   **Códigos**    |     
   |-------  |--------------|----------------|
   |      13 |   Sumador	  |     74283      |
   |      3  | Decodificador|     4511       |
   |      4  | NOT |     7404       |
   |      2  | EXOR |     7486      |
   |      7  | AND |     7408      |
   |      6  | OR |     7432     |
   
   
  
**Tabla 3: Componentes electronicos del Circuito Sumador de 8 bits**

  | **N°** |**Componentes Electronicos**	|    
   |-------|------------------------------|
   |     47|   Resistencias de 330        |    
   |      2|   Dip Switch 8 entradas      |     
   |      1|   Fuente de 5 V              |   
   |      16|   Led Green                 | 
   |      3|   Display 7 segmentos        | 
   |      1|   Dip Switch 1 entrada      | 


### 7. MAPA DE VARIABLES

 |**Variable** | 	**Tipo**   | **Descripción**|
 |-------------|----------------|-------------------|
 |A0,A1,A2,A3,A4,A5,A6,A7|  Entrada|Son los bits de Entrada del numero A donde A7 es el bit mas significativo y A0 es el bit menos significativo|
 |B0,B1,B2,B3,B4,B5,B6,B7| Entrada|	Son los bits de Entrada del numero B donde B7 es el bit mas significativo y B0 es el bit menos significativo|
 |M0,M1,M2,M3,M4,M5,M6,M7,M8| Salida|Bits del resultado de la operación suma donde M0  el bit menos significativo y M7 es el bit mas significativo|
 |N0,N1,N2,N3,N4,N5,N6,N7,N8| Salida| Bits del resultado de la operación resta donde N0  el bit menos significativo y N7 es el bit mas significativo|
 |G0,G1,G2,G3,G4,G5,G6,G7,G8| Salida|Bits que nos devuelve el mutiplexor dependiendo del selector|
 |SIG|Salida| Signo de la operación resta|

### 8. EXPLICACIÓN DEL CÓDIGO FUENTE
* Para realizar el circuito sumador de dos números de 8 bits primero se definen las variables de entrada y salida que tendrá el circuito, todas se encuentran en lógica positiva y se presentan de la siguiente forma:

![Diagrama de bloques: Sumador 8 Bits](https://github.com/JorgeGallegos99/Producto-Unidad-2/blob/master/Img/ENTRADAS.png)

**Figura 22.** Diagrama de bloques: Sumador 8 Bits

**Entradas**

**Número A**: A7, A6, A5, A4, A3, A2, A1, A0
Donde: A0 es el bit menos significativo y A7 es el más significativo

**Número B**: B7, B6, B5, B4, B3, B2, B1, B0
Donde: B0 es el bit menos significativo y B7 es el más significativo

![Entradas en DIPSW](https://github.com/JorgeGallegos99/Producto-Unidad-2/blob/master/Img/DIPSENTRADAS.PNG)

**Figura 23.** Entradas en DIPSW

**Salidas**

M8,M7,M6,M5,M4,M3,M2,M1,M0

Donde: M0 es el bit menos significativo y M8 (acarreo) es el más significativo.

* Para realizar el proceso de la suma binaria se utiliza el circuito integrado 74LS283 que cumple la función de sumador.

![Sumador LS74283](https://github.com/JorgeGallegos99/Producto-Unidad-2/blob/master/Img/SUM.png)

**Figura 24 .** Sumador LS74283

Donde A0 - A3 representan los cuatro primeros bits del número A y B0 - B3 del número B, sin embargo, los números de las entradas son de 8 Bits de magnitud entonces para realizar la suma se necesita realizar una conexión en cascada entre dos sumadores.

Para que se cumpla el proceso se debe conocer las reglas de la suma binaria:

![Reglas de la suma binaria](https://github.com/JorgeGallegos99/Producto-Unidad-2/blob/master/Img/REGLASUMA.PNG)

**Figura 25.** Reglas de la suma binaria

El integrado 74LS283 tiene dos pines que representan el acarreo de entrada y salida, entonces para realizar la conexión en cascada: el acarreo de salida del primer sumador es el acarreo de entrada del segundo, por lo tanto, ambos se encuentran conectados y en las entradas del integrado se colocan las cuatro variables restantes de los números A y B, las cuales son: A4 - A7 y B4 - B7 identificando la conexión de los bits más y menos significativos.

![Conexión en cascada](https://github.com/JorgeGallegos99/Producto-Unidad-2/blob/master/Img/CASCADA.png)

**Figura 26.** Conexión en cascada

 * Las salidas de los sumadores representan el resultado de la suma realizada por el circuito integrado y se encuentran conectadas a unos LEDS, de tal forma que cuando el LED se enciende, representa un 1 y cuando se apaga representa un 0.
 
Donde:

M0=A0+B0

M1=A1+B1

M2=A2+B2

M3=A3+B3

M4=A4+B4

M5=A5+B5

M6=A6+B6

M7=A7+BB7

M8=Acarreo de salida del segundo sumador

* Para el circuito restador se utiliza el complemento a 1:

![Complemento a 1](https://github.com/JorgeGallegos99/Producto-Unidad-2/blob/master/Img/COMPLEMENTO1.PNG)

**Figura 27.** Complemento a 1 

Utilizando este concepto se niega el número B por utilizando inversores y se suma este resultado al número A teniendo como acarreo de entrada un uno lógico: 5V

![Negacion de B](https://github.com/JorgeGallegos99/Producto-Unidad-2/blob/master/Img/NEGADO.png)

**Figura 28.** Negación de B

Para encontrar el signo de la resta,es decir cuando A sea menor a B se utiliza la compuerta XOR y el acarreo de salida resultante de la suma realizando una conexión en cascada para volver a complementar la salida anterior de la siguiente manera:

![XOR](https://github.com/JorgeGallegos99/Producto-Unidad-2/blob/master/Img/RESTA1.png)

**Figura 29.** XOR en la resta

Para un sumador completo de 8 Bits se debe realizar el mismo proceso de complemento a 1 para los 4 bits restantes de ambos números ingresados. De esta forma el restador completo de 8 Bits con signo se establece de la siguiente forma:

![Restador](https://github.com/JorgeGallegos99/Producto-Unidad-2/blob/master/Img/RESTA.png)

**Figura 30.** Restador

Las salidas del restador se encuentran conectadas a unos LEDS, de tal forma que cuando el LED se enciende, representa un 1 y cuando se apaga representa un 0.

Donde:

N0=A0+B0

N1=A1+B1

N2=A2+B2

N3=A3+B3

N4=A4+B4

N5=A5+B5

N6=A6+B6

N7=A7+BB7

S=SIGNO

El signo del restador completo está dado por la suma de los signos correspondientes a los primeros 4 bits de los números y los 4 bits siguientes:

![Signo del restador](https://github.com/JorgeGallegos99/Producto-Unidad-2/blob/master/Img/SIGNO.png)

**Figura 31.** Signo del restador

Las salidas del sumador y restador deben mostrar un solo resultado dependiendo de la operación que se elija por medio de un selector: 

![Selector](https://github.com/JorgeGallegos99/Producto-Unidad-2/blob/master/Img/SELECTOR.png)

**Figura 32.** Selector

Estos selectores se encuentran conectados a Multiplexores de 2:1 es decir, dos entradas y una salida. Existen integrados como el 74HC153 que realizan el proceso de multiplexar las salidas:

![Multiplexores 74HC153](https://github.com/JorgeGallegos99/Producto-Unidad-2/blob/master/Img/MULTIPLEXORES.png)

**Figura 33.** Multiplexores 74HC153

Las entradas de estos MUX estan conformadas por las salidas del circuito sumador y restador, es decir:

M0-M7-ACARREO(M8): SUMA

N0-N7-(SIGNO): RESTA

Selector: 1 suma, 0 resta

Las salidas del MUX dependerán del selector y será:

G0-G7 + (G8: ACARREO SUMA, G9: SIGNO RESTA)

Sin embargo es posible diseñar estos mux por medio de compuertas lógicas ya conocidas: AND, OR, NOT. Para un MUX 2:1 la configuración es la siguiente:

![MUX](https://github.com/JorgeGallegos99/Producto-Unidad-2/blob/master/Img/Mux.png)

**Figura 34.** MUX

* Para visualizar este resultado en un display de 7 segmentos se utiliza el decodificador 4511 conectado a las salidas de un decodificador de binario 8 Bits a BCD y a su vez a las entradas del display junto con resistencias para evitar que el dispositivo sufra daños.

![Decodificador 8Bits a BCD](https://github.com/JorgeGallegos99/Producto-Unidad-2/blob/master/Img/DECO.png)

**Figura 35.* Decodificador 8Bits a BCD

![Decodificador 4511](https://github.com/JorgeGallegos99/Producto-Unidad-2/blob/master/Img/DECODIFICADOR.PNG)

**Figura 36.** Decodificador 4511

* Para conectar el display se debe tomar en cuenta la estructura que posee, para este circuito se usa un display 7 segmentos cátodo común. Esto quiere decir que el pin común del display debe ir conectado a tierra:

![Display 7 seg catodo común](https://github.com/JorgeGallegos99/Producto-Unidad-2/blob/master/Img/DISPLAY.PNG)

**Figura 37.** Display 7 seg catodo común

* El resultado se todos estos procesos da un circuito sumador/restador de dos números de 8 bits como se muestra a continuación en el software de simulación Proteus:

![Simulación Proteus](https://github.com/JorgeGallegos99/Producto-Unidad-2/blob/master/Img/SimulacionProteus.png)

**Figura 38.** Simulación Proteus


### 9. DESCRIPCIÓN DE PRERREQUISITOS Y CONFIGURACIÓN

Para realizar la multiplexación de las salidas se utilizo el integrado 74153 sus caracteristicas se muestras a continuación.

| **Código**|**Características**	|    
|---------- |--------------------|
|   74153   | **MULTIPLEXOR de 4 a 1 líneas:** contiene dos multiplexores con sus cuatro entradas de datos y su salida cada uno. Tiene dos entradas de inhibición (STROBE 1G y 2G) activas a nivel bajo(0V) para cada multiplexor y dos entradas de selección (SELECT A y B) comunes a los cuatro multiplexores.|  
                                              
![74ls153.jpg](https://github.com/JorgeGallegos99/Producto-Unidad-2/blob/master/Img/74ls153.jpg)

**Figura 39.** Integrado 74153

En el circuito para realizar la conexión entre las salidas de los circuitos y el display de 7 segmentos hicimos uso de un Decodificador 4511 BCD de 7 segmentos cuyas características se muestran en la tabla 9.

| **Código**|**Características**	|    
|---------- |--------------------|
|   4511    | El CD4511 es un decodificador bcd de 4 bits para display cátodo común, que utiliza tecnología cmos.                                                                             Recibe en los Pines de entrada a ABCD los datos en código binario y los decodifica a código decimal,                                                                             siendo posible su exhibición en los display de 7 segmentos.|  
                                              
![4511.gif](https://github.com/JorgeGallegos99/Trabajo-de-investigacion-2/blob/master/Img/4511.gif)


**Figura 40.** Integrado 4511

El circuito fue implementado en la plataforma Thinkercad como se muestra que ha acontinuación


|                 **Herramientas de Software**       |                  **Descripción**                      |
|----------------------------------------------------|-------------------------------------------------------|
|              Tinkercad                             | Tinkercad es una sencilla aplicación en línea de diseño e impresión en 3D para todos, creado por la empresa Autodesk. Sus ventajas son claras: es sencillo de usar, su aspecto es atractivo y con unas pocas horas de entrenamiento podemos                                                           adquirir mucha destreza en su uso. Como desventaja podríamos señalar que es necesario tener una cuenta de correo para darse de alta como usuario y que sólo                                                         posee una versión online, por lo que hace falta conexión a internet.|

![Thinkercad.png](https://github.com/JorgeGallegos99/Trabajo-de-investigacion-2/blob/master/Img/Thinkercad.png)

**Figura 41.** Laboratorio Virtual Tinkercad

### 10. APORTACIONES

Adicional al Sumador y al restador se realizo la implementacion de las funciones AND y OR para completar una ALU

![Aporte](https://github.com/JorgeGallegos99/Producto-Unidad-2/blob/master/Img/Aporte.png)

**Figura 42.** Funciones And y OR implementadas al circuito 


### 11. CONCLUSIONES

•	Para realizar la suma de dos números de 8 bits se debe realizar una conexión en cascada de dos sumadores para que se refleje el resultado completo.

•	Para el resultado de cualquier operación suma se debe considerar cuales son los números más grandes que se pueden sumar y por lo tanto siempre aumenta un bit a la salida, por lo tanto, si se operan dos números de 8 bits cada uno, el resultado será un binario de 9 bits.

•	Para realizar la resta debemos tomar en cuenta si el número B es mayor al número A, cuando esto suceda obligatoriamente se tiene que mostrar el resultado como un número negativo. 

•	Hay que tomar en cuenta que para los displays de 7 segmentos el número más alto que se puede visualizar es el nueve, por lo tanto, cuando el resultado de la suma implique un número mayor al indicado, no se va a encender el display.

•	La manera idónea para conectar sumadores es atar el acarreo de salida del sumador de menor peso, con el acarreo de entrada del integrado de mayor peso, y de esta manera el residuo de la suma es transferido para tomar en cuenta cualquier valor que venga acumulado. 

•	Tinkercad es un laboratorio virtual que posee varios componentes electrónicos y nos permite visualizar el comportamiento de elementos electrónicos, sin embargo, cuando los circuitos son muy complejos esta herramienta deja de ser eficiente.

### 12. RECOMENDACIONES

• Se debe tomar en cuenta el valor del acarreo de entrada y salida para cada sumador ya que puede aleterar el resultado.

• Debemos establecer adecuadamente los bits mas significativos y menos significativos que van a ingresar a cada sumador.

• Para las conexion adecuada del display se debe conciderar si será de ánodo o cátodo común para asegurar un correcto funcionamiento del mismo en el circuito diseñado.

• Verificar que no se encuentren conectadas entradas y/o salidas en un mismo punto para que no se generen errores de operación y así evitar que nuestro integrado daños en el integrado.

• Debemos tener claro como se realiza la operacion resta, de esta forma sera mas facil la comprension del funcionamiento del circuito implementado.

• Tinkercad es una potente herramienta de simulacion, preso presenta algunos inconvenientes cuando el circuito es muy complejo.


### 13. CRONOGRAMA

![Cronograma](https://github.com/JorgeGallegos99/Producto-Unidad-2/blob/master/Img/Cronograma.png)

**Figura 43.** Cronograma Monday

### 14. BIBLIOGRAFÍA

https://teoriadelastelecomunicaciones.files.wordpress.com/2011/11/multiplexacion.pdf

https://www.wikiversus.com/tv/que-es-multiplex/

https://personales.unican.es/manzanom/Planantiguo/EDigitalI/MuxG7_09.pdf

https://wilaebaelectronica.blogspot.com/2017/01/sumador-binario.html

https://iesbernatguinovart.com/04v_tecnologia/carpeta_arxius/elec%20dig%20basica.pdf

https://www.studocu.com/pe/document/universidad-nacional-del-callao/circuitos-digitales-turno-01t-ciclo-5/informe/circuitos-aritmeticos/5637738/view

http://homepage.cem.itesm.mx/garcia.andres/PDF201411/Aritmetica(Basis).pdf

http://circuitos-aritmeticos.blogspot.com/

http://serdis.dis.ulpgc.es/~gii-fc/material_clases_teoria/Tema3/Tema3_1_Componentes_combinacionales_FC_GII.pdf

http://electroucn.blogspot.com/2014/06/Restador.html


### 15. ANEXOS

**15.1.  MANUAL DE USUARIO**

1. Ingresar los números binarios con los que sedesea operar en las entradas del dip switch:

![VARENTRADAS](https://github.com/JorgeGallegos99/Producto-Unidad-2/blob/master/Img/VARENTRADAS.PNG)
**Figura 44.** Paso 1
2. Escoger la operación que se desea realizar por medio del selector, siendo 1 suma y 0 resta:

![DIPSELECTOR](https://github.com/JorgeGallegos99/Producto-Unidad-2/blob/master/Img/DIPSELECTOR.PNG)

**Figura 45.** Paso 2

3. Si se escoge 1:
La operación suma se realiza por medio del circuito sumador en cascada implementado:

![SUMA](https://github.com/JorgeGallegos99/Producto-Unidad-2/blob/master/Img/SUMA.PNG)

4. La salida de verificación resultado para la suma se da en los siguientes leds, siendo 1 encendido y 0 apagado.

![LEDSUMA](https://github.com/JorgeGallegos99/Producto-Unidad-2/blob/master/Img/LEDSUMA.PNG)

5. Si se escoge 0:
La operación resta se realiza por medio del circuito restador con signo implementado:

![RESTA](https://github.com/JorgeGallegos99/Producto-Unidad-2/blob/master/Img/RESTA.PNG)

6. La salida de verificación de resultado para la resta se da en los siguientes leds, siendo 1 encedido y 0 apagado.

![LEDRESTA](https://github.com/JorgeGallegos99/Producto-Unidad-2/blob/master/Img/LEDRESTA.PNG)

7. Para poder visualizar ambas salidas en un solo resultado dependiente del selector, se utilizan multiplexores de 2:1 para multiplexar las salidas de la suma y resta del circuito.

![MULTIPLEXORES](https://github.com/JorgeGallegos99/Producto-Unidad-2/blob/master/Img/MUX2.1.PNG)

8. La primera salida de verificación de resultado para la calculadora básica se da en los siguientes leds, siendo 1 encedido y 0 apagado.

![LEDRESULTADO](https://github.com/JorgeGallegos99/Producto-Unidad-2/blob/master/Img/LEDRESULTADO.PNG)

9. La segunda salida de visualización de resultado para la calculadora básica se da en los displays de 7 Segmentos conectados al decodificador BCD y este a su vez conectado al decodificador de binario de 8bits a bcd

![DISPLAYRESULTADO](https://github.com/JorgeGallegos99/Producto-Unidad-2/blob/master/Img/DISPLAYRESULTADO.PNG)


