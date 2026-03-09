# Descripción del proyecto
Este es un trabajo que he hecho con HTML y Bootstrap. Es una página web para informar a la gente sobre una quedada de animación antes del partido Real Zaragoza vs Burgos CF en el Ibercaja Estadio.
La idea es que los aficionados sepan:

De qué va la previa (la Fan Zone y animar al equipo desde fuera).
Qué cosas vamos a hacer allí.
Cuándo y dónde hay que ir.

Cómo está organizada la página (secciones y columnas Bootstrap)

-Navbar (la barra de arriba):
Tiene un container para que quede centrada. No usa columnas, solo el menú con links a las secciones.
Solo un container con texto centrado. No tiene row ni columnas.
Sección "Previa en la Fan Zone" (antes "El evento"):
Usa un row con dos columnas:
col-md-6 → texto descriptivo
col-md-6 → foto del estadio

-Sección "Qué vamos a hacer" (actividades):
Un row con tres columnas:
col-md-4
col-md-4
col-md-4

-Sección "Información importante" (antes "Cuándo y dónde"):
Un row con dos columnas:
col-md-6 → lista con los datos (fecha, hora, etc.)
col-md-6 → foto de la afición animando

-Footer (el pie de página):
Un container con texto centrado. No usa columnas.

# Componentes de Bootstrap que he usado

-Navbar (con navbar-expand-lg, navbar-dark, bg-dark, fixed-top)
-Grid: container, row, col-md-*
-Cards para las actividades (card, card-body, card-title, h-100 para que queden igual de altas)
-List-group para la info del partido (list-group, list-group-item)
-Clases de espaciado: py-5, mb-4, mt-3, etc.
-Imágenes responsive: img-fluid + rounded
-Utilidades como text-center, text-muted

-Commit 1 – Estructura básica

Hice el HTML vacío, metí el link de Bootstrap por CDN, puse la navbar y la parte de arriba.
-Commit 2 – Grid y secciones

Añadí las tres secciones principales con row y columnas.
-Commit 3 – Componentes chulos

Puse las cards en la sección de actividades y el list-group en la info. Añadí clases para que quedara más bonito.
-Commit 4 – Arreglar la navbar fija

Le puse fixed-top a la navbar y padding-top al body para que no tapara el contenido de arriba.
-Commit 5 – Últimos retoques

Ajusté tamaños de fotos (max-height), espaciados y detalles pequeños.

# Lo que más me costó y cómo lo solucioné
Problema: Cuando puse la navbar fija (fixed-top), el texto del hero quedaba tapado por la barra y no se veía bien al entrar en la página.
Solución: Añadí esto en el <style>:
CSSbody {
  padding-top: 70px;
}
