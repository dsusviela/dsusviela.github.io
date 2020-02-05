Hace un tiempo una amiga me pregunto si su bolso de 60 litros podía viajar como equipaje de mano y así evitarse el proceso tedioso del despacho. Mi respuesta era lo que ella menos esperaba; “Depende”. Y si, es la verdad. Cada aerolínea tiene sus propias normas sobre los distintos tamaños de lo que constituye “equipaje de mano”. Incluso cuando se trata del mismo modelo de avión, no se pueden poner de acuerdo con un tamaño estándard. Ella tenía que tomar una decisión al tener que determinar si intentaba viajar con ese bolso y arriesgar tener que pagar el despacho o comprar otro un poco mas chico el cual probablemente no se ajustaba a sus necesidades. Y ni hablar de la cadena de decisiones que surgen a partir de la segunda opción. Mi amiga estaba siendo **víctima de la falta de convención** y no lo sabía.

* * *

## Libremonos de las decisiones innecesarias

En el mundo del software existe un concepto el cual se llama “Convención sobre configuración”, quizás más conocido en inglés por “Convention over configuration” el cual busca simplificarnos la vida. El objetivo es simple, decrecer la cantidad de decisiones de un programador mediante el acuerdo de buenas prácticas, lo cual libera a este para que se concentre realmente en los problemas a resolver.

¿Quién determina estos acuerdos? Por lo general los determinan la comunidad de programadores detrás de la filosofía de la tecnología en la que se está trabajando. ¿Esto quiere decir que la tecnología en cuestión no anda si no se siguen estas pautas? No realmente, el conjunto de reglas puede ser sobrescrito pero se pierden varios de los beneficios si se ignoran.

## Caso de estudio: Rails

Rails, se basa fuertemente en este principio, al punto de llamarlo uno de sus [nueve pilares](https://rubyonrails.org/doctrine/). Entre las convenciones más notorias del framework se encuentran las siguientes;

 - Nombrado y ordenamiento de los archivos y carpetas de una aplicación: Esta establecida la jerarquía de archivos que debe tener una aplicación.

 - Nombrado de las tablas en la base de datos: Rails toma las clases y les asocia una tabla con el nombre de la clase en plural.

 - Carga automática de las clases: Rails detecta cuando un objeto de una clase es llamado y busca dicha clase en las rutas especificadas en el archivo `config.autoload_paths`

 - En las tablas de las bases de datos Rails pone por defecto `id` como la clave primaria y las claves foráneas las nombra con el nombre de la clase asociado y el sufijo `_id`.

 Existen muchas otras convenciones en el framework, pero los ejemplos demotrados sirven para probar que *realmente se elimina la toma de decisiones intradescendentes*. Todas estas simplificaciones permiten el desarrollo más rápido, muchas operaciones comunes son automatizables y al existir un acuerdo tácito se ahorra la comunicación innecesaria. Este último punto es extremadamente fuerte ya que permite mayor entendimiento por otros desarrolladores externos, que al conocer la convención se pueden llevar menos sorpresas.

## No todo es un arcoíris

Hay un cierto precio a pagar por todo esto. La curva de aprendizaje es un poco más inclinada para los desarrolladores que vienen de otras convenciones o de otros paradigmas. Obviamente, las convenciones no son todas iguales por lo que desarrolladores experimentados en una metodlogía pueden afrontar dificultades al tener que cambiar la mentalidad en nuevos ambientes. De la misma forma, las personas acostumbradas a la configuración pueden ver la falta de explicitud confusa. 

Otro punto en contra es el hecho de que cada aplicación es única, esto significa que alejarse de los modelos preestablecidos es casi inevitable para llevar acabo ciertas funcionalidades. El determinar cuando uno se debe alejar de la convención es una tarea para nada trivial incluso para los más expertos.

## En resumidas cuentas...

A pesar de los puntos mencionados, el principio de Convención sobre Configuración tiene gran poder al simplificar la vida de los programadores. Muchos aclaman que este es uno de los grandes motivos por el cual Rails logró ser lo que es. Y sin embargo es cierto que a veces es necesario tomar las riendas e ir en contra de lo establecido para seguir creando aplicaciones que destaquen. De todas formas, el tener convenciones claras ahorra no solo trabajo pero comunicación sobre decisiones banales. Nos hace la vida más fácil, lo que lleva a que podamos desarrollar mejor.