# Recomendación de bajos eléctricos

### Descripción
Este es un sitio con recomendaciones de bajos eléctricos de toda índole para diferentes necesidades y gustos, pensado para todo tipo de gente interesada en el instrumento.

### ¿Qué quieres constuir?

- ¿Qué voy a recomendar?
Recomendaré diferentes modelos de bajos eléctricos de todos los tiempos. Todos los enlistados son emblemáticos por sus virtudes y cualidades.

- ¿A quién va dirigida la página?
El público objetivo son tanto personas curiosas y principiantes del bajo eléctrico como gente con más experiencia que desea conocer nuevos modelos icónicos.

- ¿Qué información tendrá cada recomendación?
Una imagen de referencia del modelo, una breve descripción de sus mejores características y un botón que enlaza a un video de YouTube con una demostración de sonido.

- ¿Qué quiero que suceda cuando el usuario interactúe con mi página?
Primero que encuentre la navbar y el encabezado de la página, conforme el usuario se desplaza hacia abajo por la página, tendrá la navbar siempre presente y las diferentes categorías de la página se desplegarán lateralmente para una navegación más cómoda.
Adicionalmente, en la consola se muestra una recomendación para el público en general.

### Tecnologías

- HTML
- CSS
- Bootstrap
- JavaScript
- Git
- GitHub
- DeepSeek

### Proceso con IA

| ¿Qué necesitabamos | Prompt | ¿Qué respondió? | ¿Qué utilicé? | ¿Qué aprendí? |
| -------- | -------- | -------- | -------- | --------| 
| Planificación y diseño de la página con HTML | Estoy trabajando en el diseño de una pequeña pagina web que se trate de recomendaciones de bajo eléctrico, modelos los cuales ya tengo enlistados. Pero vamos por partes, primero me gustaría que revises la distribución de mi enlistado en el sentido de diseño web y des sugerencias de uso de elementos de bootstrap, pero hay limitantes. Si aparecen conceptos como: function, for, while, addEventListener, querySelector, map, filter NO deben utilizarlos. Reescribe la solución utilizando únicamente variables, tipos de datos, console.log(), HTML, CSS y Bootstrap. No utilices funciones, ciclos ni manipulación del DOM. Por el momento mi styles.css está vacío y mi script.js tambien esta vacio | Propuesta de diseño mejorado: Se reestructura el HTML con Bootstrap incluyendo: contenedor principal (container) que centra el contenido y da márgenes adecuados; grid responsive (row + col-*) que en móviles muestra 1 columna, en tablets 2 columnas (col-md-6) y en desktop 3 columnas (col-lg-4); cards de Bootstrap para cada bajo con h-100 para igualar altura y shadow-sm para sombra sutil; mejor tipografía con display-4 para el título principal, lead para subtítulos, y text-primary y text-muted para colores; espaciado consistente con py-5 (padding vertical), g-4 (gap entre cards) y mb-5 (margen inferior). Se sugiere agregar transición suave en cards con transform y box-shadow al hacer hover, y personalizar el color de text-primary y la opacidad del separador hr. | Utilicé la idea general que me proporcionó y tomé los elementos de Bootstrap que me sugirió directo de la documentación oficial | Aprendí que existen las transiciones suaves para diferentes elementos si se pasa el mouse por encima de ellos, agregando las propiedades adecuadas en CSS |
| Incorporación de Navbar de Bootstrap | Incorporaré una navbar al inicio. No me des código, mi duda es si la seccion de navbar debe ir inmediatamente despues de abrir el body y antes de div class="container py-5" o si va dentro de del container py-5? | La navbar debe ir inmediatamente después de abrir el body y ANTES del div class="container py-5". Razones: Las navbars normalmente son de ancho completo (full-width) y no deben estar limitadas por el padding de un container. Bootstrap tiene clases específicas como container-fluid o simplemente sin container para que la navbar ocupe todo el ancho de la pantalla. La navbar suele tener su propio fondo (color sólido o degradado) que debe extenderse de borde a borde, mientras que el contenido principal tiene un fondo diferente o más sutil. Estética profesional: Es el estándar en la mayoría de sitios web que verás (ej: navbar oscura en la parte superior, contenido centrado debajo). | Utilicé la información dada para aplicar mi Navbar inmediatamente al iniciar el body | Aprendí que la navbar tiene prioridad de aparición en el body |
| Sugerencia de diseño con Bootstrap | Tengo pensado categorizar a todos los instrumentos de la siguiente manera: 1	Los Imprescindibles	Eléctricos de cuerpo sólido (P-Bass, J-Bass, StingRay) 2	Mejor Calidad-Precio	Eléctricos económicos (Ibanez SR) 3	Técnicas Avanzadas	Eléctricos de boutique (Sadowsky) 4	Sonido Vintage	Eléctricos clásicos (Höfner, Rickenbacker, Thunderbird) 5   Tecnología de Nicho	Innovadores y raros (Willcox, Whamola, Audiovox) 6	Acústicos y Tradicionales	Contrabajo, Tololoche, Bajo Electroacústico. Aún no me proporciones código, me gustaría una sugerencia de elemento de bootstrap para poder separarlos adecuadamente en esas categorías, que se note el orden. Me gustan más las cards separadas con títulos. Un título en letras medianas/grandes (pero no tanto como los titulos del header) y que las cards estén dentro de algún contendor con un borde delgado y sin background para que la imagen de fondo de la página sea visible | Elementos de Bootstrap que necesitas: 1. Para los títulos de categoría: Usa .h4 o .h5 (con h2 o h3 semántico). Acompañado de .fw-bold para darles peso visual. Puedes agregar un ícono o badge al lado para reforzar el número de categoría. 2. Para el contenedor de cada categoría: Usa .border para el borde delgado. .border-1 o .border-2 para controlar el grosor. .rounded para esquinas suaves. Sin background (no uses .bg-*). .p-3 o .p-4 para padding interno. .mb-4 para separación entre categorías. 3. Para las cards de los bajos dentro de cada categoría: Usa .card con .bg-transparent para que sean transparentes. .border-0 para eliminar el borde de las cards individuales (así solo el contenedor padre tiene borde). O puedes mantener borde en las cards pero muy sutil (.border-light). 4. Para la imagen de fondo: Asegúrate de que el body o un contenedor principal tenga la imagen de fondo. Usa .bg-transparent en todos los elementos que quieras que muestren el fondo. | Utilicé la idea general para los títulos de secciones y cards, pero no apliqué la transparencia a cada una de las cards por gusto personal. | Aprendí una nueva manera de agrupar cards |
| Reescalamiento de imágenes con CSS | Ya apliqué los cambios de las secciones de categorías y de poner imagenes en las cards y por ahi puse un solo boton para ver como quedaría, pero tengo un problema: Muchas cards utilizan absolutamente toda la altura del contenedor en el que están dejando mucho espacio muerto que se ve mal, intenté corrigiendo las alturas de las imagenes de la categoria de imprescindibles pero no ayudó mucho, tienes alguna solución para esto? | El problema que tienes es que h-100 en las cards las estira para igualar la altura del contenedor, pero las imágenes tienen diferentes tamaños, creando espacios vacíos inconsistentes. Soluciones (sin código): Opción 1: Altura fija para las imágenes (más recomendada). Asigna una altura fija a todas las imágenes dentro de las cards (ej: 200px o 250px). Usa object-fit: cover para que la imagen se recorte manteniendo proporción. Esto hace que todas las imágenes sean exactamente iguales y las cards queden uniformes. Opción 2: Eliminar h-100 de las cards. Quita la clase h-100 de cada card. Las cards solo ocuparán el espacio que necesiten según su contenido. Esto puede hacer que las cards de la misma fila tengan alturas diferentes. Opción 3: Combinación de ambas. Mantén h-100 en las cards para igualar alturas. Pon altura fija a las imágenes (opción 1). Agrega un padding consistente en el card-body. Opción 4: Flexbox en el contenedor. Usa d-flex flex-column en la card. La imagen ocupa un espacio fijo. El card-body se estira para llenar el espacio restante con flex-grow-1. Mi recomendación: Opción 1 es la más limpia y profesional. Todas las imágenes con la misma altura (object-fit: cover) y las cards con h-100 se verán perfectamente alineadas sin espacios muertos extraños. Lo que NO funciona: height: 50% en las imágenes (como tienes ahora) porque el porcentaje depende del contenedor padre, y cada card tiene altura diferente por el contenido variable. ¿Qué opción prefieres que desarrolle con código? | Utilicé la opción 1 que incorpora object-fit y reescalé las imagenes de cada sección a conveniencia en vez de lo sugerido por la IA | Aprendí una nueva manera de estandarizar el tamaño de las imágenes. |

### Código generado vs código propio

- ¿Qué generó la IA?
La IA me ayudó generando código principalmente estructural a manera de marcador de posición para que yo lo modificara y personalizara posteriormente. Así pues, también generó explicaciones y aclaraciones a preguntas que tenía acerca de diferentes elementos y clases de Bootstrap y el manejo de ciertos atributos en CSS, auxiliando en mi proceso de aprendizaje.
Adicionalmente también me ayudó en la redacción de ciertas oraciones.

- ¿Qué modificamos nosotros?
El código estructural proporcionado por la IA para personalizarlo, y de manera similar el código de la documentación oficial de Bootstrap.

### Aprendizaje

- ¿Qué concepto nuevo comprendí gracias a la IA?
Aprendí dos conceptos nuevos de CSS. El primero es la creación de un efecto de elevación suave para una card, haciendo uso de las propiedades transform, box-shadow y transition para dar un efecto de que está volando y proyecta una sombra.

El segundo es la propiedad llamada object-fit con valor cover, que controla como el contenido de un elemento se redimensiona para ajustarse a su contenedor, permitiendo evitar distorsiones o recortes no deseados. Este nuevo concepto fue clave para que las imágenes de los bajos se vieran del mismo tamaño y las cards se vieran visualmente armónicas.

### Reflexión

- ¿Hubo algún momento en que la IA generó código que no comprendía?
Sí, tanto de no saber que hacían ciertas etiquetas de HTML o propiedades de CSS, como código que costaba trabajo entender por mala separación o pocos comentarios.

- ¿Qué hicimos?
Investigar en sitios de documentación oficial, foros o pedirle que genere de nuevo la información de manera más clara y explicativa por medio de un prompt mucho más detallado.