# HTML semántico desde su inicio.😎
Desde su inicio el HTML añade significado semántico a el código que comprende un sitio web.
Con etiquetas como `<h1>` , `<p>`, `<img>` , etc… el desarrollador puede designar un título,
añadir encabezados y párrafos e insertar imágenes para así dar forma al documento.
En el HTML cada elemento tiene su propio modelo de contenido,
el cual describe el tipo de contenido que este debe contener.

### Los modelos de contenido se dividen en las siguientes categorías 📚

    Elementos para seccionar
    Elementos de metadata
    Interactivos
    Fraseo, de títulos
    Elementos para incrustar

Algunos de estos elementos pueden pertenecer a dos o más categorías por su función y definición.

Al dividir el contenido en secciones por temas o funcionalidad, logramos visualizar el esquema del documento.

Antes del lanzamiento del HTML5 la mejor manera para describir el esquema o índice del contenido, era utilizando los elementos de títulos que van del H1 al H6.
En verdad hoy siguen siendo muy importantes para identificar y generar secciones dentro del contenido.

Aplicar estas etiquetas de títulos correctamente es fundamental para optimizar el contenido para los buscadores y uno de los elementos más importantes en el checklist del On-page SEO.

Los autores pueden otorgar diferente peso y relevancia a las secciones del contenido utilizando el número correspondiente en el título al inicio de dicha sección.

> Utiliza el `<h1>` para el título del artículo o página y `<h2>` a `<h6>` para dividir el contenido interno de acuerdo al esquema del documento.
```
<h1> titulo de la pagina</h1>
<h2> sección 1 </h2>
<h3> sección 1.a </h3>
<h3> sección 1.b </h3>
<h2> sección 2 </h2>
<h3> sección 1.a </h3>
<h4> titulo interno </h4>
```

Otro elemento esencial es la etiqueta `<head>` que funciona para designar el espacio dentro del documento donde se alberga los elementos que configuran y preparan el documento para ser visualizados correctamente.
```
<head>
  <meta http-equiv="Content-Type" content="text/html; charset=UTF-8" />
  <title>Titulo de documento</title>
  <link rel="stylesheet" type="text/css" href="estilos.css" />
  <link rel="shortcut icon" href="/favicon.ico" />
</head>
```

# Estructura semántica utilizando HTML 5 🤯
Con el lanzamiento del HTML5 surgieron nuevos elementos enfocados en aumentar el poder semántico y estructural del lenguaje.

> `<article>`, `<aside>`, `<nav>`, `<section>`, `<footer>`, `<header>` y `<main>`

Nuevos elementos como `<main>` o `<nav>` que describen secciones de una página de Internet y nuevos elementos como `<figure>` o `<time>` que describen el tipo de contenido que contienen.

Entender el significado semántico de estos nuevos elementos permite estructurar con detalle el esquema del documento. Lo que ayuda al lector a visualizar y entender mejor el contenido.

Además permite a personas con discapacidad, navegar y consumir tu contenido con mayor facilidad. Además que ayuda a los buscadores como Google rastrear y entender mejor el contenido de tu sitio de internet.

Con el surgimiento de los asistentes digitales y la búsqueda por voz, hoy en día la semántica en el código de tu página es fundamental.Consejo: Como buena práctica y para dar compatibilidad con navegadores antiguos como internet explorer 9 o anteriores, utiliza el archivo shim o shiv html.js.

## Nuevos elementos estructurales 🤩
`<header>` – Este elemento se utiliza para agrupar las piezas de introducción del contenido.

Los elementos que encontramos dentro de la cabecera o introducción de una página de Internet generalmente son: Elementos de identidad o branding como el logotipo, nombre de la organización, slogan y elementos de navegación del sitio.

`<nav>` – Este elemento es para agrupar elementos de navegación del sitio, muy importante utilizarlo en el menú principal.
```
<section>
  <header>
    <h1>Título de sección - noticia </h1>
    <nav><a href=”#”>menu1</a><a href=”#”>menu2</a><a href=”#”>menu3</a></nav>
  </header>
</section>
```
`<main>` – Utilizado para indicar el contenido más importante de la página, este nuevo elemento resulta muy importante para los lectores de pantalla y dispositivos de asistencia a discapacitados. Lo importante es utilizarlo para agrupar justo el contenido deseado y no agrupar aquí elementos que estén fuera del tema principal de la página como, anuncios y las barras laterales.

`<article>` – La definición de este elemento indica que se debe utilizar para agrupar contenido que por sí solo tiene razón de ser y significado. Un buen ejemplo es utilizarlo en un blog para agrupar cada uno de los artículos o publicaciones.

    Ejemplo:
```
<article>
  <h2>título del artículo 1</h2>
  <p>contenido del artículo 1</p>
</article>
<article>
  <h2>título del artículo 2</h2>
  <p>contenido del artículo 2</p>
</article>
```
`<section>` – Este elemento tiene un valor semántico más general y es utilizada para agrupar secciones o subsecciones de contenido. El significado de que es una sección se vuelve muy personal y subjetiva. Lo importante es tener consistencia en tu propia definición y uso de la elemento.

`<aside>` Dentro de este elemento va el contenido que está fuera del tema principal del tema principal de la página.

Por ejemplo, las barras laterales con contenido como anuncios o los artículos más populares.

`<footer>` El pie de página o footer generalmente contiene los avisos legales, información de derechos de autor e información de contacto. Por lo general también es la última sección de la página.
```
<main>
  <section>
    <article>
      <h2>título del artículo 1</h2>
      <p>contenido del artículo 1</p>
    </article>
    <article>
      <h2>título del artículo 2</h2>
      <p>contenido del artículo 2</p>
    </article>
  </section>
  <aside>
    <p>barra lateral</p>
  </aside>
</main>
<footer>
  <p> aviso de privacidad </p>
</footer>
```
## Nuevos elementos de contenido 🤗
`<figure>` – Este elemento describe contenido de flujo con significado propio, muy utilizado para describir imágenes, video, ilustraciones, diagramas, fragmentos de código, etc.

Por lo general este elemento viene acompañado de una leyenda con la descripción o información relacionada del elemento.

`<figcaption>` – Es el elemento que contiene la leyenda o información relevante acerca del elemento `<figure>` antecesor.
```
<figure>
  <img src="imagen.jpg" alt="descripción" width="304" height="228">
  <figcaption>Leyenda de imágen</figcaption>
</figure>
```
`<video>` – Otra etiqueta nueva en HTML5 indica y otorga funcionalidad para insertar un video con controles para su playback,

Hay 3 formatos de video están soportados por la etiqueta `<video>`: MP4, WebM, y Ogg.

`<audio>` – Indica que el contenido es uno o más archivos de audio, inserta los controles e interfaz para reproducir los archivos.

Los formatos de archivos soportados por la etiqueta `<audio>`: MP3, WAV y Ogg.

`<canvas>` – Este elemento se utiliza para contener gráficos generados por código, Javascript por lo general.

`<data>` – Esta etiqueta es utilizada para entregar un valor asociado a el contenido dentro de la etiqueta para ser leído por alguna aplicación o sistema. Por ejemplo el valor asociado por producto.
```
<ul>
  <li><data value="21053">Tomates</data></li>
  <li><data value="21054">Jitomates</data></li>
  <li><data value="21055">Uvas</data></li>
</ul>
```

`<mark>` – Contiene información marcada o seleccionada, el resultado debe ser texto marcado con un fondo de algún color.

`<time>` – Contiene información de fechas, horarios o tiempo. Al formatear estas fechas, horarios o tiempo con estándares legibles por máquinas, esta información puede servir para guardar información en calendarios y agendar notificaciones.

`<details>` – Este elemento representa detalles adicionales que el usuario puede ver y esconder a su gusto.

`<summary>` – Es el elemento que conforman la cabecera siempre visible del elemento `<details>` antecesor.

`<progress>` – Contiene información acerca del progreso de una actividad o acción.

> ### Para más información visita la página **http://www.manualweb.net/html5/semantica-html5/**