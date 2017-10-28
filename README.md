### Freelancer

* **HTML:**

Dentro del `head`se incluye el titulo de la pestaña que se muestra en el navegador, el enlazamiento con el archivo `css` y el linkeo de los iconos y las fuentes. 

Luego de esto comencé a incluir la barra de navegación dentro del body, la que a su vez se encuentra en un elemento `header` dentro de este header va el titulo dentro de un `p` que corresponde a START BOOTSTRAP, para la barra de navegación se incluye todo dentro de una etiqueta `nav`, a esta etiqueta en particular se le asigna el `id menu`, lo que corresponde al menu que se encuentra en la esquina superior derecha de la página, donde podemos encontrar los enlaces a la sección portfolio, about y contact. 

Al finalizar el `header` se crea una `section`, esta incluye una clase llamada `bigtitlebar` esto corresponde a la parte de la pagina donde hay una imagen de un trabajador como foto de perfil, en esta parte se encuentra el titulo `start bootstrap` y ademas las palabras Web Developer - Graphic Artist - User Experience Designer, dentro de esta sección se incluye una estrella con dos lineas blancas, al detallar el codigo de `css` explicaré como fue que lo realicé. 

Creé una nueva `section` la que incluye un `p` dentro de un `div`para dar el titulo `portfolio` y varios `divs`más para poder trabajar mejor las barras con el icono de la estrella y además las imágenes, ya que cada imagen es un `div`por separado. Todo esto va dentro de un `div`contenedor, al que le asigno el fondo color blanco para poder encerrar las imágenes y el texto. 

Creo otra `section` con una class llamada `aboutbar` en la que nuevamente se encuentra un titulo grande (en este caso about) y el icono de la estrella en medio de dos líneas. Además de esta `section`creé un `div`contenedor, el que encierra dos parrafos y otros dos divs, un párrafo a cada lado, bajo estos párrafos creé una etiqueta `button`la que corresponde a un botón llamado `download theme`, este boton tiene un icono en su interior, que corresponde a `fa-download`. 

La última sección corresponde a la parte `contact me` para esta sección se crearon dos `div`contenedores, uno para darle estilos al  fondo y poder encerrar todo dentro de él y otro que contuviera el formulario. 
El primer `div`contiene el título de la sección y la conocida estrella con sus barras laterales. 
El segundo contiene el formulario, dentro de este div se creo la etiqueta `form` la que tiene un `input`para cada ingreso de información.
Además del formulario esta parte también tiene un boton, el que se crea mediante la etiqueta `button`y solo tiene la palabra `send`dentro. 

Para finalizar el `html`se creó un footer, este footer tiene tres parrafos, uno corresponde a la locación de la empresa, el otro a las redes sociales y el último, información adicional about freelancer. 
En esta parte se crearon varios `div`el principal es el contenedor, abarca toda la informacion que está dentro del `footer` después de este `div`contenedor se hicieron tres que son "subcontenedores" uno para cada columna de información, para poder alinear de mejor forma todas las partes de la página, sobre todo la de los íconos de redes sociales, para el cual cree un `div`para cada uno. 


* **CSS:**

Para explicar más o menos como le di los estilos a cada parte lo iré explicando paso por paso, para hacerlo más ordenado.

Partí con un selector universal el cual tiene asignado 0 como valor de `margin y padding`esto hace que la página ocupe todo su ancho sin quedar con espacios en blanco.

`#title` corresponde al titulo `start bootstrap` ubicado al lado superior izquierdo de la página.

`header` como lo comentaba en `html`este header encierra el color de fondo y el menú de navegación ubicado al lado superior derecho de la página.

`header nav`le da los estilos a la barra de navegación. 

`header nav a`le da los estilos en particular a los "enlaces" que se encuentran dentro del menú de la barra de navegación, engloba el color de texto y la posición de este. 

`header nav a:hover`hace que al pasar el mouse por encima del menú, este cambie de color, no supe como hacerlo igual que en la página original, por este motivo es que solo hice que quedara como un elipse el color de fondo y así que no se viera tan cuadrado por medio de `border-radius`. 

`#bigtitlestarbar` corresponde a la barra que se encuentra al lado izquierdo del ìcono de la estrella, ya que no supe usar la pseudo clase :after :before lo hice con un background color #fff para que quedara como una línea y luego le fui dando la posición, lo mismo ocurre con la estrella que se llama `bigtitlestar`y con la barra que va a la derecha de la estrella, hice lo mismo para cada estrella y barras de la página.

`#bigtitle`corresponde al título en la parte del perfil, me refiero a perfil por la imagen del trabajador que aparece ahí.

`#bigtitlebar`creé este `id`para poder darle estilo y un fondo a esta parte de la página.

`div.profile img` corresponde a la imagen del trabajador.

`.profiletext`corresponde al texto debajo de la imagen del perfil (Web Developer - Graphic Artist - User Experience Designer) 

`#portfolio`con este id se le da estilo solamente al titulo de esta sección.

`#portfoliobar #portfoliostar #portfoliobar-right`corresponden a la estrella y ambas barras laterales, como expliqué más arriba se crearon con un background del color que correspondía. 

`#white`este id le da al estilo que encierra toda la sección portfolio, de este modo hago que todo el texto y las imágenes queden dentro. 

`div .images img` le da los estilos a todas las imágenes de la sección portfolio.

`div .images img:hover`permite que al pasar el mouse por encima de cada imagen, esta cambie a un color más opaco, ya que no pude hacer que todas cambiaran al color `#18bc9c`

`.aboutbar`al igual que en clases anteriores, por medio de esta clase hago que encierre todos los elementos de la sección about, tales como los párrafos que van debajo del título y ademñas el botón de "donwload theme". 

`#abouttitle`le da estilo al titulo about solamente. 

`#aboutstarbar #aboutstar  #aboutstarbar-right` le da estilo al icono de la estrella y sus barras laterales. 

`#container .paragraphleft y #container .paragraphright` le dan el estilo y posición a los dos párrafos debajo del título about.

`.download-button` le da el estilo al botón que aparece en la sección about. `.download-button:hover`hace el resto, que al pasar el mouse por encima cambie el color de fondo. 

`#contacttitle`solamente le da el estilo al título de la sección contact me.

`#contactstarbar #contactstar y #contactstarbar-right`corresponden al estilo de la estrella y sus barras laterales. 

`#white-b`este id tiene este nombre ya que más arriba usé un id llamado `#white` al igual que en casos anteriores, este solamente corresponde al color de fondo y hace que todo quede encerrado en él, en este caso todo lo que se encuentra en la sección contact me

`.send-button`corresponde al botón de enviar que se encuentra debajo del formulario, 
`.send-button:hover`hace que al pasar el mouse por encima, este botón cambie de color. 

`input[type=text]`esta parte selecciona todo el texto que se encuentra dentro del formulario, hace que cambie el estilo de las líneas que lo encierran. 

`form:focus` saca la linea del formulario. 

`footer`contiene todo lo que contiene el final de la página, la locación, las redes sociales y eñ about freelancer. 

Por medio de la clase `.div-foot`hice que todos los `h3`se alinearan y quedaran todos ordenados de inmediato. 

`.div-foot p` da el estilo a todos los parrafos del footer, alineando el texto y dejándolo centrado. 

`.div-foot div`hace que todo quede como tipo inline.

`.icon` esta parte le da el estilo y la circunferencia que encierra a los iconos de las redes sociales. 

`a.icon:hover`hace que al pasar el mouse por encima se cubra a toda la circunferencia y no solamente a los iconos y cambia el color de fondo de los mismos. 

`.around`solamente alinea el último titulo que es "about freelancer". 

