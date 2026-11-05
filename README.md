# ATLAS HUMANO

**Un planeta. Muchas vidas. Preguntas compartidas.**

> Una forma de no estar tan solos frente a las preguntas.

Ensayo documental y visual interactivo donde la cartografía satelital se convierte en caleidoscopio y abre preguntas sobre geología, biodiversidad, convivencia, salud, derechos, cooperación y futuro.

**[Explorar el atlas](https://juanmanueltorres-creator.github.io/atlas-humano/)** · [Instagram @geoespacialcode](https://www.instagram.com/geoespacialcode/)

## Edición 5.2

- **36 historias, siete actos.** El nuevo acto «Encontrarnos» investiga conexión social, restauración comunitaria, bosques y cooperación internacional.
- **Manifiesto en ocho escenas** con lectura manual o reproducción opcional. El recorrido no avanza solo por defecto y se puede cerrar con Escape.
- **Interacción por movimiento de mouse**: el caleidoscopio responde suavemente sin mantener presionado. En pantallas táctiles, arrastrar sigue funcionando. Respeta la preferencia `prefers-reduced-motion`.
- **Sin cambios en el motor de mosaicos optimizado 5.1.** El efecto de movimiento del mouse no solicita más teselas; solo desplaza la textura ya dibujada.
- **Compartir preguntas:** desde cada historia se puede copiar un vínculo directo. No recopila comentarios ni datos de visitantes.
- **Modo mapa** para distinguir el territorio real de la representación artística.

## Cómo ejecutar

Abrí `index.html` con un navegador moderno y conexión a Internet. Es una aplicación estática: HTML, CSS, JavaScript y Canvas 2D. No requiere React, servidor de aplicaciones ni compilación.

La navegación incluye el índice por temas, capítulos anterior/siguiente, botón «Descubrir», mapa sin espejos, cambio de simetrías y pausa. El manifiesto se abre desde el botón ✳ en la cabecera. En computadoras, el movimiento del mouse afecta únicamente el caleidoscopio; para mover el mapa real o navegar con precisión se conserva el arrastre.

## Estructura y fuentes

- `index.html`: aplicación y relatos incluidos como datos estructurados.
- `data/catalogo.csv`: catálogo consultable de las 36 historias.
- `data/fuentes.json`: recopilación editorial de datos y fuentes (no se carga automáticamente).

**Las fechas, coberturas, denominadores y límites importan.** Una estadística mundial no describe automáticamente el territorio que se observa en pantalla. Para los cuatro capítulos nuevos se consultaron, entre otras fuentes:

- [OMS · Comisión sobre conexión social (2025)](https://www.who.int/groups/commission-on-social-connection): estimación mundial de soledad.
- [Banco Mundial · Bosques en Nepal (2025)](https://www.worldbank.org/en/country/nepal/publication/may-the-forest-be-with-you-mapping-nepal-s-forest-landscapes-and-livelihoods): evolución forestal y papel de la gestión comunitaria, con limitaciones.
- [Banco Mundial / FAO · Superficie forestal en Costa Rica](https://data.worldbank.org/indicator/AG.LND.FRST.ZS?locations=CR): porcentaje nacional, no índice de biodiversidad.
- [Secretaría del Ozono / Naciones Unidas](https://ozone.unep.org/facts-and-figures-ozone-protection): proyecciones condicionales de recuperación.

El proyecto diferencia **dato, interpretación editorial y pregunta abierta**. No transforma correlaciones en pruebas causales ni genera cifras mediante IA. Las consultas a Banco Mundial y NASA EONET son opcionales y requieren conexión.

## Atribuciones y condiciones de uso

- Imágenes de **Esri World Imagery** y proveedores, bajo sus respectivos términos. Las imágenes no pertenecen al proyecto.
- © [OpenStreetMap contributors](https://www.openstreetmap.org/copyright); respetar su [política de uso de mosaicos](https://operations.osmfoundation.org/policies/tiles/).
- Tipografías de Google Fonts y sus respectivas licencias.
- El repositorio público **no contiene licencia abierta explícita** para el código. La visibilidad pública no implica permiso general de reutilización. Revisar licencias de datos e imágenes antes de redistribuir o comercializar.

## Alcance

Obra de divulgación artística y pensamiento crítico. No es un sistema de decisión pública ni un producto comercial. Las interpretaciones son editoriales, las cifras están fechadas y las fuentes se ofrecen para verificar o profundizar.