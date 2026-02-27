<!DOCTYPE html>
<html lang="es">
	<head>
	  <meta charset="utf-8">
	  <title>Evento Real Zaragoza vs Burgos</title>
	  <meta name="viewport" content="width=device-width, initial-scale=1">

# Descripción del proyecto
El proyecto consiste en una página web estática informativa sobre un evento de animación previo al partido entre el Real Zaragoza y el Burgos CF, que se celebra en el Ibercaja Estadio (Zaragoza).
La web tiene como objetivo informar a los aficionados sobre:
En qué consiste el evento.
Qué actividades se realizarán.
Cuándo y dónde tendrá lugar.
Facilitar una navegación clara mediante un menú superior fijo.
Está desarrollada con HTML5 y Bootstrap 5 mediante CDN, utilizando un diseño responsive que se adapta correctamente a dispositivos móviles, tablets y ordenadores.

# Secciones usadas y número de columnas Bootstrap
La página utiliza el sistema de grid de Bootstrap basado en 12 columnas.
Navbar
Se utiliza un container para centrar el contenido.
No se emplea el sistema de columnas directamente en esta sección.
Hero
Se utiliza un container con texto centrado.
No usa row ni columnas.
Sección "El evento"
Se utiliza un row con dos columnas:
col-md-6 para el texto.
col-md-6 para la imagen.
En pantallas medianas o superiores ocupa 6 + 6 columnas (12 en total).
En móviles las columnas se apilan automáticamente.
Sección "Actividades"
Se utiliza un row con tres columnas:
col-md-4
col-md-4
col-md-4
En pantallas medianas o superiores ocupa 4 + 4 + 4 columnas (12 en total).
En móviles las tarjetas se colocan en vertical.
Sección "Cuándo y dónde"
Se utiliza un row con dos columnas:
col-md-6 para la lista informativa.
col-md-6 para la imagen.
Footer
Se utiliza un container con texto centrado.
No se emplea sistema de columnas.

# Componentes prediseñados de Bootstrap usados
En el proyecto se han utilizado los siguientes componentes de Bootstrap:
Navbar (navbar, navbar-expand-lg, navbar-dark, bg-primary)
Collapse para menú responsive (collapse navbar-collapse)
Sistema de grid (container, row, col-md-*)
Cards (card, card-body)
List Group (list-group, list-group-item)
Navbar toggler (navbar-toggler)
Clases utilitarias de espaciado (py-4, mb-3, mt-3)
Clases de imagen (img-fluid, rounded)
Clase fixed-top para fijar la barra de navegación

# Descripción de los commits y mejoras implementadas
Commit 1 – Creación de la estructura base
Se creó el archivo HTML con la estructura básica del documento.
Se añadió Bootstrap mediante CDN.
Se implementó la navbar y la sección principal (hero).
Commit 2 – Implementación del sistema de grid
Se añadieron las secciones “El evento”, “Actividades” y “Cuándo y dónde”.
Se organizó el contenido utilizando row y col-md-*.
Se comprobó el correcto funcionamiento responsive.
Commit 3 – Implementación de componentes Bootstrap
Se añadieron tarjetas (Cards) en la sección de actividades.
Se incorporó un List Group para organizar la información del evento.
Se mejoró la estructura visual con clases utilitarias.
Commit 4 – Mejora de diseño y usabilidad
Se añadió la clase fixed-top a la navbar.
Se ajustó el padding-top del body para evitar que el contenido quedara oculto.
Se mejoraron los espaciados y el ajuste visual de imágenes.
Commit 5 – Optimización final
Se revisó el diseño en diferentes tamaños de pantalla.
Se comprobó el funcionamiento del menú desplegable en móvil.
Se ajustaron detalles visuales como el tamaño máximo de imágenes.

# Mayor dificultad encontrada y solución
Dificultad
Al fijar la barra de navegación con fixed-top, el contenido inicial quedaba oculto debajo de la navbar.
Solución
Se añadió una regla CSS en el body:
body {
  padding-top: 70px;
}
De esta forma se compensa la altura de la barra de navegación y el contenido se muestra correctamente desde el inicio.
