# FirstProject
Proyecto básico de Git y Github

Principalmente, se inició clonando el repositorio de GitHub donde se alojaba una plantilla guía de HTML para lograr desarrollar nuestra web tributo con base en esa plantilla.
### 	El comando en Git para clonar el repositorio es $ git clone <URL del repositorio a clonar>

Luego de revisar la estructura propuesta de la plantilla, logre entender que se manejó mediante una librería la cual era W3School para dar una mejor visualización acorde. De igual manera, decidí cambiarla por la librería Bootstrap la cual ya tengo un poco de experiencia en utilizarla.

# Estructura de HTML
## Estándar principal de un documento de HTML
```
<!DOCTYPE html>
<html>
  ‘En este campo va todo el código’
</html>
```
Esta parte del código es significativo para empezar un documento HTML, se basa en identificar que versión de HTML que usaremos posteriormente, en este caso utilice HTML5 que es la versión más reciente y semántica para poder leer mejor el código. 

## Head del documento HTML 
```
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <!-- Importamos recursos externos -->
  <link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Open Sans">
  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.2.1/dist/css/bootstrap.min.css" rel="stylesheet"
    integrity="sha384-iYQeCzEYFbKjA/T2uDLTpkwGzCiq6soy8tYaI1GyVh/UjpbCx/TYkiZhlZB6+fzT" crossorigin="anonymous">
  <!-- Importamos recurso css para los estilos-->
  <link rel="stylesheet" href="css/index.css">
  <link rel="stylesheet" href="fontawesome-free-6.2.0-web/css/all.css">
  <link rel="shortcut icon" href="img/logoPestaña.png" type="image/x-icon">
  <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.2.2/dist/js/bootstrap.bundle.min.js"></script>
  <title>Amasijos Tradicionales</title>
</head>
```
Prácticamente en esta parte del código se importan los diferentes recursos que se utilizaron durante la construcción de la página web tributo, los recursos que se utilizaron fueron la fuente de Google Fonts, la librería Bootstrap para algunas funcionalidades, la ruta local de los estilos de la página web, la ruta local de los iconos descargados de Font-awesome y por último agregando el logo y título en la parte de la pestaña.

## Header del documento HTML 
```
<!-- START Boostrap -->
  <div class="part-body container p-0" style="max-width:100%;">
    <!-- Header -->
    <section class="header-fixed">
      <header class="part-header p-10">
        <nav class="nav-header">
        'etiquetas correspondientes para poder visualizar el menú'
        </nav>
      </header>
    </section>
  </div>
<!-- END Header -->
```
Esta parte del código incluida en la etiqueta <body></body> se le agregó un contenedor para tener control del ancho máximo para que no se desbordara algún contenido, en ella nos encontramos el encabezado del documento que incluye el logo, nombre de la empresa y un menú para poder navegar a distintas vistas dentro de la web. Además, en el menú se encuentra una parte desplegable que abarca variadas recetas de una sola sección llamada recetas, con la ayuda de Bootstrap se logró implementar para una mejor facilidad de uso, comparándolo esta parte con el Wireframe y Mockup anteriormente realizado, decide añadir esa funcionalidad sin haberla incluido en el diseño. 

Por último, el encabezado está incluido en una sección principal para poder tener el menú fijado en la Ventana y siempre tener la facilidad de interactuar con el menú sin necesidad de volver hasta la parte superior, al principio sé ME complico, ya que, dos pociones entraron en conflicto y no me daba el resultado que quería, revisando el código logre encontrar el bug y solucionarlo lo cual logre obtener lo que esperaba.

## Slider de imágenes 
```
<!-- Slider image header -->
   <div id="carouselExampleCaptions" class="carousel slide" data-bs-ride="carousel">
     <div class="carousel-indicators">
      'etiquetas correspondientes que brinda Boostrap para el carusel de imagenes'
     </div>
  </div>
<!-- END Slider image header -->
```
Esta parte del código incluida en las etiquetas ```<body><main></main></body>```, abarca la sección de un carrusel de imágenes alusivas a los amasijos tradicionales la cual puede llevar a cabo con la ayuda de Bootstrap, el desafío fue poder cambiar gran parte de su estructura y estilo para lograr lo propuesto en el diseño, pero finalmente lo logre con la ayuda de la herramienta de desarrollador que nos ofrece el navegador para revisar toda la estructura de HTML y CSS.

## Sección de información sobre el significado de los amasijos
```
<!-- History entry -->
  <div class="content-first container" style="max-width: 90%;">
    <div class="content-first-left text-center">
       'etiqueta para la imagen alusiva a la sección'
    </div>
    <div class="content-first-right">
       'etiquetas para el título y descripción sobre la sección'
    </div>
    <hr class="m-0">
  </div>
<!-- END HISTORY ENTRIES -->
```
Esta parte del código incluida en las etiquetas ```<body><main></main></body>```, es un contenedor con máximo de ancho que tiene como propósito informar a los usuarios sobre “¿Qué son los amasijos?” y esa información descriptiva envuelve alrededor una imagen alusiva sobre el tema principal.

## Sección del video descriptivo 
```
<!-- Video -->
  <section class="m-5 p-5">
    <iframe>
      'video desciprivo de youtube'
	  </iframe>
  </section>
<!-- END Video -->
```
Esta parte del código incluida en las etiquetas ```<body><main></main></body>```, es una sección que tiene como propósito transmitir por medio de un video en YouTube los productos tradicionales en Colombia.

S## ección de la historia de los amasijos y sus productos 
```
<!-- History all entry -->
   <div class="container pt-5 pb-5" style="max-width: 90%;">
     <div class="row mt-5">
       <div class="col-8 text-center">
         'etiquetas para el título, descripción sobre la sección y enlace'
       </div>
      <div class="text-center col-4">
        'etiqueta para la imagen alusiva a la sección'
      </div>
    </div>
   </div>
<!-- END History  -->
```
Esta parte del código incluida en las etiquetas ```<body><main></main></body>```, es un contenedor con máximo de ancho que tiene como propósito informar a los usuarios sobre “La historia de los amasijos en Colombia” esa información descriptiva se encuentra al lado de una imagen alusiva sobre el tema y un enlace para visualizar mejor la información. Con la ayuda de las filas y las columnas que brinda Bootstrap para controlar elementos seguidos como en este caso. Luego se incluyen imágenes representativas sobre algunos amasijos tradicionales.


## Sección de las recetas de los amasijos
```
<!-- Recetas all entry -->
   <div class="container pt-5 pb-5" style="max-width: 90%;">
     <div class="row mt-5">
       <div class="col-4 text-center">
         'etiqueta para la imagen alusiva a la sección'
       </div>
       <div class="content-middle col-8 text-center">
         'etiquetas para el título, descripción sobre la sección y enlace'
       </div>
     </div>
   </div>
   <div class="container pt-5 pb-5" style="max-width: 90%;">
     <section class="content-third">
       <div class="row pt-3">
         <div class="text-center col-4">
           'etiqueta para la imagen alusiva al producto'
         </div>
         <div class="content-last p-3 col-8">
           'etiquetas para el título y descripción del producto'
         </div>
       </div>
       <div class="row pt-5">
     </section>
   </div>
<!-- END Recetas  -->
```
Esta parte del código incluida en las etiquetas ```<body><main></main></body>```, es un contenedor con máximo de ancho que tiene como propósito informar a los usuarios sobre “Las recetas comunes de los amasijos” esa información descriptiva se encuentra al lado de una imagen alusiva sobre el tema y un enlace donde redirige a una nueva vista con información más detallada. Con la ayuda de las filas y las columnas que brinda Bootstrap para controlar elementos seguidos como en este caso. Luego se incluyen imágenes representativas sobre algunos amasijos tradicionales.

## Sección Footer del documento HTML
```
<!-- Footer -->
   <footer class="part-footer">
     <div class="container" style="max-width: 100%;">
      'etiquetas para el logo, iconos de redes, ubicación y email corporativo'
     </div>
   </footer>
<!-- END footer -->
```
Esta parte del código se describe como pie de página de una web, en esta última sección abarca información puntual sobre la empresa seguida de las diferentes redes sociales con las cuales se puede contactar igualmente que el correo empresarial y finalmente la ubicación donde se encuentre la empresa actualmente.

