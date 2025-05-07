UNIVERSIDAD POLITECNICA DE  ́

JUVENTINO ROSAS

KATSI Hardware

Presenta:

Cristian Jesus Ortiz Pineda  ́
Ramses Alejandro Ramos Guerrero
Daniel Castro Reyes

Asesor:

Dr. Juan Israel Yanez Vargas  ̃

Co-Asesor:

M.C. V ́ıctor Lauro Perez Garc  ́  ́ıa

Santa Cruz de Juventino Rosas, Gto.5 de diciembre de 2024.

Contenido

Contenido i
Lista de figuras viii
Lista de tablas xi
1 Introduccion ́ 1
1.1. Motivacion ́ . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 1
1.2. Planteamiento del problema. . . . . . . . . . . . . . . . . . . . . . . . 2
1.3. Justificacion ́ . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 2
1.4. Objetivo General . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 2
1.5. Objetivos particulares . . . . . . . . . . . . . . . . . . . . . . . . . . . 3
1.6. Antecedentes . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 3
2 Marco teorico  ́ 7
2.1. Hardware . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 7
2.2. Analisis FODA Mayo Agosto 2024  ́ . . . . . . . . . . . . . . . . . . . . 11
2.2.1. FORTALEZAS: . . . . . . . . . . . . . . . . . . . . . . . . . 11
2.2.2. OPORTUNIDADES: . . . . . . . . . . . . . . . . . . . . . . . 11
2.2.3. DEBILIDADES: . . . . . . . . . . . . . . . . . . . . . . . . . 12
2.2.4. AMENAZAS: . . . . . . . . . . . . . . . . . . . . . . . . . . 12
2.3. Analisis FODA Septiembre Diciembre 2024  ́ . . . . . . . . . . . . . . . 13
2.3.1. FORTALEZAS: . . . . . . . . . . . . . . . . . . . . . . . . . 13
2.3.2. OPORTUNIDADES: . . . . . . . . . . . . . . . . . . . . . . . 13
2.4. DEBILIDADES: . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 13
2.5. AMENAZAS: . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 14
3 Desarrollo 15
3.1. Diagrama de trabajo . . . . . . . . . . . . . . . . . . . . . . . . . . . . 15
3.1.1. Identificar Sensor . . . . . . . . . . . . . . . . . . . . . . . . . 15
3.1.2. Desarrollar codigo  ́ . . . . . . . . . . . . . . . . . . . . . . . . 16

i

ii CONTENIDO

3.1.3. Cargar codigo  ́ . . . . . . . . . . . . . . . . . . . . . . . . . . . 16
3.1.4. Analizar datos . . . . . . . . . . . . . . . . . . . . . . . . . . 16
3.1.5. Almacenar/Transmitir Datos . . . . . . . . . . . . . . . . . . . 16
3.1.6. Pruebas y ajustes . . . . . . . . . . . . . . . . . . . . . . . . . 16
3.2. Memoria RAM y ROM utilizada . . . . . . . . . . . . . . . . . . . . . 16
3.3. Protocolo de Comunicacion ́ . . . . . . . . . . . . . . . . . . . . . . . 17
3.3.1. USART . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 17
3.4. Hardware . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 19
3.4.1. Visualizacion de datos dentro de una pantalla OLED  ́ . . . . . . 20
3.4.2. Modulacion por ancho de pulso  ́ . . . . . . . . . . . . . . . . . 21
3.4.3. DHT11 . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 21
3.4.4. DHT11 . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 22
3.4.5. Sensor de Tierra . . . . . . . . . . . . . . . . . . . . . . . . . 23
3.4.6. USART LM35 . . . . . . . . . . . . . . . . . . . . . . . . . . 23
3.4.7. Implementacion de Circuitos  ́ . . . . . . . . . . . . . . . . . . . 24
3.4.8. Hola Mundo en Hardware . . . . . . . . . . . . . . . . . . . . 25
3.4.9. Sensor de temperatura LM35 . . . . . . . . . . . . . . . . . . . 26
3.4.10. Sensor de tierra . . . . . . . . . . . . . . . . . . . . . . . . . . 26
3.4.11. Sensor DHT11 . . . . . . . . . . . . . . . . . . . . . . . . . . 27
3.4.12. Compilacion de Circuitos  ́ . . . . . . . . . . . . . . . . . . . . 27
3.4.13. USART . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 28
3.5. Propuesta . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 31
3.5.1. Explicacion ́ . . . . . . . . . . . . . . . . . . . . . . . . . . . . 31
3.6. Desarrollo del codigo  ́ . . . . . . . . . . . . . . . . . . . . . . . . . . . 33
3.6.1. Simulacion del circuito en el software de proteus  ́ . . . . . . . . 36
3.6.2. Circuito construido f ́ısicamente . . . . . . . . . . . . . . . . . 38
3.6.3. Pruebas de mediciones con el circuito en protoboard . . . . . . 39
4 Resultados 43
4.1. Resultados hardware . . . . . . . . . . . . . . . . . . . . . . . . . . . 43
4.2. Tabla con los valores de la temperatura obtenida mediante el sensor LM35 43
4.3. Grafica con los valores de la temperatura obtenida mediante el sensor  ́
LM35 . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 44
4.4. Tabla con los valores de la temperatura obtenida mediante el sensor
DHT-11 . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 44
4.5. Grafica con los valores de la temperatura obtenida mediante el sensor  ́
DHT-11 . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 45
4.6. Tabla con los valores de la humedad obtenida mediante el sensor DHT-11 45
4.7. Grafica con los valores de la humedad obtenida mediante el sensor DHT-11  ́ 46
4.8. Tabla con los valores de la temperatura obtenida mediante el multimetro 46
4.9. Grafica con los valores de la temperatura obtenida mediante el sensor  ́
DHT-11 . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 47

CONTENIDO iii

4.10. Grafica de promedios del registro de temperatura de cada sensor  ́ . . . . 47
4.10.1. Modificado . . . . . . . . . . . . . . . . . . . . . . . . . . . . 48
4.10.2. Modulo Xbee  ́ . . . . . . . . . . . . . . . . . . . . . . . . . . 49
4.10.3. Pruebas y resultados . . . . . . . . . . . . . . . . . . . . . . . 49
5 Actividades realizadas en los cuatrimestres anteriores 59
5.1. Septiembre diciembre 2023. . . . . . . . . . . . . . . . . . . . . . . . 59
5.2. Enero abril 2024. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 60
5.3. Mayo agosto 2024. . . . . . . . . . . . . . . . . . . . . . . . . . . . . 60
5.4. Actividades a realizar en los proximos cuatrimestres  ́ . . . . . . . . . . . 61
5.5. Septimo cuatrimestre.  ́ . . . . . . . . . . . . . . . . . . . . . . . . . . . 61
5.6. Octavo cuatrimestre. . . . . . . . . . . . . . . . . . . . . . . . . . . . 61
5.7. Noveno cuatrimestre. . . . . . . . . . . . . . . . . . . . . . . . . . . . 62
5.8. Actividades que se estan realizando . . . . . . . . . . . . . . . . . . . 63
5.9. Circuito inicial . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 63
5.10. Demostracion de variables en el circuito  ́ . . . . . . . . . . . . . . . . . 63
5.11. Mediciones de humedad . . . . . . . . . . . . . . . . . . . . . . . . . 64
5.12. Subtema de transferencia de archivos . . . . . . . . . . . . . . . . . . . 68
5.13. Cronograma de actividades . . . . . . . . . . . . . . . . . . . . . . . . 69
6 Conclusion ́ 71
6.1. Trabajo a Futuro . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 72
Bibliograf ́ıa 73

Resumen

El presente documento es expuesto con el objetivo de dar a conocer la idea
principal del proyecto KATSIs en el cual se tomaran bases del proyecto RIO para su  ́
desarrollo y evolucion con el fin de mejorar en el  ́ ambito de software para crear un  ́

ambiente digital que sea amigable y accesible para la consulta de datos del adminis-
trador. El proyecto se enfoca en disenar y desarrollar una interfaz de visualizaci  ̃ on,  ́

procesamiento, control y almacenamiento de datos de tipo texto y figura, recolecta-
dos y obtenidos por medio de sensores que seran usados en el  ́ ambito de hardware  ́

en el prototipo de uso para el invernadero, estos sensores realizaran un monitoreo
para la evolucion de la flora existente, con ayuda de c  ́ amaras en el procesamiento  ́
de imagenes sobre los cambios en las plantas, los datos ser  ́ an recopilados y alma-  ́
cenados en una base de datos que tendra una vinculaci  ́ on con la interfaz.  ́

El control y registro sobre el crecimiento de la produccion y control de riego, as  ́  ́ı co-
mo examinar si existe presencia de plaga para efectuar una solucion o tomar control  ́

de la situacion, las cuales estar  ́ an dentro de las variantes y datos almacenados  ́
en la base de datos, de esta forma, se tendra un control de la producci  ́ on, ya que  ́
se estara monitoreando continuamente y observando su desarrollo, guiando a una  ́
alternativa para una produccion con mejores resultados.  ́

v

Abstract

This document is presented with the objective of presenting the main idea of

the KATSIs project in which the bases of the RIO project will be taken for its de-
velopment and evolution in order to improve in the software field to create a digital

environment that is friendly and accessible for the consultation of the administrator’s
data. The project focuses on designing and developing an interface for visualization,

processing, control and storage of text and figure data, collected and obtained th-
rough sensors that will be used in the field of hardware in the prototype for use in the

greenhouse, these sensors will monitor the evolution of the existing flora, with the
help of cameras in the processing of images of changes in plants, the data will be
collected and stored in a database that will have a link with the interface.
The control and registration on the growth of production and irrigation control, as well

as examining whether there is the presence of pests to make a solution or take con-
trol of the situation, which will be within the variants and data stored in the database,

in this way, there will be a control of production, as it will be continuously monitored
and observing its development, guiding an alternative for a production with better
results.

vii

Lista de figuras

1.1. Diagrama de motivacion del proyecto  ́ . . . . . . . . . . . . . . . . . . . . 1
1.2. Tarjeta electronica  ́ . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 4
1.3. Esquema de circuito . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 5
1.4. Colaboration point . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 6
2.1. Ejemplo de PIC16f877A . . . . . . . . . . . . . . . . . . . . . . . . . . . 7
2.2. Oscilador De Cristal . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 8
2.3. Termistor . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 8
2.4. Tipos de Pantallas Oled . . . . . . . . . . . . . . . . . . . . . . . . . . . . 9
2.5. Representacion de un sensor  ́ . . . . . . . . . . . . . . . . . . . . . . . . . 10
2.6. Ejemplo de Transductor . . . . . . . . . . . . . . . . . . . . . . . . . . . . 11
3.1. Diagrama de flujos del codigo hola mundo  ́ . . . . . . . . . . . . . . . . . . 15
3.2. Grafico del almacenamiento Utilizado . . . . . . . . . . . . . . . . . . . . 17
3.3. Conexion Serial con Modulo USART . . . . . . . . . . . . . . . . . . . . 18
3.4. Sensor para la Temperatura del ambiente . . . . . . . . . . . . . . . . . . . 19
3.5. Sensor para la Humedad en la Tierra . . . . . . . . . . . . . . . . . . . . . 20
3.6. Primera simulacion de una pantalla oled . . . . . . . . . . . . . . . . . . . 21
3.7. Simulacion de pwm en proteus  ́ . . . . . . . . . . . . . . . . . . . . . . . . 21
3.8. Tercera simulacion en proteus mostrando los valores del sensor DHT11 . . 22
3.9. Simulacion en Proteus mostrando los valores del sensor LM35 . . . . . . . 23
3.10. Simulacion de los valores obtenidos por el Sensor de Tierra  ́ . . . . . . . . . 23
3.11. Simulacion mostrando en maquina virtual los valores de un sensor LM35  ́ . 24
3.12. Simulacion donde se mostrar  ́ a una uni  ́ on de varios sensores en una pantalla  ́
OLED . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 25
3.13. Circuito Fisico del Hola Mundo en pantalla OLED . . . . . . . . . . . . . 26
3.14. circuito f ́ısico del Sensor LM35 . . . . . . . . . . . . . . . . . . . . . . . 26
3.15. Sensor de Tierra implementado de forma fisica . . . . . . . . . . . . . . . 27
3.16. Sensor de humedad y temperatura construido de forma fisica . . . . . . . . 27
3.17. Circuito f ́ısico que usa una variedad de sensores . . . . . . . . . . . . . . . 28

viii

LISTA DE FIGURAS ix

3.18. Circuito en fisico de la conexion USART . . . . . . . . . . . . . . . . . . . 28
3.19. Mediciones de sensores de temperatura del ambiente . . . . . . . . . . . . 29
3.20. Graficas realizadas con los valores obtenidos del sensor DHT-11 . . . . . . 29
3.21. Graficas realizadas con los valores obtenidos del sensor DHT-22 . . . . . . 30
3.22. Graficas realizadas con los valores obtenidos del sensor LM35 . . . . . . . 30
3.23. Graficas realizadas con los valores obtenidos con el mult ́ımetro . . . . . . . 30
3.24. Diagrama de bloques . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 31
3.25. Diagrama de flujo . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 33
3.26. Continuidad del diagrama de flujo . . . . . . . . . . . . . . . . . . . . . . 34
3.27. Circuito construido en el software de proteus . . . . . . . . . . . . . . . . 36
3.28. Circuito funcionando en el software de proteus . . . . . . . . . . . . . . . 37
3.29. Disminucion de la temperatura en el sensor LM35  ́ . . . . . . . . . . . . . . 37
3.30. Mensaje de error ya que no se encuentra conectado el sensor . . . . . . . . 38
3.31. Circuito recreado en protoboard . . . . . . . . . . . . . . . . . . . . . . . 38
3.32. Pruebas de mediciones dentro del invernadero . . . . . . . . . . . . . . . . 39
3.33. Horario con mayor temperatura dentro del invernadero . . . . . . . . . . . 39
3.34. Pruebas de medicion de temperatura en disntintos puntos de la universidad.  ́ 40
3.35. Pruebas de medicion de temperatura en disntintos puntos de la universidad  ́ . 40
3.36. Metodo de planchado en PCB  ́ . . . . . . . . . . . . . . . . . . . . . . . . 41
3.37. Metodo de planchado en PCB  ́ . . . . . . . . . . . . . . . . . . . . . . . . 42
4.1. Datos de la temperatura registrada con el sensor LM35 durante los 5 d ́ıas de
la semana. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 43
4.2. Grafica de la temperatura registrada con el sensor LM35 durante los 5 d  ́  ́ıas
de la semana. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 44
4.3. Datos de la temperatura registrada con el sensor DHT-11 durante los 5 d ́ıas
de la semana. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 44
4.4. Grafica de la temperatura registrada con el sensor DHT-11 durante los 5 d  ́  ́ıas
de la semana. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 45
4.5. Datos de la humedad registrada con el sensor DHT-11 durante los 5 d ́ıas de
la semana. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 45
4.6. Grafica de la humedad registrada con el sensor DHT-11 durante los 5 d  ́  ́ıas de
la semana. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 46
4.7. Datos de la temperatura registrada con el multimetro durante los 5 d ́ıas de la
semana. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 46
4.8. Grafica de la temperatura registrada con el multimetro durante los 5 d  ́  ́ıas de
la semana. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 47
4.9. Grafica del promedio de las temperaturas del sensor LM35, DHT-11 y mul-  ́
timetro . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 48
4.10. Grafica de errores de los sensores con respecto al multimetro  ́ . . . . . . . . 48
4.11. Interfaz Digi XCTU . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 49
4.12. Simulacion del circuito  ́ . . . . . . . . . . . . . . . . . . . . . . . . . . . . 50

x LISTA DE FIGURAS

4.13. Prueba f ́ısica de funcionamiento . . . . . . . . . . . . . . . . . . . . . . . 50
4.14. Cambio de variables en prueba de funcionamiento. . . . . . . . . . . . . . 51
4.15. Cambio de voltaje, AC. . . . . . . . . . . . . . . . . . . . . . . . . . . . . 51
4.16. Buen funcionamiento con corriente Alterna. . . . . . . . . . . . . . . . . . 52
4.17. Almacenamiento de datos . . . . . . . . . . . . . . . . . . . . . . . . . . . 52
4.18. Diagrama 2D del circuito . . . . . . . . . . . . . . . . . . . . . . . . . . . 53
4.19. Placa PCB modelo 3D . . . . . . . . . . . . . . . . . . . . . . . . . . . . 54
4.20. Planchado de la placa base . . . . . . . . . . . . . . . . . . . . . . . . . . 55
4.21. PCB en acido ferrico  ́ . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 56
4.22. . Perforacion y posterior soldadura  ́ . . . . . . . . . . . . . . . . . . . . . . 56
4.23. Prueba de env ́ıo y recepcion de mensajes con m  ́ odulos Xbee.  ́ . . . . . . . . 57
5.1. Funcionamiento inicial del circuito . . . . . . . . . . . . . . . . . . . . . . 63
5.2. Demostracion de variables  ́ . . . . . . . . . . . . . . . . . . . . . . . . . . 63
5.3. Pruebas de medicion de humedad  ́ . . . . . . . . . . . . . . . . . . . . . . . 64
5.4. Visualizacion de mensaje inicial  ́ . . . . . . . . . . . . . . . . . . . . . . . 64
5.5. Sensor de puesta a tierra . . . . . . . . . . . . . . . . . . . . . . . . . . . 65
5.6. Pruebas de humedad con vasos de agua . . . . . . . . . . . . . . . . . . . 65
5.7. Realizando pruebas de humedad . . . . . . . . . . . . . . . . . . . . . . . 66
5.8. Visualizacion de humedad en pantalla Oled  ́ . . . . . . . . . . . . . . . . . 67
5.9. Endendido de diodo led simulando el encendido de un foco . . . . . . . . . 68
5.10. Registros de temperatura almacenado en un archivo txt . . . . . . . . . . . 69

Lista de tablas

xi

Cap ́ıtulo 1

Introduccion
 ́

En este cap ́ıtulo seran agregados los antecedentes de proyectos similares a un inver-  ́
nadero, la definicion de problema consiste en mostrar los motivos del porqu  ́ e la situaci  ́ on ́
amerita a tener una solucion, justificaci  ́ on el porqu  ́ e se har  ́ a algo al respecto. Por  ́ ultimo,  ́
los objetivos generales y espec ́ıficos, que detallaran las metas que se buscan alcanzar
para el presente cuatrimestre.

1.1. Motivacion ́

Figura 1.1: Diagrama de motivacion del proyecto  ́

En la figura 1.1 se realiza una descripcion gr  ́ afica de la motivaci  ́ on y meta a seguir,  ́
este proyecto se enfoca en ayudar a la sociedad, en buscar un bien comun y facilitar  ́

1

2 CAP ́ITULO 1. INTRODUCCION ́

labores con un sistema de monitoreo, control y adquisicion de informaci  ́ on de un inver-  ́
nadero, mas contar con una interfaz tecnol  ́ ogica f  ́ acil de usar y controlar para cualquier  ́
usuario que la adquiera.
Representa la busqueda de objetivos y puntos a lograr partiendo desde el interior  ́
del invernadero, lugar que se espera lograr que pueda ser monitoreado por un usuario a
distancia, a traves de las mediciones y valores que proporcionen los sensores utilizados  ́
hacia la interfaz donde el usuario puede visualizar estos valores. A partir de modulos  ́
XBEE se transmitiran las mediciones de los sensores, est  ́ as podr  ́ an ser visualizadas a  ́
traves de la interfaz y adem  ́ as de lograr almacenar las variables dentro de una base de  ́
datos que pueda mostrar los datos almacenados a traves de la interfaz en modo de datos  ́
y estad ́ısticas y a partir de esto llevar un seguimiento del interior del invernadero.

1.2. Planteamiento del problema.

¿La perdida y desperdicio de agua en cultivos de invernaderos podr ́ıa evitarse crean-
do un sistema de automatizacion, medici  ́ on, an  ́ alisis y control que pueda administrarse y  ́

en cual se pueda consultar informacion que sea almacenada en una interfaz desarrollada  ́
en python?.

1.3. Justificacion ́
Al implementar el proyecto se busca encontrar una solucion y apoyo al problema de  ́
desperdicio de agua en el riego de cultivos en invernaderos, en donde la implementacion ́
de hardware propone realizar un sistema automatizado de riego mediante la recopilacion ́
de datos de sensores de humedad, temperatura y PH, y todos los datos sean almacenados

en una interfaz desarrollada en python por el equipo que busque generar la automati-
zacion de invernaderos a un nivel m  ́ as accesible para un usuario o administrador que  ́

busque consultar y monitorear los cambios y datos almacenados de cada cierto tiempo.

1.4. Objetivo General
Disenar y desarrollar un sistema embebido para adquisici  ̃ on, monitoreo, control y  ́
envuo a distancia de datos de invernadero y sean visualizados en una interfaz desarrolla-  ́
da en python para el procesamiento, control y almacenamiento de datos.

1.5. OBJETIVOS PARTICULARES 3

1.5. Objetivos particulares
Realizar un analisis de requerimientos a partir del uso del sistema de adquisici  ́ on ́
de datos.

Diseno de una interfaz para la visualizaci  ̃ on, procesamiento, control y almacena-  ́
miento de datos.

Desarrollo de la interfaz 1.0 de visualizacion de datos de invernadero.  ́

Creacion de la base datos 1.0 de almacenamiento de informaci  ́ on en MySQL.  ́
Diseno de un sistema embebido para la adquisici  ̃ on, monitoreo, control y env  ́  ́ıo a
distancia de datos. (Topolog ́ıa)

Desarrollo de un sistema de control de invernadero a partir de un sensor de hume-
dad del suelo y del ambiente.

1.6. Antecedentes
Proyecto: RIO
El desperdicio de agua en los ultimos a  ́ nos en el mundo ha ido aumentando de manera  ̃
drastica, tal es el caso de los sistemas de riego de los diferentes cultivos que existen  ́
ademas de las m  ́ ultiples condiciones en donde estos est  ́ an operando ya sea a campo  ́
abierto o en un invernadero. El 70 % de agua que se utiliza en Mexico es destinada a la  ́
agricultura donde el 60 % de esta agua destinada es desperdiciada por los sistemas de
riego ya sea por la infiltracion o evaporaci  ́ on.  ́
En Guanajuato la construccion de invernaderos a lo largo y ancho del estado es muy  ́
comun con diferentes cultivos. En la referencia [  ́ ?] se describe un proyecto en el que

su principal objetivo es disminuir el consumo de agua en los sistemas de riego, as ́ı co-
mo, reducir costos de operacion de estos, para lograr la meta se construir  ́ a un sistema  ́

embebido empleando microcontroladores, los cuales mediran temperatura del inverna-  ́
dero en diferentes puntos y a traves de radiofrecuencias se creara una red multipunto  ́
implementando modulos xbee donde la cual las temperaturas obtenidas ser  ́ an enviadas  ́
a un dispositivo central el cual procesara la informaci  ́ on y activar  ́ a el riego de forma  ́
automatica.  ́
Para lograr esto se emplearan t  ́ ecnicas como comunicaci  ́ on serial, conversi  ́ on an  ́ alogo-  ́
digital, multiplexacion, demultiplexaci  ́ on.  ́

4 CAP ́ITULO 1. INTRODUCCION ́

En la figura 1.2 se muestra el diseno de la tarjeta electr  ̃ onica desarrollada en este  ́
proyecto.
El art ́ıculo describe el diseno y desarrollo de una Interfaz Gr  ̃ afica de Usuario a trav  ́ es ́
del software de instrumentacion virtual NI LabVIEW mediante la funci  ́ on VISA, para  ́
visualizar graficamente y almacenar los datos de las variables climatol  ́ ogicas de tempe-  ́
ratura y la humedad relativa. La interfaz grafica ofrece la opci  ́ on de exportar la fecha,  ́
hora y los datos de las dos variables a documentos de texto con extension ?.txt?, la cual  ́
adquiere la informacion de una tarjeta electr  ́ onica de monitoreo y control inal  ́ ambrico,  ́

que utiliza como dispositivo principal un microcontrolador PIC16F877A en la adqui-
sicion de datos. Se utiliz  ́ o el sensor anal  ́ ogico de precisi  ́ on AMT1001 para sensar la  ́

temperatura y humedad relativa.

Figura 1.2: Tarjeta electronica  ́

El PIC16F877A se programo utilizando un lenguaje de programaci  ́ on en C en el  ́
compilador CCS Compiler, para realizacion de la adquisici  ́ on de datos, y enviarlos por  ́
comunicacion RS232 a la computadora, usando el m  ́ odulo PL2303 convertidor USB a  ́
TTL.
En trabajos a futuro se pretende monitorear el clima de un invernadero hort ́ıcola con
tecnolog ́ıa XBBE, para que los datos sean enviados en forma inalambrica a una compu-  ́
tadora conectada a Ethernet o WIFI, la cual tendra la interfaz gr  ́ afica de LabVIEW expli-  ́
cada en el presente art ́ıculo, y los datos sean mostrados/analizados a traves de internet.  ́
El diseno del circuito desarrollado en la tarjeta se muestra en la figura  ̃ 1.3.

1.6. ANTECEDENTES 5

Figura 1.3: Esquema de circuito

Articulo:HEMS-IoT: A Big Data and Machine Learning-Based Smart Home
System for Energy Saving
El art ́ıculo [?] demuestra que el IoT esta modificando los entornos vitales de los ciu-  ́
dadanos al pasar de un hogar tradicional a un inteligente. En los hogares inteligentes, las
personas pueden controlar, supervisar y gestionar el consumo de energ ́ıa en funcion de  ́
su estilo de vida.
En este art ́ıculo se presenta una revision de trabajos relacionados con iniciativas IoT  ́
para la eficiencia energetica en hogares inteligentes. Fue prestada especial atenci  ́ on a  ́
aquellas iniciativas que utilizan machine learning y big data. El IMS se disen ̃o con soft-  ́
ware y hardware de codigo abierto para poder extenderse en el contexto IoT.  ́
El sistema se probo servicios dom  ́ esticos inteligentes basados en IMS en dos esce-  ́
narios: un servicio domestico inteligente de atenci  ́ on sanitaria y un servicio de gesti  ́ on ́
de catastrofes. Adem  ́ as, introdujeron un protocolo de optimizaci  ́ on para WSN a trav  ́ es ́

de una arquitectura para un hogar inteligente, esta arquitectura se divide en dos entor-
nos, exterior e interior, que se comunican a traves de un punto de acceso. La casa del  ́

usuario puede ser controlada desde cualquier lugar y en cualquier momento mediante un
telefono inteligente.  ́
HEMS-IoT brinda a los residentes de hogares una expectativa mas significativa de  ́
consumo de energ ́ıa en sistemas inteligente hogares, porque recopila datos mas profun-  ́
dos a traves de su capa de servicio utilizando aprendizaje autom  ́ atico y big data tecno-  ́
log ́ıas.
En esta seccion fueron analizados los datos recopilados por HEMS-IoT durante el  ́
estudio de caso para identificar patrones de consumo de energ ́ıa y comprender las cir-

6 CAP ́ITULO 1. INTRODUCCION ́

cunstancias que fomentan dichos patrones. Ademas, se propuso una serie de acciones de  ́
ahorro energetico y fue presentado un enfoque centrado en el usuario.  ́

Internet of Things in Greenhouse Agriculture: A Survey on Enabling Techno-
logies, Applications, and Protocols

El invernadero es una de las formas sostenibles de agricultura inteligente, se consi-
dera como un metodo alternativo para superar la crisis alimentaria que se genera debido  ́

al elevado crecimiento demografico el cambio clim  ́ atico y la contaminaci  ́ on ambiental.  ́

La imagen 1.4 es una muestra de como el usuario puede utilizar un dispositivo inteligen-
te para controlar su hogar desde cualquier lugar y en cualquier momento.

Figura 1.4: Colaboration point

Enfocados en lo anteriormente visualizado en cada uno de los art ́ıculos se puede
destacar el uso y en algunos casos la falta de sistemas de almacenamiento de variables
y datos para un control organizado de informacion. Es por ello que la iniciativa de este  ́
proyecto pretende llevar a cabo mas all  ́ a de la idea de automatizar y facilitar el riego en  ́
invernaderos, poder ofrecerle a el administrador e incluso un perfil de usuario el cual
pueda tener ciertos privilegios como la consulta de datos de ciertas a areas o en ciertos  ́
ambitos del invernadero, accediendo mediante una interfaz gr  ́ afica a un perfil que le  ́
ofrezca un almacenamiento y muestra de datos guardados anteriormente. Ademas de esto  ́
poder proporcionar un facil y mejor control de una forma digital y a un f  ́ acil alcance del  ́
administrador que desee realizar cambios, actualizar, visualizar o consultar informacion ́
enviada o almacenada en la interfaz y en la base de datos, aunado al desarrollado del
hardware para todo el monitoreo, control y visualizacion, gener  ́ a un proyecto de valor y  ́
de gran futuro.

Cap ́ıtulo 2

Marco teorico  ́

2.1. Hardware
La presente seccion comprende la explicaci  ́ on de algunos elementos a utilizar para  ́
el desarrollo del hardware para monitoreo, analisis, envi  ́ o y control de datos de un inver-  ́
nadero.
MICROCONTROLADOR

Un Microcontrolador es un circuito integrado que incluye sistemas para controlar ele-
mentos de entrada/salida. Incluye un procesador y una memoria que puede guardar el

programa y sus variables (flash y RAM) para posteriormente ejecutar las instrucciones
almacenadas en su memoria. Su funcion es la de automatizar procesos y procesar infor-  ́
macion ́
PIC

El Programable Integrated Circuit (PIC) (Circuito Integrado Programable), es un dispo-
sitivo que controla las interrupciones que van al CPU 2.1.

Figura 2.1: Ejemplo de PIC16f877A

Modulos XBee  ́
XBee es el nombre comercial del Digi de una familia de modulos de comunicaci  ́ on por  ́

7

8 CAP ́ITULO 2. MARCO TEORICO  ́

radio y estan basados en el est  ́ andar zigbee, pero digi tiene muchos Xbee y algunos son  ́
zigbee estandar y otros son propietarios o modificaciones del est  ́ andar. Existen muchos  ́
modulos Xbee basados en el est  ́ andar IEEE 802.15.4  ́ ??.
Zigbee
Zigbee es el nombre de la especificacion de un conjunto de protocolos de alto nivel de co-  ́
municacion inal  ́ ambrica para su utilizaci  ́ on con radiodifusi  ́ on digital de bajo consumo,  ́
basada en el estandar IEEE 802.15.4 de redes inal  ́ ambricas de  ́ area personal (wireless  ́

personal area network, WPAN). Su objetivo son las aplicaciones que requieren comuni-
caciones seguras con baja tasa de env ́ıo de datos y maximizacion de la vida  ́ util de sus  ́

bater ́ıas.
ADC
Son dispositivos capaces de transformar una senal anal  ̃ ogica en una digital, de esta ma-  ́
nera permiten la transmision de informaci  ́ on de un dispositivo a otro.  ́
Oscilador de cristal
Un oscilador de cristal es un componente electronico que utiliza las propiedades pie-  ́
zo electricas de ciertos cristales para generar una se  ́ nal el  ̃ ectrica precisa y estable en  ́
terminos de frecuencia  ́ 2.2.

Figura 2.2: Oscilador De Cristal

Sistema embebido
Es un sistema de computacion dise  ́ nado para realizar funciones espec  ̃  ́ıficas, y cuyos
componentes se encuentran integrados en una placa base.
Termistor
Un termistor es un tipo de resistencia (componente electronico) cuyo valor var  ́  ́ıa en
funcion de la temperatura de una forma m  ́ as acusada que una resistencia com  ́ un ́ 2.3.

Figura 2.3: Termistor

2.1. HARDWARE 9

Pantalla OLED
La tecnolog ́ıa OLED (OLED significa diodo organico emisor de luz (OLED). Tambi  ́ en ́
se conoce como diodo electroluminiscente organico (EL).) la encontramos en televiso-  ́
res de gama alta. Se trata de pantallas de muy alta calidad, la mas alta del mercado. A  ́
diferencias de las pantallas LED o LCD, que usan la retroiluminacion general del panel  ́
de p ́ıxeles, estas pantallas cuentan con un diodo emisor de luz por cada p ́ıxel. Esto quiere
decir que cada p ́ıxel esta iluminado por separado, lo que otorga a este tipo de pantallas  ́
unas caracter ́ısticas unicas de color, de contraste y de brillo, hay algunos dipos de pan-  ́
tallas Oled como se mostrara a continuacion en la figura  ́ 2.4

Figura 2.4: Tipos de Pantallas Oled

I2C
I2C es un puerto y protocolo de comunicacion serial, define la trama de datos y las  ́
conexiones f ́ısicas para transferir bits entre 2 dispositivos digitales. El puerto incluye
dos cables de comunicacion, SDA y SCL. Adem  ́ as el protocolo permite conectar hasta  ́
127 dispositivos esclavos con esas dos l ́ıneas, con hasta velocidades de 100, 400 y 1000
kbits/s.
El protocolo I2C es uno de los mas utilizados para comunicarse con sensores digitales,  ́
ya que a diferencia del puerto Serial, su arquitectura permite tener una confirmacion de  ́
los datos recibidos.
Memoria RAM
La memoria RAM es la memoria principal de un dispositivo, esa donde se almacenan
de forma temporal los datos de los programas que estas utilizando en este momento. Sus  ́
siglas significan Random Access Memory, lo que traducido al espanol ser  ̃  ́ıa Memoria
de Acceso Aleatorio, y es un tipo de memoria que te puedes encontrar en cualquier
dispositivo, desde ordenadores de sobremesa hasta telefonos m  ́ oviles.  ́
Memoria ROM

10 CAP ́ITULO 2. MARCO TEORICO  ́

La ROM o memoria de solo lectura (de su acronimo en ingl  ́ es ?read-only memory?)  ́
es el medio de almacenamiento que se usa en los ordenadores y dispositivos electronicos  ́
cuya caracter ́ıstica diferencial es que unicamente tiene acceso de lectura, y no de escri-  ́
tura.
Esto significa que la ROM puede recuperar informacion, pero no modificarla ni inter-  ́
venir en ella, y su uso principal es el almacenamiento del firmware y demas contenidos  ́
usados para el correcto funcionamiento de los dispositivos.
La informacion almacenada en la ROM no se altera con el tiempo ni al apagar el  ́
dispositivo.
¿Que es un sensor?  ́
Un sensor es un dispositivo que esta capacitado para detectar acciones o est  ́  ́ımulos

externos y responder en consecuencia. Estos aparatos pueden transformar las magnitu-
des f ́ısicas o qu ́ımicas en magnitudes electricas [  ́ ?].

En la siguiente imagen se mostrara una representaci  ́ on grafica de la funci  ́ on de un  ́
sensor figura 2.5.

Figura 2.5: Representacion de un sensor  ́

¿Que es un transductor?  ́
Un transductor define como un dispositivo fundamental en el sistema de control de
medidores electricos. Actualmente, son muy utilizados en los sistemas de automatiza-  ́
cion y control para registrar grandes magnitudes. Y no s  ́ olo nos estamos refiriendo a las  ́
magnitudes mas conocidas como son: temperatura y presi  ́ on; tambi  ́ en sirven para regis-  ́
trar caudales o concentracion de gases [  ́ ?].
A continuacion se mostrar  ́ a un ejemplo del funcionamiento de un transductor  ́ 2.6.

2.2. ANALISIS FODA MAYO AGOSTO 2024  ́ 11

Figura 2.6: Ejemplo de Transductor

2.2. Analisis FODA Mayo Agosto 2024  ́
2.2.1. FORTALEZAS:
Proyecto con componentes economicos de f  ́ acil acceso.  ́
Optimiza la medicion de varios procesos dentro de un solo ambiente.  ́
Es sustentable ya que los elementos que se utilizan no danan al medio ambiente.  ̃
Maestros capacitados para la orientacion del proyecto.  ́
Apoyo emocional y moral por parte de docencia.
Acceso a variedad de libros, links y art ́ıculos espec ́ıficos del tema.
Conocimiento suficiente y creciente sobre los temas abordados
Automatizacion y control preciso: Al integrar sensores de temperatura y humedad.  ́
Analisis y Estad  ́  ́ısticas de Datos: La capacidad de almacenar datos y analizarlos
para generar estad ́ısticas. Ofrece informacion valiosa para la optimizaci  ́ on de la  ́
produccion y la reducci  ́ on de recursos innecesarios, como el uso excesivo de agua.  ́
2.2.2. OPORTUNIDADES:
Mantenimiento del invernadero de manera continua
Implementacion de materiales adicionales  ́
Aplicacion de productos agr  ́  ́ıcolas
Brinda conocimientos sobre electronica.  ́
Brinda experiencia sobre el cuidado y preservacion de invernaderos.  ́

12 CAP ́ITULO 2. MARCO TEORICO  ́

Expansion a Otros Par  ́ ametros Ambientales: Incluir sensores adicionales para otros  ́
parametros como CO2, luz, o pH del suelo. A  ́ nadir capacidades para monitorear y  ̃
controlar mas aspectos del ambiente del invernadero, aumentando la precisi  ́ on en  ́
la gestion de cultivos.  ́
2.2.3. DEBILIDADES:
Mucha competencia en el ambito de desarrollo.  ́
Complicaciones con los horarios de actividades academicas.  ́
Varaciones en el posicionamiento del sol y el clima.
Falta de tiempo.
Falta de personal en el equipo.
Carencia de trabajo en equipo
Dependencia de la Conectividad: La funcionalidad en tiempo real puede depender
de una conexion de estable. En  ́ areas con conectividad d  ́ ebil o inestable, la eficacia  ́
del sistema podr ́ıa verse comprometida.
2.2.4. AMENAZAS:
Plagas.
Cambios de temperatura.
Animales silvestres.
El personal de seguridad de la Universidad.
Ambiente peligroso.
Poca disponibilidad del area de trabajo (invernadero).  ́
Pocos integrantes en las tareas a desarrollar.
Fallas del Hardware: Los sensores, camaras o el hardware en general pueden fallar,  ́
afectando la operacion del invernadero. Podr  ́  ́ıa resultar en un monitoreo y control
incompletos, afectando la produccion y el bienestar de las plantas.  ́
Cambios en la Regulacion y Normativas: Nuevas regulaciones sobre el uso de  ́

tecnolog ́ıa en la agricultura pueden afectar el proyecto. Podr ́ıan requerirse modi-
ficaciones costosas o ajustes en el sistema para cumplir con nuevas normativas.

2.3. ANALISIS FODA SEPTIEMBRE DICIEMBRE 2024  ́ 13

2.3. Analisis FODA Septiembre Diciembre 2024  ́
2.3.1. FORTALEZAS:
Crecimiento en el area de la electr  ́ onica para futuros proyectos aplicados en inver-  ́
naderos sustentables.
Independencia en el desarrollo de las tarjetas electronicas para su libre patente.  ́

Adaptabilidad para cumplir con los requerimientos solicitados, dentro de los in-
vernaderos.

Calidad en el producto.
Crecimiento en el desarrollo de nuevas tecnolog ́ıas para la competitividad.
Aprendizaje practico en el  ́ ambito acad  ́ emico.  ́
Flexibilidad en el monitoreo de variables ambientales en invernaderos.
Optimizacion de recursos para su desarrollo.  ́
2.3.2. OPORTUNIDADES:
Crecimiento inteligente del sector agr ́ıcola y sostenible con el medio ambiente.
Comercializacion de productos tecnol  ́ ogicos a consumidores del sector agr  ́  ́ıcola.
Integracion con tecnolog  ́  ́ıas de control remoto.
Colaboracion con otros sectores.  ́
Aplicacion de energ  ́  ́ıas renovables para el suministro electrico.  ́
Aportaciones en el area agr  ́  ́ıcola para la solucion de futuras problem  ́ aticas.  ́
Expansion de cultivo hacia otros productos para el consumo humano.  ́
2.4. DEBILIDADES:
Limitaciones en el hardware en comparacion con otras tecnolog  ́  ́ıas.
Consumo de energ ́ıa con respecto a la aplicacion de nuevos componentes.  ́
Falta de precision en los sensores para la medici  ́ on de variables ambientes.  ́
Deficiencia en el mantenimiento del invernadero por falta de herramientas.
Falta de servicios debido a la ubicacion del invernadero.  ́

14 CAP ́ITULO 2. MARCO TEORICO  ́

Dificultas en la integracion de nuevos m  ́ odulos.  ́
Entorno desafiante en la programacion de los microcontroladores.  ́
2.5. AMENAZAS:
Entorno peligroso al encontrarse en una zona rural.
Fallas en los componentes y poca disponibilidad del material.
Condiciones climaticas extremas, as  ́  ́ı como bajas temperaturas.
Costos de implementacion al contar con un presupuesto limitado.  ́
Competencia en el ambito tecnol  ́ ogico.  ́
Propagacion de plagas dentro del invernadero.  ́
Dificultades en el uso y aplicacion para la persona que no est  ́ e capacitado.  ́

Cap ́ıtulo 3

Desarrollo

3.1. Diagrama de trabajo

Debido a la necesidad de formar y obtener experiencia manejando microcontrola-
dores es necesario una practica constante programando en ellos, para ello se mostrara  ́

a continuacion la estructura del diagrama a bloques que se utilizara para la creaci  ́ on e  ́
implementacion de c  ́ odigos, simulaciones y pruebas  ́ 3.1

Figura 3.1: Diagrama de flujos del codigo hola mundo  ́

Para comprobar la integridad y veracidad de este diagrama de flujo se simulo utili-
zando un software de simulacion conocido colocando cada componente especificado en  ́

el diagrama y trasladandolo a una simulaci  ́ on.  ́
3.1.1. Identificar Sensor
El bloque correspondiente a identificar el sensor corresponde a ver las descripciones
de los diferentes sensores y sus aplicaciones, en este apartado tambi  ́ en deben realizarse  ́

15

16 CAP ́ITULO 3. DESARROLLO

investigaciones del voltaje y corriente de trabajo, su implementacion y como se utiliza  ́
dentro del sistema.
3.1.2. Desarrollar codigo  ́
Una vez que fueron elegidos los sensores a utilizar, se debe desarrollar el codigo  ́
que corresponde a esos sensores, ya sea que se implemente en forma individual o en
conjunto, se debe incluso analizar el desarrollo del codigo para futuras implementaciones  ́
o union a otros c  ́ odigos. En est  ́ a subsecci  ́ on deben realizarse simulaciones en el software  ́
de diseno para identificar problemas en el c  ̃ odigo y en el momento del ensamble.  ́
3.1.3. Cargar codigo  ́
Una vez que fueron verificados los codigos y las simulaciones, deben de construirse  ́
los circuitos en f ́ısico, ya sea en protoboard o en placa fenolica, para que as  ́  ́ı mismo sean
cargados los codigos en el PIC designado.  ́
3.1.4. Analizar datos
El analisis de los datos corresponde a verificar si las mediciones son correctas o si  ́
toma las acciones correctas, uno de los detalles importantes para este presente bloque es
el uso de sistemas calibrados para comparar los resultados y as ́ı mejorar la precision y  ́
exactitud de la informacion.  ́
3.1.5. Almacenar/Transmitir Datos
En el presente apartado puede dividirse en dos partes, la primera puede definirse
como el almacenamiento de los datos in-sito o el envio de la informaci  ́ on de manera  ́
inalambrica a trav  ́ es del protocolo X-bee a una tarjeta en otra posici  ́ on m  ́ as lejana para  ́
su posterior almacenamiento y exhibicion.  ́
3.1.6. Pruebas y ajustes
Una vez que se tenga el almacenamiento de los datos y exhibicion, se pueden rea-  ́
lizar ajustes a lo largo de todos los bloques, ya que es de suma importancia calibrar la
informacion para la mejora del propio proyecto.  ́
3.2. Memoria RAM y ROM utilizada
Debido a la misma naturaleza del proyecto, la necesidad del aprendizaje sobre la
programacion no es poca, al utilizar un hardware en especifico como lo son los micro-  ́
controladores PIC 16f877a es necesario utilizar un software que pueda programarlo, en
este caso se estara utilizando el software de programaci  ́ on ”PIC C Compiler”para poder  ́
darle las instrucciones requeridas para su uso especifico. Para adquirir mas experiencia

3.3. PROTOCOLO DE COMUNICACION ́ 17

y conocimiento en este entorno de programacion tan complejo como lo es C, el uso y  ́
programacion de c  ́ odigos es constante, en la siguiente imagen se podr  ́ a observar el cre-  ́
cimiento del uso de la memoria RAM y memoria ROM mediante la complejidad de los
codigos avanza.  ́

Figura 3.2: Grafico del almacenamiento Utilizado

3.3. Protocolo de Comunicacion ́
3.3.1. USART
El termino USART, viene de receptor transmisor s ́ıncrono as ́ıncrono universal.”
Es una forma de comunicacion entre dispositivos que tengan esta capacidad, donde  ́
los datos son enviados en grupos de 8 bits o de 9 bits pero de bit por bit, esto es en serie
por eso se dice que esta es una comunicacion serial.  ́
Con el modulo USART el microcontrolador puede comunicarse e intercambiar datos  ́
con el ordenador, con otros microcontroladores, etc.
Existen dos tipos de comunicacion USART  ́
Comunicacion as  ́  ́ıncrona: Uno de los hilo sera para la transmisi  ́ on de datos y el  ́
otro hilo sera para la recepci  ́ on de datos entre un dispositivo a otro, la transmisi  ́ on ́
y la recepcion puede ocurrir de forma simult  ́ anea.  ́ //
Comunicacion s  ́  ́ıncrona: Uno de los hilos sera utilizado tanto para la transmisi  ́ on ́
y la recepcion de datos por lo que la transmisi  ́ on no puede ser simult  ́ anea, el otro  ́
hilo sera utilizado para enviar la se  ́ nal de reloj de sincronizaci  ̃ on entre dispositivos.  ́
Una caracter ́ıstica sobre el protocolo USAR son los pines utilizados es este. Debido a la
naturaleza del envio serial se deben usar pines de env  ́  ́ıo y otro de recepcion, los cuales  ́

18 CAP ́ITULO 3. DESARROLLO

estaran presentes no solo en el modulo USART, si no, tambi  ́ en en el microcontrolador.  ́
Los pines de envio y recepci  ́ on se les da el nombre de TX y RX, sus pines respectivos  ́
suelen ser RC7 y RC6 y su cableado debera ser cruzado, es decir, el pin RX (recepci  ́ on)  ́
debe ir conectado al pin TX (Transmision) como se mostrara en la figura  ́ 3.3

Figura 3.3: Conexion Serial con Modulo USART

3.4. HARDWARE 19

3.4. Hardware
Utilizar un software de simulacion de circuitos electr  ́ onicos, como lo es ”Proteus”,  ́
proporciona un entorno virtual para disenar, simular y depurar circuitos antes de la im-  ̃
plementacion f  ́  ́ısica.

Realizar una simulacion del dise  ́ no antes de implementarlo de forma f  ̃  ́ısica contribu-
ye significativamente al proyecto, pues esto ayuda a identificar errores, realizar cambios

y evitar el retraso al quemar o averiar un componente.
En la siguiente imagen se observara una simulacion para obtener la temperatura en  ́
el ambiente utilizando el sensor DHT22 y as ́ı asegurarnos de que las condiciones dentro
del invernadero son ideales para el crecimiento y desarrollo de los cultivos 3.4.

Figura 3.4: Sensor para la Temperatura del ambiente

20 CAP ́ITULO 3. DESARROLLO

De la misma manera fue disenado otra simulaci  ̃ on para obtener la humedad de la  ́
tierra disenada con un sensor hidrometro de esta forma tendremos total control en las  ̃
condiciones que podr ́ıan afectar y/o beneficiar a nuestros cultivos 3.5.

Figura 3.5: Sensor para la Humedad en la Tierra

3.4.1. Visualizacion de datos dentro de una pantalla OLED  ́

En el desarrollo del proyecto se ha visto reflejado la visualizacion de datos obteni-  ́
dos por los sensores dht11, lm35, y el sensor puesto a tierra, los cuales son componentes
esenciales para la adquisicion de datos de temperatura y humedad. Estas variables am-  ́
bientales son las que se estan trabajando dentro del proyecto, sin embargo, en necesario  ́
que dichos datos pueden proyectarse en una pantalla.

Anteriormente hemos trabajado con pantalla LCD para mostrar los datos de los sen-
sores, pero en esta ocasion vamos a mostrar los datos de los sensores dentro de una  ́

pantalla OLED.

A continuacion, podremos observar algunas de las simulaciones desarrolladas en  ́
el software de proteus, las cuales son la introduccion hacia los circuitos con pantallas  ́
OLED los cuales deriban de codigos mas complejos, en el siguiente ejemplo en especi-  ́
fico se mostrara un mensajes de texto, as  ́  ́ı como algunos caracteres especiales dentro de
una pantalla OLED, este sera el ”Hola mundo”de las pantallas OLED.  ́

3.4. HARDWARE 21

Figura 3.6: Primera simulacion de una pantalla oled

3.4.2. Modulacion por ancho de pulso  ́
En la proxima simulaci  ́ on veremos la aplicaci  ́ on del pwm, de como podemos con-  ́
trolar el voltaje por medio de un potenciometro y dicho valor de voltaje se vera reflejado  ́
en una pantalla OLED, as ́ı como podremos visualizar por medio de un osciloscopio el
comportamiento de la senal en sus respectivos estados altos y bajos.  ̃

Figura 3.7: Simulacion de pwm en proteus  ́

La simulacion anterior est  ́ a conformada por un pulsador y un resistor en el pin del  ́
Master Clear, as ́ı como sus respectivos cables en los pines de SDA y SCL los cuales
estan conectados directamente hacia la pantalla OLED adem  ́ as en el pin RA0 podemos  ́
encontrar un potenciometro el cual nos ayuda a controlar el voltaje del circuito, el cual  ́
se vera reflejado en la pantalla OLED.  ́
3.4.3. DHT11

Siguiendo con las simulaciones se adaptara nuevamente un circuito donde se mues-
tren los valores del sensor de temperatura y humedad, el sensor DHT11, sin embargo,

se mostraran dichos valores en una pantalla oled. En su configuracion se encuentra el  ́
circuito m ́ınimo de funcionamiento, el cual incluye el oscilador de cristal, el maestro

22 CAP ́ITULO 3. DESARROLLO

limpio, es decir y el boton que reinicia la secuencia del microcontrolador, por supuesto  ́
se implementara la pantalla OLED con todos aquellos resistores que protejen tanto el
PIC como la pantalla, sin embargo, no se debe dejar aparte el componente principal que
seria el sensor DHT11.

Figura 3.8: Tercera simulacion en proteus mostrando los valores del sensor DHT11

3.4.4. DHT11

Prosiguiendo con la tematica actual, nuevamente se dar  ́ a continuidad al c  ́ odigo y  ́
simulacion en donde se encuentra el sensor LM35, el cual mostrara los valores perte-  ́
necientes a la temperatura del ambiente, dicha simulacion contiene el circuito m  ́  ́ınimo
de funcionamiento y el susodicho sensor, sin embargo, aparte de la pantalla OLED en
donde se mostraran los valores, la pantalla debera ser protegida por los pulsos de bajada  ́
y subida por lo que dispondra de pocos resistores que se encarguen de evitar quemar  ́
tanto el PIC como la pantalla OLED

3.4. HARDWARE 23

Figura 3.9: Simulacion en Proteus mostrando los valores del sensor LM35

3.4.5. Sensor de Tierra
Una diferencia clara que se debe de tener en cuenta, es el uso que se le da a los
sensores pues algunos de las mediciones ya exhibidas tienen un proposito en especifico,  ́
en otras palabras la siguiente simulacion la cual presenta al sensor de Tierra, sirve tam-  ́
bien para la medici  ́ on de humedad, sin embargo, se diferencia de los valores obtenidos  ́
del sensor DHT11, puesto que este sensor mide la humedad de ambiente y el entorno,
en cambio el sensor actual como su nombre lo dice, mide la humedad encontrada en la
tierra.

Figura 3.10: Simulacion de los valores obtenidos por el Sensor de Tierra  ́

3.4.6. USART LM35
Una vez obteniendo los datos de los sensores sera indispensable poder mandar los  ́
datos hacia una PC para resguardar y respaldar la informacion, as  ́  ́ı se tendra un mayor  ́

24 CAP ́ITULO 3. DESARROLLO

control sobre el invernadero al conocer sus valores. Para poder transmitir los datos co-
rrectamente tambien se necesito realizar una simulaci  ́ on para conocer el funcionamiento  ́

del protocolo serial USART, en dicha simulacion se puso nuevamente el sensor de tem-  ́
peratura LM35 y sus valores en vez de mostrarse en una pantalla (OLED o LCD) se
usara una maquina virtual para simular una PC.

Figura 3.11: Simulacion mostrando en maquina virtual los valores de un sensor LM35  ́

3.4.7. Implementacion de Circuitos  ́

Finalmente tres de estos codigos se implementaran en uno solo, es decir, la siguiente  ́
simulacion se mostraran los valores de varios sensores como el DHT11, LM35 y el sen-  ́
sor a tierra, esto mostrado en una pantalla OLED, esta pantalla estara rotando continua-  ́
mente para mostrar las diferentes variables, es por ello que para una mayor presentacion ́
se introdujo al mismo tiempo una portada principal antes de mostrar todos los demas ́
valores.

3.4. HARDWARE 25

Figura 3.12: Simulacion donde se mostrar  ́ a una uni  ́ on de varios sensores en una pantalla  ́
OLED

3.4.8. Hola Mundo en Hardware

Para la implementacion de la pantalla OLED, el primer circuito a realizar seria la
bienvenida, en la figura 3.13 se presenta la implementacion en f  ́  ́ısico.

26 CAP ́ITULO 3. DESARROLLO

Figura 3.13: Circuito Fisico del Hola Mundo en pantalla OLED

3.4.9. Sensor de temperatura LM35
A continuacion ́ 3.14 se mostrara el circuito que implementa el uso del sensor LM35  ́
construido de forma f ́ısica

Figura 3.14: circuito f ́ısico del Sensor LM35

3.4.10. Sensor de tierra
Continuando con los circuitos, en la siguiente figura 3.15 se observa el circuito del
sensor de tierra implementado en f ́ısico.

3.4. HARDWARE 27

Figura 3.15: Sensor de Tierra implementado de forma fisica

3.4.11. Sensor DHT11

Siguiendo con los resultados obtenidos el siguiente en mostrar 3.16sera el circuito  ́
de sensor de humedad y temperatura DHT11 construidos de forma f ́ısica.

Figura 3.16: Sensor de humedad y temperatura construido de forma fisica

3.4.12. Compilacion de Circuitos  ́

Despues de verificar el correcto funcionamiento de los circuitos anteriores, se cons-  ́
truira la conexi  ́ on entre ellos, es decir, a continuaci  ́ on se mostrara el circuito que imple-  ́
menta el uso de una variedad de sensores de forma f ́ısica.

28 CAP ́ITULO 3. DESARROLLO

Figura 3.17: Circuito f ́ısico que usa una variedad de sensores

3.4.13. USART
Finalmente se mostrara el ultimo circuito construido  ́ 4.10, el cual seria el envio de
datos mediante USART usando el LM35.

Figura 3.18: Circuito en fisico de la conexion USART

3.4. HARDWARE 29

Es importante conocer la temperatura dentro del invernadero, esto para controlar y

monitorear el crecimiento de las plantas, al ajustar sus condiciones ambientales, sin em-
bargo, para poder conocer su temperatura se tuvo que construir 2 circuitos para tomar la

temperatura del ambiente para comparar sus mediciones con un termometro.  ́
En la siguiente figura se mostrara los circuitos hechos con los sensores LM35,DHT11  ́

y DHT22 en comparacion con la medici  ́ on de temperatura de un mult  ́  ́ımetro, todos mi-
diendo temperatura ambiente.

Figura 3.19: Mediciones de sensores de temperatura del ambiente

Sin embargo, las temperaturas no son constantes durante el d ́ıa, por lo que, se to-
maron muestras a diferentes horas para observar el cambio de temperatura. Durante las

siguientes imagenes se mostrar  ́ an las gr  ́ aficas hechas con los valores obtenidos durante  ́
las capturas de temperatura:

Figura 3.20: Graficas realizadas con los valores obtenidos del sensor DHT-11

30 CAP ́ITULO 3. DESARROLLO

Figura 3.21: Graficas realizadas con los valores obtenidos del sensor DHT-22

Figura 3.22: Graficas realizadas con los valores obtenidos del sensor LM35

Figura 3.23: Graficas realizadas con los valores obtenidos con el mult ́ımetro

3.5. PROPUESTA 31

3.5. Propuesta
Para iniciar, es indispensable la creacion de dise  ́ no sobre un sistema de control que  ̃

sea capaz de captar diferentes mediciones las cuales incluyen: la temperatura, la hu-
medad del aire y la humedad de la tierra, en tiempo real y mostrar este valor en una

pantalla OLED. El sistema determinara 2 rangos de temperatura diferentes, cuando sea
menor que 25 ◦C y cuando sea mayor a este, en este ultimo caso, se mandara una alerta.
Concretamente para controlar la temperatura se activara un ventilador dependiendo de la  ́
temperatura. A continuacion, se presenta el diagrama a bloques del circuito propuesto,  ́
en donde se mostrara la conexi  ́ on realizada entre componentes:  ́

Figura 3.24: Diagrama de bloques

3.5.1. Explicacion ́
Fuente de poder: Tendra una capacidad de 5 voltios, la cual ser  ́ a la responsable de  ́
alimentar el resto de los componentes.
Pantalla oled: Sera un dispositivo encargado de visualizar el valor de las variables.  ́
Sensor LM35:Se especializa en obtener la temperatura de forma precisa.

32 CAP ́ITULO 3. DESARROLLO

Sensor DHT-11: El sensor es capaz de obtener la temperatura y la humedad del
ambiente.
Sensor de humedad del suelo: Este sensor es capaz de recolectar la humedad que
se encuentra en la tierra de las plantas.
Resistor 10 K Ohms: Es el encargado de proteger el microcontrolador (PIC) contra
la corriente.
Resistor de 220 Ohms: Este resistor es el responsable de proteger al diodo led
contra la corriente.
Diodo led: Este componente emisor de luz.
Fuente de 9 Voltio: Esta fuente de poder tendra una capacidad de 9 voltios, la cual  ́
sera la responsable de alimentar componentes espec  ́  ́ıficos.
Puente H: Circuito utilizado para el control de motores.
Motor: Modulador de temperatura.
Comunicacion RS232: Modulo serial para la transmisi  ́ on de informaci  ́ on.  ́
Ambiente grafico: Visualizaci  ́ on de datos que van a la computadora.  ́
Computadora: Medio receptor de datos.
PIC: Microcontrolador programable para la funcion de los diferentes componen-  ́
tes.

3.6. DESARROLLO DEL CODIGO  ́ 33

3.6. Desarrollo del codigo  ́

A continuacion, se mostrar  ́ a el diagrama de flujos el cual explicar  ́ a la estructura de  ́
la programacion del microcontrolador PIC el cual controlar  ́ a los aspectos del funciona-  ́
miento del circuito:

Figura 3.25: Diagrama de flujo

34 CAP ́ITULO 3. DESARROLLO

Figura 3.26: Continuidad del diagrama de flujo
El diagrama anteriormente visto, cuenta con los siguientes recuadros:
Inicio, usa un s ́ımbolo ?principio o fin, en donde especifica donde empieza.
KATSI S-H, usa un S ́ımbolo de pantalla para mostrar texto ya especificado.
SENSOR LM35, usa un S ́ımbolo de pantalla para mostrar texto ya especificado.
Leer sensor LM35, usa un S ́ımbolo de proceso para determinar el valor entrante
del sensor.
ADC=0, usa un s ́ımbolo de decision en donde se eval  ́ ua si la entrada de ADC de  ́
un sensor hacia el PIC es igual o mayor a 0.

Sensor no conectado, usa un S ́ımbolo de pantalla para mostrar texto ya especifi-
cado en donde se muestra unicamente si la decisi  ́ on es cierta.  ́

TEMP? ADC, usa un s ́ımbolo de entrada o salida para ingresar el valor del ADC
hacia una formula ya prescrita, en donde se guardara ́ unicamente si la decisi  ́ on es  ́
incorrecta.

3.6. DESARROLLO DEL CODIGO  ́ 35

TEMP ¡ 25 usa un s ́ımbolo de decision en donde se eval  ́ ua si el valor de la tempe-  ́
ratura obtenida es mayor o menor que 25◦
.

Apagar motor, usa un S ́ımbolo de proceso para quitar el pulso hacia los motores
(en caso de que lo tenga), este proceso se llevara a cabo  ́ unicamente si la tempera-  ́
tura en menor a 25 grados.

Encender Motor, usa un S ́ımbolo de proceso para colocar un pulso hacia los mo-
tores (en caso de que no lo tenga), este proceso se llevara a cabo  ́ unicamente si la  ́

temperatura en mayor a 25 grados.
1, es un s ́ımbolo de conector y especifica que el diagrama de flujos continuara en
otra pagina.  ́
Envio por USART, usa un S  ́  ́ımbolo de proceso para enviar el valor del sensor hacia
un pc.
DHT11, usa un S ́ımbolo de pantalla para mostrar texto ya especificado.
Leer sensor DHT11, usa un S ́ımbolo de proceso para determinar el valor entrante
del sensor.
. ADC=0, usa un s ́ımbolo de decision en donde se eval  ́ ua si la entrada de ADC de  ́
un sensor hacia el PIC es igual o mayor a 0.

Sensor no conectado, usa un S ́ımbolo de pantalla para mostrar texto ya especifi-
cado en donde se muestra unicamente si la decisi  ́ on es cierta.  ́

Temperatura ? ADC, usa un s ́ımbolo de entrada o salida para ingresar el valor
del ADC hacia una formula ya prescrita, en donde se guardara ́ unicamente si la  ́
decision es incorrecta.  ́
Humedad ? ADC, usa un s ́ımbolo de entrada o salida para ingresar el valor del
ADC hacia una formula ya prescrita, en donde se guardara ́ unicamente si la deci-  ́
sion es incorrecta.  ́
Envio por USART, usa un S  ́  ́ımbolo de proceso para enviar el valor del sensor hacia
un pc.
SENSOR DE HUMEDAD DE SUELO, usa un S ́ımbolo de pantalla para mostrar
texto ya especificado.
2, es un s ́ımbolo de conector y especifica que el diagrama de flujos continuara en
otro lugar.
Leer SENSOR DE HUMEDAD DE SUELO, usa un S ́ımbolo de proceso para
determinar el valor entrante del sensor.

36 CAP ́ITULO 3. DESARROLLO

ADC=0, usa un s ́ımbolo de decision en donde se eval  ́ ua si la entrada de ADC de  ́
un sensor hacia el PIC es igual o mayor a 0.

Sensor no conectado, usa un S ́ımbolo de pantalla para mostrar texto ya especifi-
cado en donde se muestra unicamente si la decisi  ́ on es cierta.  ́

Humedad ? ADC, usa un s ́ımbolo de entrada o salida para ingresar el valor del
ADC hacia una formula ya prescrita, en donde se guardara ́ unicamente si la deci-  ́
sion es incorrecta.  ́
Envio por USART, usa un S  ́  ́ımbolo de proceso para enviar el valor del sensor hacia
un pc.
FIN, usa un s ́ımbolo principio o fin, en donde especifica donde termina.
3.6.1. Simulacion del circuito en el software de proteus  ́
A continuacion, se mostrar el circuito simulado en el software de proteus y las prue-  ́
bas de que esta funcionado correctamente.

Figura 3.27: Circuito construido en el software de proteus
Como podemos observar nuestro circuito esta constituido de un microcontrolador
PIC, de un pantalla oled, de los sensores LM35 para la medicion de la temperatura y tam-  ́
bien un sensor DHT-11 para medir la temperatura y la humedad del ambiente, adem  ́ as ́
cuenta con un diodo led que sirve como indicador de un cierto rango de temperatura que
definiremos mas adelante.  ́

3.6. DESARROLLO DEL CODIGO  ́ 37

Figura 3.28: Circuito funcionando en el software de proteus

Iniciamos la simulacion y podemos ver que funciona de manera correcta sin errores  ́
ya que los datos de la temperatura y humedad de ambos sensores se pueden visualizar
correctamente en la panatalla oled. Como podemos observa al momento de nosotros
bajar a temperatura, a menos de 24 grados de nuestro LM35 el diodo led que ten ́ıamos
conectado se apaga por completo ya que la temperatura no es lo suficientemente alta
para lograr encenderlo. Esto tambien hace a su vez que el motor deje de girar.  ́

Figura 3.29: Disminucion de la temperatura en el sensor LM35  ́

38 CAP ́ITULO 3. DESARROLLO

De igual manera podemos observar como al momento de eliminar un sensor o en el
caso real de no tener un senor conectado nos mandara un mensaje indicando que no se
encuentra conectado ningun sensor, este mensaje nos ayuda a percatarnos para darnos  ́
cuenta si el sensor esta mal conectado o tambien si el sensor tiene alg  ́ un fallo.  ́

Figura 3.30: Mensaje de error ya que no se encuentra conectado el sensor

3.6.2. Circuito construido f ́ısicamente
Al terminar las pruebas en el software de proteus pasamos a recrear el circuito en una
protoboard y realizar las pruebas correspondientes para verificar que todos los sensores
funcionaran de manera correcta y verificando que no existan errores.

Figura 3.31: Circuito recreado en protoboard

3.6. DESARROLLO DEL CODIGO  ́ 39

3.6.3. Pruebas de mediciones con el circuito en protoboard
Mas tarde se realizaron pruebas de mediciones con el circuito armado en la proto-  ́
board para corroborar que los sensores estuvieran obteniendo la temperaturas y pudieran

visualizarse en la pantalla oled. Para realizar dichas mediciones se tomaron en cuenta di-
ferentes lugares y horarios ya que la temperatura puede varias dependiendo mucho de

estos factores.Esto con el objetivo de comprobar si los sensores estaban obteniendo los
mismos valores que el multimetro y corroborar cual de los dos sensores LM35 o DHT-11
ten ́ıa los valores mas precisos.  ́

Figura 3.32: Pruebas de mediciones dentro del invernadero
Todas estas mediciones se fueron registrando en un archivo de excel en el cual se
crearon distintas tablas con los valores obtenidos en cada uno de los sensores.Las cuales
podremos observar con mayor detalle en el cap ́ıtulo de resultados.La temperatura es de
las variables mas importantes dentro de un inveradero ya que esta en la mayor parte de  ́
los casos debe ser constante.

Figura 3.33: Horario con mayor temperatura dentro del invernadero

40 CAP ́ITULO 3. DESARROLLO

De la misma manera se realizaron pruebas para la medicion de la temperatura en  ́
diferentes puntos de la universidad para obtener las temperaturas y percibir cual de los
dos sensores ten ́ıa mayor precision.  ́

Figura 3.34: Pruebas de medicion de temperatura en disntintos puntos de la universidad.  ́

Figura 3.35: Pruebas de medicion de temperatura en disntintos puntos de la universidad  ́

3.6. DESARROLLO DEL CODIGO  ́ 41

Posteriormente preparamos todo para el diseno de nuestra placa de circuito impreso  ̃
PCB y la desarrollamos con el metodo de planchado. De esta manera podemos apreciar  ́
que todas las pistas y as ́ı como los respectivos lugares de nuestros componentes ya se
encuentran en nuestra placa de cobre. Posteriormente pasamos a retirar el exceso de
cobre de nuestra placa de circuito impreso, nos apoyamos con cloruro ferrico, aunque  ́
tambien este procedimiento se puede realizar con  ́ acido muri  ́ atico.  ́

Figura 3.36: Metodo de planchado en PCB  ́

42 CAP ́ITULO 3. DESARROLLO

Al terminar el proceso de planchado y de haber sumergido nuestra placa de circuito
impreso en cloruro ferrico, obtendremos el siguiente resultado:  ́

Figura 3.37: Metodo de planchado en PCB  ́

Como podemos observar el cloruro ferrico retiro el exceso de cobre en la placa,  ́

dejando solamente las pistas del circuito y procederemos a realizar las respectivas perfo-
raciones para ir colocando los componentes que va llevar uno a uno y aplicaremos estano ̃

para soldar dichos componentes a la pbc.

Cap ́ıtulo 4

Resultados

4.1. Resultados hardware

Acto seguido podemos encontrar las tablas del archivo de Excel en el cual se alma-
cena la temperatura obtenida de los sensores y podremos observar las graficas generadas  ́

con distintos calculos como son los promedios de cada sensor, las tablas de errores,  ́
los promedios de los errores, las graficas de la semana en la que se estuvo tomando la  ́
temperatura entre otros aspectos.

4.2. Tabla con los valores de la temperatura obtenida median-
te el sensor LM35

Figura 4.1: Datos de la temperatura registrada con el sensor LM35 durante los 5 d ́ıas de
la semana.

43

44 CAP ́ITULO 4. RESULTADOS

4.3. Grafica con los valores de la temperatura obtenida me-  ́
diante el sensor LM35

Figura 4.2: Grafica de la temperatura registrada con el sensor LM35 durante los 5 d  ́  ́ıas
de la semana.

4.4. Tabla con los valores de la temperatura obtenida median-
te el sensor DHT-11

Figura 4.3: Datos de la temperatura registrada con el sensor DHT-11 durante los 5 d ́ıas
de la semana.

4.5. GRAFICA CON LOS VALORES DE LA TEMPERATURA OBTENIDA MEDIANTE  ́
EL SENSOR DHT-11 45
4.5. Grafica con los valores de la temperatura obtenida me-  ́
diante el sensor DHT-11

Figura 4.4: Grafica de la temperatura registrada con el sensor DHT-11 durante los 5 d  ́  ́ıas
de la semana.

Recordando que el sensor DHT-11 tambien nos proporciona la humedad del ambien-  ́
te la cual se presenta en la siguiente tabla.

4.6. Tabla con los valores de la humedad obtenida mediante
el sensor DHT-11

Figura 4.5: Datos de la humedad registrada con el sensor DHT-11 durante los 5 d ́ıas de
la semana.

46 CAP ́ITULO 4. RESULTADOS

4.7. Grafica con los valores de la humedad obtenida mediante  ́
el sensor DHT-11

Figura 4.6: Grafica de la humedad registrada con el sensor DHT-11 durante los 5 d  ́  ́ıas de
la semana.

4.8. Tabla con los valores de la temperatura obtenida median-
te el multimetro

Figura 4.7: Datos de la temperatura registrada con el multimetro durante los 5 d ́ıas de la
semana.

4.9. GRAFICA CON LOS VALORES DE LA TEMPERATURA OBTENIDA MEDIANTE  ́
EL SENSOR DHT-11 47
4.9. Grafica con los valores de la temperatura obtenida me-  ́
diante el sensor DHT-11

Figura 4.8: Grafica de la temperatura registrada con el multimetro durante los 5 d  ́  ́ıas de
la semana.

4.10. Grafica de promedios del registro de temperatura de ca-  ́
da sensor

A continuacion, podremos observar las gr  ́ aficas de error que tiene cada uno de los  ́

sensores, as ́ı como el promedio de los sensores LM35, DHT-11 y el que tiene el mult ́ıme-
tro.

48 CAP ́ITULO 4. RESULTADOS

Figura 4.9: Grafica del promedio de las temperaturas del sensor LM35, DHT-11 y mul-  ́
timetro

Figura 4.10: Grafica de errores de los sensores con respecto al multimetro  ́

4.10.1. Modificado

El PIC puede realizar diversas funciones dependiendo de las condiciones que se apli-
quen, es decir, es posible modificar el codigo para cuando el PIC tenga las variables de  ́

los sensores se produzcan diferentes estados dependiendo del sensor que emita la va-
riable, por ejemplo, cuando el sensor LM35 obtenga una temperatura mayor a los 35

4.10. GRAFICA DE PROMEDIOS DEL REGISTRO DE TEMPERATURA DE CADA  ́
SENSOR 49
grados centigrados, el PIC, este se encarga de encender una alarma, un extractor y una

bomba dependiendo del tipo de lectura. Este tipo de funciones de ?emergencia? son ali-
mentados de manera externa al circuito como tal, usando corriente alterna para alimentar

aparatos con alto consumo de energ ́ıa, para ello se utilizara un relevador para utilizar los  ́
pulsos del PIC y controlar el encendido y apagado de estos aparatos. El cual estara ar-  ́
mado en un modulo separado de la PCB general al tener una placa de relevadores unidos.  ́

4.10.2. Modulo Xbee  ́
Durante este cuatrimestre se llevo a cabo el desarrollo de un sistema de comuni-  ́
cacion inal  ́ ambrica utilizando dos m  ́ odulos Xbee, los cuales se configuraron mediante  ́
adaptadores USB para establecer la conexion entre ellos. El proceso de configuraci  ́ on se  ́
realizo utilizando el software XCTU, herramienta que permite gestionar y programar los  ́
modulos Xbee de manera eficiente. En este proceso, uno de los m  ́ odulos se configur  ́ o co-  ́
mo transmisor y el otro como receptor, permitiendo as ́ı la transmision y recepci  ́ on de  ́
datos de manera bidireccional.

Figura 4.11: Interfaz Digi XCTU

Para llevar a cabo esta configuracion, se conectaron los m  ́ odulos Xbee a computado-  ́
ras a traves de puertos USB, operando en modo serial. A trav  ́ es del software XCTU,  ́
se ajusto el firmware de los m  ́ odulos, lo que posibilit  ́ o la correcta comunicaci  ́ on entre  ́
ambos dispositivos. Este ajuste es crucial para garantizar que los modulos pudieran in-  ́
tercambiar datos sin problemas, asegurando su correcto funcionamiento dentro de las
distancias y condiciones esperadas.

4.10.3. Pruebas y resultados
La manera de evitar un corto circuito o quemar algun componente durante las prue-  ́
bas, es realizando una simulacion del mismo circuito en alg  ́ un software de simulaci  ́ on en  ́
este caso, ?Proteus? a continuacion se mostrar  ́ an las conexiones del diagrama esquem  ́ ati-  ́
co del circuito.

50 CAP ́ITULO 4. RESULTADOS

Figura 4.12: Simulacion del circuito  ́

Al verificar el funcionamiento correcto en la simulacion pasaremos a las pruebas  ́

f ́ısicas, armando el circuito en una ProtoBoard y realizar observaciones sobre las accio-
nes del mismo circuito, haciendo uso de corriente directa (DC).

Figura 4.13: Prueba f ́ısica de funcionamiento

Inmediatamente en estas pruebas de funcionamiento, se deberan comprobar las ac-  ́
ciones realizadas por el PIC al cambio de variables en las mediciones de los sensores,
como se mostrara en la siguiente imagen.  ́

4.10. GRAFICA DE PROMEDIOS DEL REGISTRO DE TEMPERATURA DE CADA  ́
SENSOR 51

Figura 4.14: Cambio de variables en prueba de funcionamiento.

Al tener un funcionamiento cercano al deseado, las pruebas pasan por un cambio

de voltaje, cambiando entre corriente directa hacia corriente alterna, donde se reempla-
zaran componentes, como Leds, resistencias, etc. En la siguiente imagen se mostrar  ́ an ́

los cambios ya hechos en el circuito integrado.

Figura 4.15: Cambio de voltaje, AC.

Tras realizar dichos cambios se debera comprobar nuevamente su correcto funcio-  ́
namiento mostrados en la siguiente imagen.

52 CAP ́ITULO 4. RESULTADOS

Figura 4.16: Buen funcionamiento con corriente Alterna.

Mediante el uso del modulo USART el circuito se conectar  ́ a hacia una computadora,  ́
donde el codigo ingresado mandar  ́ a los datos de los sensores a trav  ́ es de un puerto COM  ́
y al mismo tiempo guardando sus datos en un archivo de texto como se mostrara a con-  ́
tinuacion en la siguiente imagen.  ́

Figura 4.17: Almacenamiento de datos

Una vez que el circuito haga lo esperamos, sabremos que las conexiones esquemati-  ́

4.10. GRAFICA DE PROMEDIOS DEL REGISTRO DE TEMPERATURA DE CADA  ́
SENSOR 53
cas estan en orden y se podr  ́ a pasar al armado de la PCB, esto se iniciara con el diagrama  ́
en 2D para realizar las conexiones de los Footprint. En la siguiente imagen se mostrara el  ́
diagrama terminado.

Figura 4.18: Diagrama 2D del circuito

Una vez construido el esquematico como el que se muestra en la figura 11 se podr  ́ a vi-  ́
sualizar el modo 3D de la placa PCB para visualizar como se ver ́ıa en f ́ısico.

54 CAP ́ITULO 4. RESULTADOS

Figura 4.19: Placa PCB modelo 3D

El siguiente paso sera le planchado de la placaba base, al exportarse en PDF el docu-  ́
mento puede imprimirse en papel transfer para facilitar ser pegado en una PCB mediante
el planchado.

4.10. GRAFICA DE PROMEDIOS DEL REGISTRO DE TEMPERATURA DE CADA  ́
SENSOR 55

Figura 4.20: Planchado de la placa base

cuando es terminado de planchar, el diseno queda pegado a la PCB, aqu  ̃  ́ı debera ser  ́
puesto en cloruro ferrico para disolver los excedentes de cobre, dejando  ́ unicamente las  ́
pistas.

56 CAP ́ITULO 4. RESULTADOS

Figura 4.21: PCB en acido ferrico  ́

Cuando se terminan de disolver, estara listo para la perforaci  ́ on de las terminales,  ́
donde iran los componentes y posteriormente su soldado como se ver  ́ a en la siguiente  ́
imagen.

Figura 4.22: . Perforacion y posterior soldadura  ́

4.10. GRAFICA DE PROMEDIOS DEL REGISTRO DE TEMPERATURA DE CADA  ́
SENSOR 57

Al contar con nuestra placa de circuito impreso de manera f ́ısica pasaremos a la sec-
cion de pruebas d  ́ onde se verificar  ́ a que el circuito funcione de manera correcta y no  ́

existe ningun error.  ́
Durante la realizacion de las pruebas restantes se implement  ́ o, un sistema de comuni-  ́
cacion basado en Xbee, el cual demostr  ́ o tener un alcance aproximado de 90.  ́

metros en entornos cerrados, lo cual es adecuado para aplicaciones que requieren co-
municacion dentro de edificios o estructuras con obst  ́ aculos. En espacios abiertos, el  ́

alcance se amplio significativamente, llegando a alcanzar hasta 3200 metros, lo que hace  ́
que este sistema sea adecuado para aplicaciones al aire libre, donde no hay interferencias
f ́ısicas significativas.

Figura 4.23: Prueba de env ́ıo y recepcion de mensajes con m  ́ odulos Xbee.  ́
mensajes con modulos Xbee. Como se observa en la figura 18 se realizaron las prue-  ́
bas de envio de informaci  ́ on de manera inal  ́ ambrica implementado los m  ́ odulos Xbee.  ́
Esta comunicacion fue solamente un emisor y receptor, posteriormente se pretende am-  ́
pliar la topolog ́ıa.

Cap ́ıtulo 5

Actividades realizadas en los
cuatrimestres anteriores

5.1. Septiembre diciembre 2023.
Analisis de proyectos anteriores o similares.  ́
Estudio del estado del arte.
Comprension te  ́ orica del proyecto.  ́
Examinar software de desarrollo de circuitos electronicos.  ́
Simulacion de circuitos en PIC para aplicaci  ́ on de invernaderos.  ́
Formular la implementacion de una topolog  ́  ́ıa de red.
Estudio de los sensores de temperatura y humedad LM35 y DHT-11.
Construccion de un circuito en protoboard para la toma y visualizaci  ́ on de datos  ́
de un sensor de humedad del suelo.
Examinar la arquitectura interna de los microcontroladores para comprender su
funcionamiento y apliaciones.
Construccion de diagramas a bloques para el entendimiento de la lectura de sen-  ́
sores.
Limpieza del invernadero.
Cultivo de plantas dentro de semilleros.
Construccion del sistema m  ́  ́ınimo del circuito PIC en protoboard.

59

60CAP ́ITULO 5. ACTIVIDADES REALIZADAS EN LOS CUATRIMESTRES ANTERIORES

5.2. Enero abril 2024.
Implementacion de nuevos componentes electr  ́ onicos termistor, transistor, hidr  ́ ome-  ́
tro, pantalla oled y pantalla lcd.
Investigacion de los nuevos componentes implementados.  ́
Construccion del sistema m  ́  ́ınimo para aplicacion de invernaderos con la utiliza-  ́
cion del microcontrolador PIC.  ́
Estudio de almacenamiento en el microcontrolador PIC.
Descripcion de los sensores utilizados LM35, DHT-11,DHT-22.  ́
Investigacion de las conversiones anal  ́ ogica ? digital.  ́
Estudio de los sensores de temperatura y humedad LM35 y DHT-11.
Atribuir el teorema de muestreo.
Aplicacion del protocolo I2C.  ́
Actualizacion del diagrama a bloques presentado el cuatrimestre anterior.  ́
Creacion de circuitos soldados para la exhibici  ́ on de los valores de los sensores de  ́
temperatura y de humedad.
Union de circuitos electr  ́ onicos de los diferentes sensores utilizados en el trans-  ́
curso del proyecto.
Visualizacion de datos de temperatura y humedad en pantalla OLED.  ́
Construccion de un invernadero a escala para su exhibici  ́ on en el sal  ́ on.  ́
Analisis del principio te  ́ orico del sistema de comunicaci  ́ on USAR.  ́
5.3. Mayo agosto 2024.
Realizacion de pruebas con los sensores para la b  ́ usqueda de una calibraci  ́ on de  ́
las mediciones.
Generacion de estad  ́  ́ısticas para la calibracion de los sensores.  ́
Creacion de gr  ́ aficos a partir de las estad  ́  ́ısticas de los sensores, para el analisis de  ́
precision y exactitud.  ́
Replica de los circuitos para generacion de constelaci  ́ on de sensores.  ́
Analisis del sistema USAR de comunicaci  ́ on.  ́

5.4. ACTIVIDADES A REALIZAR EN LOS PROXIMOS CUATRIMESTRES  ́ 61

5.4. Actividades a realizar en los proximos cuatrimestres  ́
Actividades a realizar en los proximos cuatrimestres con respecto al proyecto KATSI  ́
Hardware.

5.5. Septimo cuatrimestre.  ́
Retraso en tiempo de muestreo de variables de temperatura y humedad.
Almacenamiento de la transmision de datos de variables ambientales.  ́
Creacion del circuito de la pantalla oled del sensor de humedad de la tierra.  ́
Implementacion de todos los sensores en una sola tarjeta electr  ́ onica.  ́
Desarrollo de un generador 5 voltios para la activacion de un relevador hac  ́  ́ıa otros
componentes.
Implementacion de extractor para la disminuci  ́ on de la temperatura dentro del  ́
invernadero.
Investigacion sobre las mediciones del PH del agua, as  ́  ́ı como el funcionamiento
del sensor.
Ensamble superficial del circuito en una tarjeta electronica de circuito impreso.  ́
Instauracion de una alarma por medio del encendido de un foco.  ́
Pruebas de los componentes electricos dentro del invernadero.  ́
5.6. Octavo cuatrimestre.
Desarrollo de modulos para la tarje electr  ́ onica principal.  ́
Configuracion de la transmisi  ́ on de datos de manera inal  ́ ambrica.  ́
Activacion de una bomba de agua para el riego de plantas dentro del invernadero.  ́
Aplicacion de sensores de humedad del suelo para medir la humedad dentro de  ́
los semilleros de las plantas.
Canalizacion de agua pluvial para su aprovechamiento en el riego.  ́
Deteccion del nivel del agua en el tanque de riego.  ́
Riego por goteo para suministrar el agua con la cual cuenta el invernadero.

62CAP ́ITULO 5. ACTIVIDADES REALIZADAS EN LOS CUATRIMESTRES ANTERIORES

Control de la luz dentro del invernadero con sensores de movimiento.
Riego automatico mediante nebulizaci  ́ on.  ́
5.7. Noveno cuatrimestre.
Controlar la intensidad de la luz para simular la luz natural.
Comunicacion entre placa maestro y placa esclava.  ́
Aplicacion de una topolog  ́  ́ıa de red.
Sistema de acceso al invernadero.
Automatizacion del sistema de cultivo hidrop  ́ onico.  ́
Pruebas de funcionamiento en otros ambientes.
Establecimiento de umbrales.
Pruebas finales de la tarjeta electronica y comparaci  ́ on de datos.  ́
Sistema de alerta de fallos electricos.  ́
Sistema de calefaccion para aumentar la temperatura.  ́

5.8. ACTIVIDADES QUE SE ESTAN REALIZANDO 63

5.8. Actividades que se estan realizando
Se realizo una simulacion en el software de proteus para la realizaci  ́ on de un circuito  ́

usando el sensor de humedad de tierra, dando como diferencia el cambio en la visuali-
zacion, usando la pantalla Oled en lugar de la pantalla LCD, en la siguiente imagen se  ́

mostraran dos simulaciones del circuito, una en funcionamiento inicial y la segunda en  ́
la demostracion de variables:  ́

5.9. Circuito inicial

Figura 5.1: Funcionamiento inicial del circuito

5.10. Demostracion de variables en el circuito  ́

Figura 5.2: Demostracion de variables  ́

64CAP ́ITULO 5. ACTIVIDADES REALIZADAS EN LOS CUATRIMESTRES ANTERIORES

5.11. Mediciones de humedad

Para la comprobacion de su funcionamiento en f  ́  ́ısico, se realizo circuito usando so-  ́
lamente el sensor de humedad de tierra apartado del circuito general, dando oportunidad
y mayor movilidad en la realizacion de experimentos y pruebas de funcionamiento. La  ́
realizacion de pruebas de funcionamiento se centraba en la medici  ́ on de humedad en  ́
casos practicos con vasos llenos de tierra y diferente nivel de riego, siendo estas: seco,  ́
poco, medio y puro.

Figura 5.3: Pruebas de medicion de humedad  ́

Primero, se agrego un mensaje de bienvenida con el nombre del sensor, con la fina-  ́
lidad de mostrar su funcionamiento correcto antes de la realizacion de las pruebas.  ́

Figura 5.4: Visualizacion de mensaje inicial  ́

La siguiente imagen mostrara un nivel de humedad seco, dando como referencia a
que no se conecto a tierra:

5.11. MEDICIONES DE HUMEDAD 65

Figura 5.5: Sensor de puesta a tierra

Dando continuacion con las pruebas, la siguiente se conecto a tierra con un nivel de  ́
riego bajo:

Figura 5.6: Pruebas de humedad con vasos de agua

Posteriormente se introduje el sensor en el siguiente recipiente con un nivel superior
en humedad, sin embargo, un nivel de agua aun controlado.

66CAP ́ITULO 5. ACTIVIDADES REALIZADAS EN LOS CUATRIMESTRES ANTERIORES

Figura 5.7: Realizando pruebas de humedad

Finalmente, en la ultima prueba se introdujo el sensor en un estado de agua ?puro?,  ́
es decir, sin intervencion de tierra.  ́

5.11. MEDICIONES DE HUMEDAD 67

Figura 5.8: Visualizacion de humedad en pantalla Oled  ́

En conclusion, el funcionamiento del circuito acerca del sensor de humedad de tie-  ́
rra con uso OLED es positivo, sin embargo, quedan detalles a definir, pues a pesar de
su buen funcionamiento este posee un margen de error bastante grande, sin embargo, su
correccion es posible con un ajuste en los valores iniciales de la conversi  ́ on.  ́
Enfocando otros casos, se llevara a cabo la construcci  ́ on de un sistema de control de  ́
temperatura, haciendo uso del sensor LM35, donde si esta es superior a ciertos grados,
prendera un sistema de enfriamiento mediante un ventilador. El ventilador a usar lle-

68CAP ́ITULO 5. ACTIVIDADES REALIZADAS EN LOS CUATRIMESTRES ANTERIORES

vara su propio circuito, debido esto se realizaron experimentos con un relevador para  ́
tener la opcion de controlar el propio ventilador. A  ́ nadiendo a este sistema de enfria-  ̃
miento un complementario, en otras palabras, un sistema de alarma la cual mediante un

foco alertara sobre el sobrecalentamiento y as  ́  ́ı mismo sobre el accionamiento del ven-
tilador. En la siguiente imagen se podra apreciar el sistema de alarma de forma directa  ́

con voltaje directo:

Figura 5.9: Endendido de diodo led simulando el encendido de un foco

5.12. Subtema de transferencia de archivos

Utilizando el circuito general, donde se mantienen los demas sensores, el m  ́ odulo de  ́
transmision serial ?RS232?, mandara la informaci  ́ on que recaben los sensores a hacia la  ́
computadora mediante puertos COM, la visualizacion es posible con software que lean  ́
estos puertos COM, como seria el caso con ?Hercules? o ?Putty?, sin embargo, en el
desarrollo de un script usando PowerShell de Windows, fue posible abrir el puerto COM
utilizado para la transferencia de datos y usar un echo para guardar estos mismos datos
en un archivo tipo .txt (archivo de texto).
A continuacion, se mostrar  ́ a el archivo de texto guardado tras la ejecuci  ́ on del script  ́
en PowerShell:

5.13. CRONOGRAMA DE ACTIVIDADES 69

Figura 5.10: Registros de temperatura almacenado en un archivo txt

5.13. Cronograma de actividades

Documento controlado por medios electrónicos. Para uso exclusivo de la Universidad Politécnica de Juventino Rosas.
Universidad Politécnica de Juventino Rosas
Carrera: IRT Cuatrimestre: Septiembre-Diciembre Nombre del proyecto: KATSI H-S
Academia(s): IRT Tutor(a): Juan Heriberto Gallegos Galindo Asesor(a): Juan Israel Yañez Vargas

Actividades. Semana

1 2 3 4 5 6 7 8 9 10 11 12 13 L M M J V L M M J V L M M J V L M M J V L M M J V L M M J V L M M J V L M M J V L M M J V L M M J V L M M J V L M M J V L M M J V

Retraso en tiempo de muestreo x Almacenamiento de la transmision de datos x x x Creacion del circuito Oled del sensor de humedad de tierra x x
Implementacion de todos los sensores x x x Creacion de un generador 5 volts x x x
Implementacion de ventilador de enfriamiento x x
Investigacion de medicion de PH x x x x x x x
Implementacion en PCB x x x x

ACTIVIDADES REALIZADAS DE SER UN PROYECTO FACTIBLE PARA SER INCUBADO LLENAR LA SIGUIENTE INFORMACIÓN
DOCENTES INVOLUCRADOS (Nombre, Carrera y Materia) OBJETIVO: TIPO DE PROYECTO (CLASIFICACIÓN):
Dr. Juan Israel Yanez Vargas PROYECCIÓN: RESULTADOS OBTENIDOS: M.C. Víctor Lauro Perez García
ALUMNOS(AS) INVOLUCRADOS (Nombre, Carrera)
Ramses Alejandro Ramos Guerrero Cristian Jesus Ortiz Pineda

Cap ́ıtulo 6

Conclusion
 ́

En las etapas iniciales, el proyecto se enfoco en integrar sensores de temperatura,  ́
humedad ambiental y humedad de la tierra en un unico circuito electr  ́ onico capaz de  ́

mostrar las variables en una pantalla OLED y enviar datos a una PC mediante el pro-
tocolo de comunicacion USART. Este proceso requiri  ́ o m ́ ultiples actividades, como la  ́

validacion de sensores, la construcci  ́ on de circuitos y c  ́ alculos de errores, garantizando la  ́
fiabilidad del sistema. Actualmente, el proyecto ha evolucionado mas all  ́ a del monitoreo,  ́
incorporando funcionalidades que permiten la interaccion din  ́ amica con el entorno. Por  ́
ejemplo, ahora es posible activar un ventilador cuando se detectan altas temperaturas, lo
que ampl ́ıa las aplicaciones practicas del sistema. Adem  ́ as, se trabaja en una interfaz de  ́
monitoreo remoto accesible y economica, desarrollada en software libre, lo que mejora  ́
su portabilidad y reduce costos.

71

72 CAP ́ITULO 6. CONCLUSION ́

6.1. Trabajo a Futuro
Implementacion de PCB de los diferentes sensores.  ́
Optimizacion de los recursos del microcontrolador.  ́
Aplicacion de topolog  ́  ́ıa mallada con modulos Xbee  ́
Uso de sensores de PH.
Envio de datos de manera al  ́ ambrica y posteriormente de manera inal  ́ ambrica.  ́

Bibliograf ́
ıa

73
