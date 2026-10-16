# AGENTS.md

## Objetivo

Crear y mantener una web personal para un artista: una experiencia visual, clara y accesible que presente su obra, trayectoria y formas de contacto. Antes de modificar archivos, revisa estas pautas y conserva cualquier contenido existente que no forme parte del cambio solicitado.

## Tecnologías y estructura

- Usa HTML5 semántico y CSS escrito en archivos separados, enlazados desde el documento HTML.
- No uses frameworks, bibliotecas de interfaz, generadores CSS ni JavaScript. Resuelve la presentación con HTML y CSS nativos.
- Emplea Flexbox para los diseños y la distribución de elementos. Evita depender de posicionamiento absoluto para la estructura principal.
- Mantén el marcado sencillo, válido y organizado por responsabilidades. Usa nombres de clases descriptivos y evita estilos en línea.
- Escribe el contenido ficticio del artista directamente en el HTML. No crees un archivo JSON de datos, API ni sistema de plantillas para almacenar o generar ese contenido.
- El bloque JSON-LD de Schema.org es una excepción permitida: debe ir dentro del HTML como `<script type="application/ld+json">` y no debe contener JavaScript ejecutable.

## Datos del artista

- Inventa los datos necesarios como contenido de demostración directamente en el HTML; no afirmes que son hechos reales sobre Milo Vértice.
- Identifica visiblemente la página como una demostración con contenido ficticio.
- No uses datos personales reales de terceros. Para el correo de ejemplo, usa un dominio reservado como `example.com`.
- Mantén el contenido ficticio coherente entre secciones, metadatos y JSON-LD; indica en la descripción estructurada que se trata de un ejemplo ficticio y evita que los buscadores indexen la página como un perfil real.

## Diseño adaptable

- Diseña primero para pantallas pequeñas y amplía el diseño con media queries cuando haga falta.
- Usa dimensiones flexibles, unidades relativas y límites razonables de ancho para que el contenido se adapte sin desbordarse.
- Asegura que navegación, galerías, textos y controles sigan siendo utilizables con distintos tamaños de pantalla y orientación.
- No transmitas información únicamente mediante color, tamaño, posición o efectos visuales.

## Accesibilidad

- Define el idioma del documento y una jerarquía de encabezados coherente; incluye un único encabezado principal por página.
- Usa elementos HTML según su propósito, enlaces para navegar y botones solo para acciones.
- Proporciona texto alternativo útil para imágenes informativas; usa texto alternativo vacío en imágenes puramente decorativas.
- Mantén contraste suficiente, foco de teclado visible y orden de lectura y tabulación lógico.
- Asegura que los enlaces tengan nombres comprensibles fuera de contexto y que los controles tengan etiquetas visibles o accesibles.
- No uses elementos interactivos sin una alternativa operable con teclado.

## SEO y GEO

- Escribe títulos y descripciones pertinentes que identifiquen la página como demostración mientras incluya contenido ficticio.
- Usa URL, títulos, encabezados, enlaces y texto alternativo descriptivos; organiza las páginas con enlaces internos claros.
- Presenta de forma visible y consistente el nombre del artista, su disciplina, obra, trayectoria y ubicación o datos de contacto cuando estén disponibles.
- Publica información original, precisa y bien estructurada. Explica obras y proyectos en texto legible, no solo dentro de imágenes o elementos gráficos.
- Usa datos estructurados estándar únicamente cuando describan fielmente el contenido; mantenlos consistentes con la información visible.
- Facilita que buscadores y motores generativos interpreten las páginas mediante contenido específico, contexto claro, entidades nombradas de manera consistente y HTML semántico. No prometas posicionamiento ni inventes datos con el fin de mejorar la visibilidad.

## Alcance de cambios

- No añadas dependencias, JavaScript ejecutable, rastreadores ni servicios externos sin una solicitud explícita.
- Conserva el carácter ficticio del contenido de demostración; no lo presentes como información real.
- Mantén los cambios acotados a la petición y no generes páginas o recursos que no se hayan solicitado.

## Criterios de aceptación

- La identidad, biografía, trayectoria, presentaciones y contacto ficticios están escritos directamente en el HTML; no se crea un archivo JSON de datos.
- La página identifica visiblemente el contenido como ficticio y no usa datos personales reales de terceros.
- El bloque JSON-LD usa Schema.org `Person`, es válido y coincide con el contenido visible; identifica el perfil como ficticio.
- Los metadatos evitan presentar el mock como un perfil real y la página indica a los buscadores que no la indexen como tal.
