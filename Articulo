Diseño y desarrollo de un sistema embebido de adquisición, monitoreo, control y envío a distancia de datos de invernadero (KATSI). 
Design and development of an embedded system for acquisition, monitoring, control and remote transmission of greenhouse data (KATSI). 
Ortiz-Pineda, Cristian Jesús*’, Ramos-Guerrero, Ramses-Alejandro’, Castro-Reyes’, Daniel. 
‘Universidad Politécnica de Juventino Rosas. Departamento de Ingeniería en Redes y Telecomunicaciones.  
ID 1er Autor: Cristian Jesús, Ortiz Pineda  
ID 2do Co-Autor: Ramsés Alejandro, Ramos-Guerrero  
ID 3er Co-Autor: Daniel Castro, Reyes
 
Resumen                                                        
La utilización de mejores recursos en la agricultura se ha vuelto más crucial en los últimos tiempos, particularmente en el seguimiento y control de las condiciones ambientales en los invernaderos. La producción de diversos cultivos necesita de sistemas inteligentes que sean autosustentables y maximicen los beneficios. Este invernadero sofisticado es un proyecto capaz de captar y medir variables ambientales como la humedad, la humedad del suelo, la temperatura y los gases dañinos como el CO2. El sistema tiene como objetivo registrar y regular estas variables, permitiendo una toma automatizada de decisiones, como la activación de sistemas de riego. Los principios de guiarán la implementación del proyecto La utilización de microcontroladores, sensores especializados y técnicas avanzadas como conversión analógico-digital, multiplexación y análisis datos. La información recabada es transmitida a un dispositivo central de seguimiento y control, que supondrá una disminución tanto del consumo de agua como de los gastos operativos.

 Abstract
The use of better resources in agriculture has become more crucial in recent times, particularly in the monitoring and control of environmental conditions in greenhouses. The production of various crops requires intelligent systems that are self-sustaining and maximize profits. This sophisticated greenhouse is a project capable of capturing and measuring environmental variables such as humidity, soil moisture, temperature, and harmful gases like CO2. The system aims to record and regulate these variables, enabling automated decision-making, such as the activation of irrigation systems. The principles that will guide the project's implementation are the use of microcontrollers, specialized sensors, and advanced techniques such as analog-to-digital conversion, multiplexing, and data analysis. The information collected is transmitted to a central monitoring and control device, which will lead to a reduction in both water consumption and operating costs.



 
Citación: Ortiz-Pineda, Cristian Jesús, Ramos-Guerrero, Ramses-Alejandro, Daniel-Castro, Reyes, Diseño y desarrollo de un sistema embebido de adquisición, monitoreo, control y envío a distancia de datos de invernadero (KATSI)

*Correspondencia del Autor (322030253@upjr.edu.mx)

 
1.- Introducción 
La principal fuente de energía en los humanos radica en la alimentación, con la creciente población, mundial y local, se debe buscar la forma de dar sustento de una forma más eficiente. Al estar en contacto directo con la población en general, se debe instalar un invernadero inteligente lugares donde es más difícil recibir alimento como, por ejemplo, comunidades apartadas de la ciudad, al estar ubicados en diferentes lugares, cada invernadero deberá acoplar las diferencias ambientales (humedad, temperatura, etc.) a un punto de equilibrio donde favorezca el crecimiento de las plantas.
2.- Materiales 
En la elaboración de este proyecto se realizó una investigación y varias pruebas para determinar y seleccionar los materiales más óptimos y precisos a la visión del proyecto KATSI.
              
Figura 1: Sensor LM35
En la figura 1 se presenta uno de los 3 sensores a utilizar, en este caso es el analógico LM35, Sensor de temperatura.
             
Figura 2. Sensor DHT11 
En la figura 2 se aprecia el segundo sensor a utilizar, se trata del sensor de humedad y temperatura dht11, donde a diferencia de los demás sensores que son del tipo analógico este sensor es del tipo digital.
          
Figura 3. Sensor de humedad del suelo, YC-28 
En la figura 3 se muestra el tercer y último sensor que muestra la humedad, sin embargo, a diferencia del dht11 este muestra la humedad que tiene la tierra de una planta.
 
Figura 4. Modulo USART
En la figura 4 se muestra el enlace que tiene el circuito con una computadora, hablamos del módulo USART FT232R, un conversor USB a serial.
          
Figura 5. PIC 18f4550 
En la figura 5 se presenta el microcontrolador PIC 18f4550 con el cual se estará desarrollando el proyecto para el procesamiento de la información y automatización.
              
Figura 6. Pantalla OLED
En la figura 6 se puede apreciar una pantalla oled la cual servirá para exhibir las mediciones que las placas dentro del invernadero estén midiendo a por medio de los sensores y el microcontrolador.
                
Figura 7. Oscilado de cristal 
A fin de dar una correcta sincronía a las operaciones que está realizando el microcontrolador es necesaria la implementación de un oscilador el cual dará la sincronía suficiente y el cual es posible apreciar en la figura 7.
           
Figura 8. Modulo Xbee 
Xbee son módulos de comunicación inalámbrica fabricados por DIGI International. Que permite desarrollar aplicaciones más allá de la simple conexión y comunicación entre mismos módulos.
 
Figura 9. Sensor MQ-135 
Este sensor se especializa en la detección de diversos gases nocivos para la salud, como podría ser el metano, CO2, etc.
            
Figura 10.- Arduino uno
Arduino es una plataforma de desarrollo de hardware y software libre que permite a las personas crear dispositivos digitales e interactivos fácilmente. La compañía diseña y fabrica placas de desarrollo que pueden ser programadas para interactuar con el mundo real a través de sensores y actuadores.
Metodología
Sistema Embebido
Para el funcionamiento del proyecto se desarrollará un sistema embebido empleando microcontroladores en este caso se estará trabajando con los microcontroladores PIC. El cual este será el encargado del procesamiento de la información, recabado y enviado de la información. 
 
11.- Circuito Integrado
inclusive si conocemos el uso debido de los sensores, con el fin de construir un circuito con múltiples sensores es necesario la implementación de un diagrama a bloques, acorde a lo que se necesite, donde se muestre las características del circuito y brinde la opción de conocer los componentes con lo que cuenta.
 
Figura 12.- Diagrama a bloques.
Las conexiones de los sensores y módulos, como el sensor DHT11, LM35 y YC-28, son similares cada uno lleva una conexión hacia la fuente de alimentación y envían su información hacia el PIC, el cual recibe la información y la transmite hacia la pantalla oled para ser visualizada y hacia el módulo USART que la transmite hacia una computadora. El bloque llamado “Ambiente Grafico” radica en el uso de la información una vez dentro de una computadora, pues esa es almacenada en una página web para su visualización posterior a todo el público. El PIC puede realizar diversas funciones dependiendo de las condiciones que se apliquen, es decir, cuando los niveles en las lecturas son elevados pasando hacia el bloque denominado como “puente H”, este se encarga de encender una alarma, un extractor y una bomba dependiendo del tipo de lectura. Este tipo de funciones de “emergencia” son alimentados de manera externa al circuito como tal, usando corriente alterna para alimentar aparatos con alto consumo de energía, para ello se utilizará un relevador para utilizar los pulsos del PIC y controlar el encendido y apagado de estos aparatos. El cual estará armado en un módulo separado de la PCB general al tener una placa de relevadores unidos.
CO2
La presencia de las plantas en un ambiente cerrado, en específico, la fotosíntesis, puede derivar en un exceso de CO2, lo cual es perjudicial para los cultivos. Para analizar el CO2 presente en el invernadero fue necesario el uso de un medidor de calidad del aire implementado dentro del sistema indebido, los sensores candidatos para este trabajo fueron los sensores CCS811 y el sensor MQ-135, que pesar de no ser exclusivamente de CO2 pueden detectar este y otros gases extra como el gas metano, alcohol, amoniaco, etc.
El MQ-135 se basa en un material semiconductor de óxido de estaño (SnO₂), cuya resistencia cambia al entrar en contacto con ciertos gases. 
 
Figura 13.- Estructura del sensor
Cada módulo MQ tiene un escalado similar a los demás, es decir, Al obtener los valores del sensor y queremos implementarlos se debe realizar un escalado a los valores leídos haciendo una relación entre la lectura analógica y la real no lineal. 
 
Figura 14.- Escaldo de los valores
La fórmula necesaria para el uso de este sensor 
Vsensor=  (Lectura ADC×Vref)/Resolución ADC 
 Vsensor = Voltaje de salida del sensor
Lectura ADC = Valor digital leído por el microcontrolador
Vref = Voltaje de referencia del ADC (normalmente 5V o 3.3V)
Resolución ADC = Número máximo del ADC (1023 para un ADC de 10 bits)
 
Figura 15.- Curvas de datos en mediciones
Módulo Xbee 
Durante este cuatrimestre se llevó a cabo el desarrollo de un sistema de comunicación inalámbrica utilizando dos módulos Xbee, los cuales se configuraron mediante adaptadores USB para establecer la conexión entre ellos. El proceso de configuración se realizó utilizando el software XCTU, herramienta que permite gestionar y programar los módulos Xbee de manera eficiente. En este proceso, uno de los módulos se configuró como transmisor y el otro como receptor, permitiendo así la transmisión y recepción de datos de manera bidireccional. 
 figura 16.- Intercambio de datos por Xbee
Para llevar a cabo esta configuración, se conectaron los módulos Xbee a computadoras a través de puertos USB, operando en modo serial. A través del software XCTU, se ajustó el firmware de los módulos, lo que posibilitó la correcta comunicación entre ambos dispositivos. Este ajuste es crucial para garantizar que los módulos pudieran intercambiar datos sin problemas, asegurando su correcto funcionamiento dentro de las distancias y condiciones esperadas.
Resultados
La manera de evitar un corto circuito o quemar algún componente durante las pruebas, es realizando una simulación del mismo circuito en algún software de simulación en este caso, “Proteus” a continuación se mostrarán las conexiones del diagrama esquemático del circuito.
  Figura 17. Simulación del circuito
Al verificar el funcionamiento correcto en la simulación pasaremos a las pruebas físicas, armando el circuito en una ProtoBoard y realizar observaciones sobre las acciones del mismo circuito, haciendo uso de corriente directa (DC).
 
Figura 18. Prueba física de funcionamiento
 Inmediatamente en estas pruebas de funcionamiento, se deberán comprobar las acciones realizadas por el PIC al cambio de variables en las mediciones de los sensores, como se mostrará en la siguiente imagen.
 
Figura 19. Cambio de variables en prueba de funcionamiento. 
Al tener un funcionamiento cercano al deseado, las pruebas pasan por un cambio de voltaje, cambiando entre corriente directa hacia corriente alterna, donde se reemplazarán componentes, como Leds, resistencias, etc. En la siguiente imagen se mostrarán los cambios ya hechos en el circuito integrado.
 
Figura 20. Cambio de voltaje, AC. 
Tras realizar dichos cambios se deberá comprobar nuevamente su correcto funcionamiento mostrados en la siguiente imagen.
 
Figura 21. Buen funcionamiento con corriente Alterna.
Mediante el uso del módulo USART el circuito se conectará hacia una computadora, donde el código ingresado mandará los datos de los sensores a través de un puerto COM y al mismo tiempo guardando sus datos en un archivo de texto como se mostrará a continuación en la siguiente imagen.
 
Figura 22. Almacenamiento de datos
Una vez que el circuito haga lo esperamos, sabremos que las conexiones esquemáticas están en orden y se podrá pasar al armado de la PCB, esto se iniciara con el diagrama en 2D para realizar las conexiones de los Footprint. En la siguiente imagen se mostrará el diagrama terminado.
 
Figura 23. Diagrama 2D del circuito
Una vez construido el esquemático como el que se muestra en la figura 11 se podrá visualizar el modo 3D de la placa PCB para visualizar como se vería en físico.
 
Figura 24. Placa PCB modelo 3D
El siguiente paso será le planchado de la placaba base, al exportarse en PDF el documento puede imprimirse en papel transfer para facilitar ser pegado en una PCB mediante el planchado.
  
Figura 25. Planchado de la placa base.
Cuando es terminado de planchar, el diseño queda pegado a la PCB, aquí deberá ser puesto en cloruro férrico para disolver los excedentes de cobre, dejando únicamente las pistas.
 
Figura 26. PCB en acido férrico
Cuando se terminan de disolver, estará listo para la perforación de las terminales, donde irán los componentes y posteriormente su soldado como se verá en la siguiente imagen.
 
Figura 27. Perforación y posterior soldadura 
Al contar con nuestra placa de circuito impreso de manera física pasaremos a la sección de pruebas dónde se verificará que el circuito funcione de manera correcta y no existe ningún error.
XBEE
Durante la realización de las pruebas restantes se implementó, un sistema de comunicación basado en Xbee, el cual demostró tener un alcance aproximado de 90 metros en entornos cerrados, lo cual es adecuado para aplicaciones que requieren comunicación dentro de edificios o estructuras con obstáculos. En espacios abiertos, el alcance se amplió significativamente, llegando a alcanzar hasta 3200 metros, lo que hace que este sistema sea adecuado para aplicaciones al aire libre, donde no hay interferencias físicas significativas.
 
Figura 22. Prueba de envío y recepción de mensajes con módulos Xbee. 
Como se observa en la figura 18 se realizaron las pruebas de envió de información de manera inalámbrica implementado los módulos Xbee. Esta comunicación fue solamente un emisor y receptor, posteriormente se pretende ampliar la topología.
6. Conclusiones 
En las etapas iniciales, el proyecto se enfocó en integrar sensores de temperatura, humedad ambiental y humedad de la tierra en un único circuito electrónico capaz de mostrar las variables en una pantalla OLED y enviar datos a una PC mediante el protocolo de comunicación USART. Este proceso requirió múltiples actividades, como la validación de sensores, la construcción de circuitos y cálculos de errores, garantizando la fiabilidad del sistema. Actualmente, el proyecto ha evolucionado más allá del monitoreo, incorporando funcionalidades que permiten la interacción dinámica con el entorno. Por ejemplo, ahora es posible activar un ventilador cuando se detectan altas temperaturas, lo que amplía las aplicaciones prácticas del sistema. Además, se trabaja en una interfaz de monitoreo remoto accesible y económica, desarrollada en software libre, lo que mejora su portabilidad y reduce costos.
7. Agradecimientos 
Los autores desean expresar su agradecimiento a la Ingeniería en Redes y Telecomunicaciones, al Dr. Juan Israel Yáñez Vargas y al M.C. Víctor Lauro Pérez García, conocimiento quienes, y apoyo, con han su valioso contribuido significativamente al desarrollo y financiamiento de este proyecto.
8. Referencias 
¿Qué es XBee? XBee.cl – Comunicación Inalámbrica para Tus Proyectos. (2019, Noviembre 29). XBee.cl – Comunicación Inalámbrica Para Tus Proyectos. https://xbee.cl/que-es-xbee/
 Farooq, M. S., Javid, R., Riaz, S., & Atal, Z. (2022). IoT Based Smart Greenhouse Framework and Control Strategies for Sustainable Agriculture. IEEE Access, 10, 99394-99420. https://doi.org/10.1109/access.2022.3204066
M. S. Farooq, S. Riaz, M. A. Helou, F. S. Khan, A. Abid and A. Alvi, "Internet of Things in Greenhouse Agriculture: A Survey on Enabling Technologies, Applications, and Protocols," in IEEE Access, vol. 10, pp. 53374-53397, 2022, doi: 10.1109/ACCESS.2022.3166634. C, S. (2022c).
 Conversión Automático Análogo/Digital (A/D). Control Educación. https://controlautomaticoeducacion.com/microc ontroladores-pic/14-conversion-analogodigital- ad/ Jecrespom. (2018, 16 noviembre).
 Xbee – Aprendiendo Arduino. Aprendiendo Arduino. https://aprendiendoarduino.wordpress.com/cate gory/xbee/ https://blogagricultura.com/estadisticas- agricolas-estado-guanajuato/
 Breijo, E. (2012). Compilador C CCS y García Simulador Proteus para Microcontroladores PIC. España: Marcombo.
