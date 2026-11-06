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

## Sonido opcional (5.3)

La opción **♫ Escuchar** añade paisaje sonoro generado localmente con Web Audio API y lectura de capítulos o escenas del manifiesto mediante `SpeechSynthesis` del navegador.

- El ambiente se intenta iniciar al entrar; si el navegador bloquea autoplay con sonido, comienza en el primer clic, toque o tecla. La voz siempre es voluntaria.
- La voz, el ritmo y el volumen pueden ajustarse; la calidad de voz depende del navegador y de las voces instaladas.
- La música reduce su volumen durante la narración.
- Los textos siempre permanecen disponibles sin sonido; no se recopilan ni envían grabaciones.
- El caleidoscopio y la navegación siguen funcionando sin audio. En segundo plano, la reproducción se detiene.

**Limitación:** esta versión utiliza síntesis de voz del navegador y no audio profesional grabado. Puede haber diferencias entre dispositivos. No representa una narración sincronizada con subtítulos.


## Paisajes sonoros por capítulo · 5.4

El Atlas genera **36 variaciones musicales reproducibles** sobre **siete paletas por acto**, mediante Web Audio API nativa. Las variaciones de cada capítulo utilizan una afinación, voicing, frase, tempo y timbre determinados a partir de su identificador. Al navegar, los paisajes se superponen y se atenúan gradualmente para evitar cortes bruscos. No se cargan pistas musicales ni se requieren dependencias JavaScript nuevas.

- **▶ Escuchar voz**: botón destacado fuera del panel de configuración; lee la historia actual o la escena abierta del manifiesto, según el contexto.
- **♫ Sonido**: panel con música ambiental, voz, velocidad y control de volúmenes.
- **Ambiente 100 %**: valor inicial del deslizador *dentro de una mezcla moderada y comprimida*, no el volumen máximo del dispositivo.
- **Inicio ambiental · 5.5**: el paisaje queda activado por defecto (deslizador en 100 % de una mezcla moderada). Si el navegador bloquea el autoplay, aparece «Sonido listo» y comienza con la primera interacción; «Apagar paisaje» lo desactiva para el resto de la visita.
- **Voz**: sigue utilizando SpeechSynthesis del navegador; la naturalidad depende de las voces instaladas. No sustituye una grabación profesional.
- **Composición**: fuente original con osciladores, ruido filtrado, motivos generativos, paneo, retardo, compresión y programación anticipada de eventos.

### Referencias técnicas consultadas

- [Tone.js / Tone.Transport](https://github.com/Tonejs/Tone.js) — reloj de audio y programación musical anticipada; **no se incorporó la biblioteca**.
- [Aether, paisaje sonoro generativo](https://github.com/thomasehardt/aether) — referencia conceptual de texturas y capas; **sin copiar su código**.
- [MDN Web Audio Examples](https://github.com/mdn/webaudio-examples) — síntesis, filtros y temporización.

### Pruebas

Se verificaron sintaxis JavaScript, controles en escritorio y móvil, inicio/detención de música, cambio de capítulo con dos capas activas durante la transición y ausencia de errores JavaScript en el navegador de pruebas. Las capturas locales usan teselas simuladas para aislar la interfaz. La **calidad acústica subjetiva** y los dispositivos móviles reales necesitan revisión auditiva posterior.


## Inicio de ambiente · 5.5

Al entrar se intenta activar la música. Por las políticas de reproducción automática de los navegadores, no se puede garantizar sonido audible antes de la primera interacción. Si Web Audio queda suspendido, la primera acción en la página inicia el ambiente sin exigir abrir ajustes; el estado visible distingue **Sonido listo**, **Sonido ON** y **Sonido OFF**. Apagarlo manualmente evita que vuelva a encenderse por otra interacción. El fondo se pausa cuando la pestaña está oculta.
