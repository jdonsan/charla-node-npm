# Bienvenid@s al mundo de nOOOde

Hay un tipo de charlas que me gustan muchos y son las charlas temáticas. Hace unos meses vi una
charla de Cristina Fernandez sobre Desarrollo Front con temática en Harry Potter y me gustó tanto
que he decidido copiarle la idea. 

Cuando Isra y el equipo de formación de Adalab me propuso que os hablase sobre Node y NPM, estuve 
reflexionando sobre lo grande y diverso que se estaba convirtiendo todo el desarrollo realtivo a 
esta plataforma y me dí cuenta que tenía muchos parecidos al mundo que han creado en Hora de Aventuras,
el mundo de OOO. Un mundo lleno de seres diversos que inexplicablemente en harmonía aun estar todos
un poco locos.

Espero que mis amigos de Hora de Aventuras y yo, podamos explicaros en estas dos horas de que trata
está cosa tan divertida que es NodeJS.

## Slide: ¿Quién soy?

Me llamo José Antonio Dongil. Soy desarrollador Web. Desarrollo tanto aplicaciones front, como
aplicaciones con NodeJS. Podéis encontrarme y preguntarme todo lo que queráis en mi blog (El Abismo de Null)
y en mi twitter (@jdonsan).

Todos los recursos que podamos usar hoy, podréis encontrarlos en mi github jdonsan.

Empecemos :)

## Slide: Presentación bloque introducción

Hablando con Isra me comentó que era necesario que hicieramos una clase lo más sencilla y entendible posible
y preparando entre los dos la planificanción, dividimos la explicación en 4 bloques. Este primero es una pequeña
introducción donde pondremos un poco de contexto y el ámbito donde nos vamos a mover que difiere un plín de lo 
que estáis acostumbradas a hacer en vuestro día a día.

## Slide: Un viaje de cliente a servidor

Y lo primero que vamos a hacer es un viaje. Un viaje a una zona nueva. Parecida a la que conoceis pero nueva. Dejamos
el mundo del desarrollo front (solo por dos horas) y viajaremos al mundo del servidor.

Cuando un cliente o una persona necesita una solución de software, lo primero que los desarrolladores solemos hacer es
decidir que arquitectura queremos que nuestra aplicación tenga. Al igual que los arquitectos de casas, nosotros tenemos
que decidir donde colocar cada cosa y por qué. 

Por lo general, muchos desarrolladores ya se han encontrado con el mismo problema y para soluciones pequeñas y medianas, 
hemos descubierto que una arquitectura parecida a esta es la idonea. Es lo que se conoce como arquitectura cliente-servidor

La idea subyace en encontrar un equilibrio entre la seguridad de una aplicación y la escalabilidad. Si conseguimos equilibrar
estos conceptos conseguimos aplicaciones muy potentes. La idea de escalabilidad trata de que si yo puedo hacer que
los ordenadores de los usuarios trabajen más que los mios, significa que yo voy a poder hacer las cosas más rapido
y que el usuario tendrá una mejor experiencia con nuestra aplicación. 

Ese es el trabajo que haceis los front. Intentais que  una gran cantidad de tareas pueda hacerlas el navegador 
de vuestro usuario: renderizar HTML, mostrar datos, ordenar datos,
filtrar, transformar y todo esto presentandolo d euna forma amigable, usable y accesible.

Por otra parte, los sistemas cliente, necesitan de un centro de control, un servidor. Hay datos, información que para los
clientes o dueños de la aplicación es importante que se mantenga a recaudo. Tambien soluciona un problema de comunicaciones.
Por ahora dos navegadores no tienen la tecnologia suficiente para comunicarse entre ellos. Necesitan de un servidor. Una 
aplicacion cliente siempre suele necesitar datos de un origen y enviar las interacciones del usuario para guardarlas.

# Slide: ¿Qué nos aporta el Servidor?

Por lo tanto. Los clientes se encargan de hacer peticiones y los servidores de responderlas.
Un servidor tiene muchas posibilidades, las 3 más comunes son: 

* Recibir peticiones
* Jugar con esas peticiones
* Responder a esas peticiones.

## Slide: ¿Cómo es el mundo de Node?

Una vez que hemos hecho ese viaje, descubrimos que NodeJS es un mundo de tipo Servidor (o Backend como también es llamado).
NodeJS es una plataforma que nos proporciona todo lo necesario para cumplir con esas 3 tareas, recibir peticiones,
jugar con esas peticiones y responder a esas peticiones.

NodeJS es un mundo bastante joven que se descubrió en el AÑO, por NOMBRE. Y que intentaba solucionar un problema
que tenian el resto de mundo del tipo Servidor como Java o .NET que son el escalar peticiones de una forma más rapida
y con un menor uso de recursos.

## Slide: ¿Cómo empezamos?

Node cuenta con un numero grande de habitantes. La mejor forma de visitarlos es instalando Node en nuestros equipos

* Forma de instalarlo en ubuntu y que lo instalen
* Comprobar en el terminar que se ha instalado correctamente.

## Slide: V8

Una vez que hemos instalado NodeJS, Vamos a mostrar algunos de los componentes que podemos encontrar. Lo que hemos
hecho al instalar NodeJS es instalar una pieza clave e nuestro ordenador. Hemos instalado un motor que procesa JavaScript
llamado v8. V8 permite transformar código JavaScript en codigo que entienda el ordenador. V8 es justamente el motor que usable
Chrome y que el equipo de Google hico Open Sources para que otras personas lo pudiesen usar a su antojo. Uno de los usos
que se le dio es como compilador para NodeJS.

## Slide: JavaScript

Y si V8 entiende JavaScript, significa que nuestras aplicaciones en NodeJS están escritas con este lenguaje 
que ya habreis sufrido. Una de las cosas por las que NodeJS se está haciendo tan famoso es porque se escribe con JavaScript.
Muchos desarrolladores Front, se veian frutrados por no poder participar en otras partes del desarrollo. Si existiesa 
una plataforma como Node, esa friccion se acabaría y los equipos pueden convertirse en más disciplinares. Además 
que podemos reutilizar codigo porque si por ejemplo yo hago una librería para recorrer arrays, puedo hacer uso de ellas
tanto en Front como en Back. Por lo que contar con un lenguaje como JavaScript es un valor estrategico.

## Slide: Módulos

Los módulos o paquetes, son los verdaderos habitantes de NodeJS. Los modulos son porciones de código escritos en JavaScript 
que pueden ser usados en NodeJS para hacer un sin fin de funcionalidades para que nosotros las tengamos que volver a desarrollar. Tenemos
que ver a los modulos como cajas negras que nos permiten hacer cosas. En NodeJS existen varios tipos de módulos, por ejemplo
tenemos módulos nativos, que son los que vienen instalados por defecto con Node y que nos dan funcionalidad básica, módulos
propios, que son nuestra propia aplicación (todo en Node es un Modulo, recordadlo siempre) y modulos de terceros, que son 
módulos que han hecho otras personas y que nosotros podemos usar.

## Slide: Gestores de módulos

Los modulos en NodeJS viven en el Reino NPM. NPM significa Node Package Manager, es decir gestor de paquetes de node. NPM es
una herramienta de linea de comandos que nos permite crear módulos, buscar módulos y obtener otros módulos para que podamos
usarlos en nuestra aplicación.

## Slide: Presentación módulo de NPM
 
EN este segundo bloque vamos a ver como usar esta herramienta para trabajar con módulos.

## Slide: Creando un nuevo módulo

Explico cómo lanzar npm init y la estructura de package.json.

## Slide: package.json

Explico package.json

## Slide: Instalando dependencias locales

Explico npm install sin -g 

## Slide: Instalando dependencias global

Explico npm install -g

## Slide: Diferencia entre dependencias de desarrollo y de producción: explico el uso de:
npm install --save
npm install --save-dev


## Slide: Eliminando dependencias 

Explico npm uninstall

## Slide: Ejemplo

## Slide: Presentación módulo de NodeJS (aprox. 20 min)
 
El objetivo de este módulo es es saber cómo empezar en Node y cómo desarrollar una pequeña API.
 
## Slide: Hola Mundo en Node

Hacemos un pequeño Hola Mundo para que vean que sigue siendo lo mismo que han aprendido sobre JavaScript. 

## Slide: Un mundo asíncrono

Explico que en Node todas las entradas/salidas son asíncronas como en cliente y cómo gestionarlo.

## Slide: Módulos de Node 

Explico que hace cada uno y cómo usarlo. Explico la API básica de cad auno.

## Slide: Path

## Slide: FileSystem

## HTTP

Explico también como levantar un servidor para que escuche llamadas por un puerto especifico

## Slide: Módulos externos: Express

## Slide: Presentación de la práctica
 
El objetivo es practicar todo lo aprendido durante la sesión.
 
Práctica: ¿Quienes son los personajes de Hora de Aventuras?: Tenemos una aplicación de cliente (Esta la daré yo hecha) que hace llamadas a una API para mostrar los personajes de Hora de Aventuras. Vamos a crear una API que permita obtener estos personajes desde servidor y que nos permita ordenarlos por edad