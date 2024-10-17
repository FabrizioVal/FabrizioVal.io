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

## 🔌 Conexiones esquematicas

## 📟 Codigos y software

## ⚡ Ultimos cambios

## 🛠️ Armado final


<br>


acomodar esto bien (me faltan 2)

[Altamirano Valentino]()

[Avila Tomas](https://github.com/VMASPAD)

[Campusano Federico](https://github.com/FedeCampu1)

[Sebastian Galeotti]()

[Vallone Fabrizio](https://github.com/FabrizioVal)










Ultima seccion, adjuntar PDF del proyecto y repo
