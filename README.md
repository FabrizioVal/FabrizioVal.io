# Gestor de Inventario con Inteligencia Artificial (G.I.A.I.)

Imagen final del proyecto)

La automatizacion es una parte fundamental en la produccion de objetos que usamos dia a dia. Una seccion muy importante de esta es la categorizacion y administracion de los productos automatizados, lo cual puede ser tedioso, ya que uno tiene que ***identificar, contar y anotar*** los productos entrantes.

Para resolver esta problematica, nuestro equipo creo un proyecto de prototipo capaz de identificar fotograficamente los productos, a traves del uso de inteligencia artificial. Ademas, estos productos seran mostrados en una pagina web, donde el usuario podra administrarlos.

<br>

## 📒 Indice

El indice, sigue un orden del proyecto USAR MUCHAS IMAGENES

- ⚙️ Funcionamiento

- 🔗 Componentes del proyecto

- 🔌 Conexiones esquematicas

- 📟 Codigos y software

- ⚡ Ultimos cambios

- 🛠️ Armado final

<br>

## ⚙️ Funcionamiento

El recorrido de nuestro proyecto inicia en la **seccion fisica**. 

IMAGEN DE LA CINTA CON SU ESTRUCTURA

En esta, tenemos una base solida impresa en PLA (ácido poliláctico) la cual es la encargada de sostener en sus correspondientes lugares todos los elementos utilizados.

La forma en que los productos se mueven es a traves de una cinta transportadora con rodillos accionada por 4 motores (ESPECIFICAR MODELO MOTORES). Para controlar esa logica (y toda la logica principal del sector fisico) es usado un microcontrolador ESP32 Dev-Kit-V1.

Sobre esta cinta, se encuentra el pilar central de la estructura. En su parte superior estan montados un sensor de distancia ultrasonido(HC-SR04) y una camara (ESP32Cam). Como podran suponer, la funcion de estos dos componentes es la siguiente:

Cuando el producto pase por debajo del pilar central, el sensor de distancia lo detectara. El ESP32 detendra los motores, y le dejara al ESP32Cam tomar una foto del producto. Una vez realizada esta accion, los motores se encienden nuevamente, dando lugar al siguiente producto.

Nuestra foto ya tomada es ahora enviada via Wi-Fi a un servidor de procesamiento. Es en este momento que comienza la **seccion digital**.

En el servidor de procesamiento, esta instalado una Inteligencia Artificial entrenada para reconocer los productos que pasaran por la cinta. Al finalizar esta operacion, se notifica a la parte fisica del exito, y se obtienen los siguientes datos:

- Nombre del producto
- Cantidad (1)

Esta informacion es actualizada en la base de datos (MongoDB) del proyecto.

Por otro lado, existe otro servidor, el cual lee los cambios producidos en la base de datos. Este servidor es el encargado de proyectar una pagina web de administracion al usuario. El usuario podra visualizar, modificar, eliminar o agregar productos locamente al sitio web. 

Y con esto concluye el ciclo de funcionamiento de nuestro proyecto.

## 🔗 Componentes del proyecto

Los componentes fisicos principales utilizados para el desarrollo electronico de nuestro proyecto son:

- ESP32 Dev-Kit-V1
- ESP32Cam
- Sensor ultrasonido HC-SR04
- Controlador de motores DRV8833 (2)
- Motor QUEMODELO? (4)

## 🔌 Conexiones esquematicas

**- Placa de comando**
<br>
<br>
<img src="https://github.com/fabrizioval/fabrizioval.io/blob/main/images/esp32placaesquematico.png"/>


**- Placa ESP32Cam**
<br>
<br>
<img src="https://github.com/FabrizioVal/FabrizioVal.io/blob/main/Images/ESP32CamPlaca.png"/>

**- Controladores de motores**
<br>
<br>
<img src="https://github.com/FabrizioVal/FabrizioVal.io/blob/main/Images/Controladores%20de%20motores.png"/>

## 📟 Codigos y software

EXPLICAR DE FORMA SIMILAR EL FUNCIONAMIENTO GENERAL DE LOS CODIGOS

## ⚡ Cambios y mejoras

Durante el transcurso de nuestro proyecto surgieron ciertos problemas a resolver. Podemos destacar 2 problemas, los cuales veremos a continuacion:

En primer lugar, originalmente nuestros controladores de motores eran modelos L298n.
El problema con esto es que, debido a la cantidad de conexiones entre componentes, nos obligaba a realizar un diseño doble faz para nuestra placa de comando. 
Hubo varios modelos de placa doble faz realizados para nuestro proyecto, pero no se acercaron a ser el modelo correcto para lo que buscabamos fabricar.
Por esto mismo, buscamos un modelo de driver de motores con diferentes conexiones mas practicas para nuestro diseño. 
Al final, los drivers L298n fueron reemplazados por drivers DRV8833. 

En segundo lugar, 

## 🛠️ Armado final


<br>


acomodar esto bien (me faltan 2)

[Altamirano Valentino]()

[Avila Tomas](https://github.com/VMASPAD)

[Campusano Federico](https://github.com/FedeCampu1)

[Sebastian Galeotti]()

[Vallone Fabrizio](https://github.com/FabrizioVal)










Ultima seccion, adjuntar PDF del proyecto y repo
