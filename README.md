# Componentes y conectores - Parte I

### Andrea Valentina Torres Tobar
### Andres Serrato Camero

## Ejercico introductorio

El ejercicio se encuentra en el archivo [EjercicioIntroductorio.zip](EjercicioIntroductorio.zip)

## Blueprint

Se implementaron los metodos vacios en todas las clases que eran necesarios para su ejecución, como:

![alt text](/img/img.png)

Además, se implementó la clase InMemoryBlueprintPersistence para que se acople al diagrama de clases planteado en el ejercicio.

![alt text](/img/img_1.png)

Finalmente, se implementaron las pruebas unitarias para cada uno de los métodos de las clases, con el fin de verificar su correcto funcionamiento.

![alt text](/img/img_2.png)

Por otro lado, para qué se puede ejecutar mediante Spring, se creó una instancia de BlueprintServices, rectificando funcionalidades de registrar planos, consultar planos, registrar planos específicos.

![alt text](/img/img_3.png)

Además de eso, para que no hubiera conflicto en las inyecciones, se colocó @Qualifier, para que se pueda inyectar la clase InMemoryBlueprintPersistence.

![alt text](/img/img_5.png)

Dando como resultado:

![alt text](/img/img_4.png)


### proceso de filtrado

se realizo la implementacion de una interfaz `BlueprintFilter`
![alt text](/img/image.png)

despues creamos el filtro de redundancias `RedundancyFilter` 
![alt text](/img/image-1.png)

implementamos de igual forma el filtro de submuestreo `SubsamplingFilter`
![alt text](/img/image-2.png)

despues de esto modificamos `BlueprintsServices` para añadir el filtro

![alt text](/img/image-3.png)

procedemos a realizar una prueba con puntos redundantes 

![alt text](/img/image-4.png)

y de esto obtenemos 

![alt text](/img/image-5.png)


TEST de filters

![alt text](/img/image-6.png)