# Gestor de Inventario con Inteligencia Artificial (G.I.A.I.)

Imagen final del proyecto)

La automatizacion es una parte fundamental en la produccion de objetos que usamos dia a dia. Una seccion muy importante de esta es la categorizacion y administracion de los productos automatizados, lo cual puede ser tedioso, ya que uno tiene que ***identificar, contar y anotar*** los productos entrantes.

Para resolver esta problematica, nuestro equipo creo un proyecto de prototipo capaz de identificar fotograficamente los productos, a traves del uso de inteligencia artificial. Ademas, estos productos seran mostrados en una pagina web, donde el usuario podra administrarlos.

# Introducción

## 📒 Indice

- [⚙️ Explicacion de areas](#user-content-️-explicación-de-areas)

- [🔧 Desarrollo](#user-content--desarrollo)

- [📸 Galeria](#user-content--galeria)

- [🌟 Autores](#user-content--autores)

- [🔒 Licencia](#user-content--licencia)

## ⚙️ Explicación de areas

<br>

![diagrama](https://github.com/FabrizioVal/Proyecto_G.I.A.I./blob/main/GithubImages/GIAI.drawio.png)

El diagrama de bloques mostrado en la imagen funciona de la siguiente forma:

### Scan físico

  - En el sector de trabajo, hay una cinta transportadora. Los productos que se coloquen sobre esta se moverán de una punta a la otra. 

  - La cinta está montada en un soporte. Sobre la cinta se sitúa una cámara y un sensor de distancia. El sensor detecta cuando el producto entra en la distancia de trabajo y con este dato la cinta se detiene.

  - La cámara toma una foto del producto, para que después la cinta pueda resumir su camino.

### Servidor de procesamiento

  - La imagen que es tomada se envía a un servidor de procesamiento. Este se encarga de analizar la imagen usando inteligencia artificial. Se toman como datos la imagen en sí, el nombre del producto y la cantidad (Por cada producto que se escanea se suma 1 más).

  - Estos datos son enviados y almacenados en la base de datos.

### Servidor de administración

  - Con un servidor de administración, los productos almacenados son mostrados en una página web para que el usuario pueda interactuar con estos. 

  - Desde este medio, se pueden visualizar, añadir, editar, eliminar y buscar productos en la base de datos.

  - Todos los cambios realizados se actualizarán en la DB.

## 🔧 Desarrollo 

<br>

La jerarquía de carpetas usadas es la siguiente:

<br>

```
main
.
|- GithubImages
|- Hardware
|   |-- Kicad
|       |--- Versiones
|- Modelos3D
|   |-- Versiones
|- Software
|   |-- Arduino_IADataset
|       |--- Versiones
|   |-- PaginaWeb
|       |--- Versiones
|- READ.ME
|- LICENCE

```
<br>

Las carpetas principales son:

### Hardware

Aquí se encuentran los archivos hechos en kicad. Estas son las placas diseñadas y usadas durante el transcurso del desarrollo.

### Modelos3D

Aquí se encuentran los archivos hechos en tinkercad. Se incluyen archivos de base que se usaron para el montaje de motores, placas, cinta, entre otros elementos.

### Software

Aquí se encuentran dos carpetas diferentes, estas son:

<br>

  - **Arduino_IADataset** (Código arduino y código del servidor de procesamiento)

<br>

  - **PaginaWeb** (Código del servidor de administración)

<br>


> [!NOTE] 
> Cada carpeta tiene una subcarpeta de versiones, para poder analizar el avance de cada sección.


## 📸 Galeria

## 🌟 Autores

acomodar esto bien (me faltan 2)

[Altamirano Valentino]()

[Avila Tomas](https://github.com/VMASPAD)

[Campusano Federico](https://github.com/FedeCampu1)

[Sebastian Galeotti]()

[Vallone Fabrizio](https://github.com/FabrizioVal)

## 🔒 Licencia

[Licencia MIT](https://github.com/FabrizioVal/Proyecto_G.I.A.I./blob/main/LICENSE)

<br>

<br>

---

<div align="center">
  <a href="#user-content-introducción">🔼 Volver al inicio</a>
</div>









Ultima seccion, adjuntar PDF del proyecto y repo
