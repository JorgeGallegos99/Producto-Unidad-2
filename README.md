# Producto-Unidad-2
## Informe

### 1. PLANTEAMIENTO DEL PROBLEMA


### 2. OBJETIVOS
**Objetivo General**

● Diseñar una Unidad Aritmética lógica (ALU) con dos números de 8 bits cada uno y multiplexando las salidas,para su comprobaciòn se requiere la simulación e implementación correspondiente.

**Objetivos Específicos**

●	Elaborar una Alu con las operaciones de suma, resta, función or, y función And.

●	Emplear Multiplexores en el integrado 4511 para mostrar en los Displays de 7 segmentos para la visualización de las salidas y el 7483 para la suma.

●	Simular la ALU con 4 operaciones, con la herramienta de software Proteus.

* Implementar el circuito de la Alu diseñado en thinkercad.

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

**Multiplexor**

Un multiplexor, abreviado como “MUX” o “MPX”, es un dispositivo, circuito lógico combinatorio, que permite seleccionar una o más señales de entrada analógicas o digitales de baja velocidad, combinarlas y transmitirlas a mayor velocidad en un único medio compartido o dentro de un único dispositivo compartido.
Así, varias señales pueden compartir un único dispositivo o conductor de transmisión, como un cable de cobre o un cable de fibra óptica. Un MUX funciona como un conmutador de entrada múltiple y salida única.

Los multiplexores funcionan como interruptores rotativos de posición múltiple de acción muy rápida que conectan o controlan varias líneas de entrada llamadas “canales”, una a una, a la salida. Los multiplexores, o MUX, pueden ser circuitos digitales hechos de puertas lógicas de alta velocidad usadas para conmutar datos digitales o binarios o pueden ser de tipo analógico usando transistores, MOSFET o relés para conmutar una de las entradas de voltaje o corriente a través de una sola salida.

Un multiplexor requiere un demultiplexor para completar el proceso, es decir, para separar las señales de multiplexación transportadas por el único medio o dispositivo compartido. A menudo un multiplexor y un demultiplexor se combinan en un solo dispositivo (también llamado a menudo simplemente multiplexor) permitiendo que el dispositivo procese tanto las señales entrantes como las salientes. Alternativamente, la salida única de un multiplexor puede conectarse a la entrada única de un demultiplexor a través de un solo canal. Cualquiera de los dos métodos se utiliza a menudo como medida de ahorro de costes. Dado que la mayoría de los sistemas de comunicación transmiten en ambas direcciones, se necesitará el dispositivo único combinado, o dos dispositivos separados (en el último ejemplo), en ambos extremos de la línea de transmisión.


### 5. DIAGRAMAS
#### 5.1 Diagrama de Funcionamiento

![bloques_Funcionamiento.JPG](https://github.com/JorgeGallegos99/Producto-Unidad-2/blob/master/Img/bloques_Funcionamiento.JPG)

**Figura :** Funcionamiento del Circuito.

![variables.JPG](https://github.com/JorgeGallegos99/Producto-Unidad-2/blob/master/Img/variables.JPG)

**Figura :** Variables de entrada y de Salida del circuito ALU


### 6. LISTA DE COMPONENTES


### 7. MAPA DE VARIABLES


### 8. EXPLICACIÓN DEL CÓDIGO FUENTE


### 9. DESCRIPCIÓN DE PRERREQUISITOS Y CONFIGURACIÓN

Para realizar la multiplexación de las salidas se utilizo el integrado 74153 sus caracteristicas se muestras a continuación.

| **Código**|**Características**	|    
|---------- |--------------------|
|   74153   | **MULTIPLEXOR de 4 a 1 líneas:** contiene dos multiplexores con sus cuatro entradas de datos y su salida cada uno. Tiene dos entradas de inhibición (STROBE 1G y 2G) activas a nivel bajo(0V) para cada multiplexor y dos entradas de selección (SELECT A y B) comunes a los cuatro multiplexores.|  
                                              
![74ls153.jpg](https://github.com/JorgeGallegos99/Producto-Unidad-2/blob/master/Img/74ls153.jpg)

**Figura :** Integrado 74153

En el circuito para realizar la conexión entre las salidas de los circuitos y el display de 7 segmentos hicimos uso de un Decodificador 4511 BCD de 7 segmentos cuyas características se muestran en la tabla 9.

| **Código**|**Características**	|    
|---------- |--------------------|
|   4511    | El CD4511 es un decodificador bcd de 4 bits para display cátodo común, que utiliza tecnología cmos.                                                                             Recibe en los Pines de entrada a ABCD los datos en código binario y los decodifica a código decimal,                                                                             siendo posible su exhibición en los display de 7 segmentos.|  
                                              
![4511.gif](https://github.com/JorgeGallegos99/Trabajo-de-investigacion-2/blob/master/Img/4511.gif)


**Figura :** Integrado 4511

El circuito fue implementado en la plataforma Thinkercad como se muestra que ha acontinuación





|                 **Herramientas de Software**       |                  **Descripción**                      |
|----------------------------------------------------|-------------------------------------------------------|
|              Tinkercad                             | Tinkercad es una sencilla aplicación en línea de diseño e impresión en 3D para todos, creado por la empresa Autodesk. Sus ventajas son claras: es sencillo de usar, su aspecto es atractivo y con unas pocas horas de entrenamiento podemos                                                           adquirir mucha destreza en su uso. Como desventaja podríamos señalar que es necesario tener una cuenta de correo para darse de alta como usuario y que sólo                                                         posee una versión online, por lo que hace falta conexión a internet.|
                                ![Thinkercad.png](https://github.com/JorgeGallegos99/Trabajo-de-investigacion-2/blob/master/Img/Thinkercad.png)
**Figura :** Laboratorio Virtual Tinkercad

### 10. APORTACIONES



### 11. CONCLUSIONES


### 12. RECOMENDACIONES


### 13. CRONOGRAMA


### 14. BIBLIOGRAFÍA

https://teoriadelastelecomunicaciones.files.wordpress.com/2011/11/multiplexacion.pdf

https://www.wikiversus.com/tv/que-es-multiplex/

https://personales.unican.es/manzanom/Planantiguo/EDigitalI/MuxG7_09.pdf

### 15. ANEXOS

**15.1.  MANUAL DE USUARIO**



