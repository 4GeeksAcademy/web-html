# Especificación: landing page de Milo Vértice

## Objetivo

Presentar la obra y trayectoria de Milo Vértice en una landing page personal, accesible y adaptable, que permita conocer sus próximas presentaciones y contactarlo.

## Alcance

Esta especificación define estructura, contenido y criterios de aceptación. No incluye la implementación de la página.

## Requisitos

### Estructura y contenido

- Incluir un encabezado con navegación hacia «Sobre mí», «Trayectoria» y «Próximas presentaciones».
- Incluir una sección hero con bienvenida y presentación de Milo Vértice y su actividad artística.
- Incluir una sección «Sobre mí» con biografía y fotografía.
- Incluir una sección «Trayectoria» que presente su recorrido artístico.
- Incluir una sección «Próximas presentaciones» con eventos de muestra.
- Incluir un pie de página con el correo de contacto.
- Inventar los datos de muestra al redactar el contenido de `index.html`; no crear un archivo JSON para almacenarlos.
- Identificar visiblemente la página y sus datos como una demostración ficticia. No presentar esa información como hechos reales sobre Milo Vértice ni usar datos personales reales de terceros.
- Usar un correo de ejemplo bajo un dominio reservado, como `manuel@example.com`.

### Diseño y tecnología

- Usar HTML semántico y CSS en un archivo separado.
- Usar Flexbox para la distribución de elementos.
- No usar frameworks, bibliotecas de interfaz, JavaScript ejecutable ni dependencias nuevas. Se permite JSON-LD dentro de `<script type="application/ld+json">` exclusivamente como datos estructurados.
- Escribir el contenido directamente en el HTML; no añadir archivo JSON de datos ni renderizado dinámico desde el servidor.
- Diseñar de forma adaptable para móvil y escritorio, sin desbordamiento horizontal.
- Cada sección de contenido tendrá una altura visual aproximada a un viewport. El contenido podrá extender la sección si es necesario; no debe recortarse para cumplir una altura fija.

### Accesibilidad

- Declarar el idioma de la página y mantener una jerarquía coherente de encabezados, con un único encabezado principal.
- Usar elementos HTML de acuerdo con su propósito y enlaces descriptivos para navegación y acciones.
- Proporcionar texto alternativo útil para la fotografía; usar alternativa vacía únicamente si la imagen es decorativa.
- Mantener contraste suficiente, foco de teclado visible, orden de lectura lógico y navegación operable por teclado.
- Asegurar que enlaces e información de contacto tengan nombres comprensibles fuera de contexto.

### SEO, GEO y datos estructurados

- Usar un título descriptivo y una meta descripción que identifiquen el contenido como demostración ficticia.
- Presentar de forma clara y consistente el nombre de Milo Vértice, su actividad, trayectoria y presentaciones.
- Escribir información original y específica en texto legible; no depender únicamente de imágenes para explicar obras o eventos.
- Incorporar datos estructurados JSON-LD con Schema.org `Person`, coherentes con los datos ficticios visibles e indicando en la descripción que se trata de un ejemplo.
- Evitar que la página se indexe como perfil real mientras use datos ficticios.
- Omitir propiedades que no se incluyan en el contenido de muestra; no inventar perfiles sociales o URL de terceros.

## Criterios de aceptación

1. El encabezado ofrece enlaces a «Sobre mí», «Trayectoria» y «Próximas presentaciones», y cada enlace lleva a su sección correspondiente.
2. La página presenta las secciones hero, «Sobre mí» con biografía y fotografía, «Trayectoria», «Próximas presentaciones» y un pie con correo de contacto.
3. El correo de muestra permite iniciar un mensaje y usa un dominio reservado para ejemplos.
4. En móvil y escritorio, la navegación, el texto, la fotografía y las presentaciones se pueden utilizar sin desbordamiento horizontal ni contenido recortado; las secciones mantienen una escala cercana a un viewport y pueden crecer según su contenido.
5. La página puede recorrerse con teclado, el foco es visible y los enlaces tienen nombres descriptivos.
6. La fotografía informativa tiene texto alternativo adecuado y el documento usa idioma y estructura de encabezados coherentes.
7. El título y la descripción identifican la página como demostración; el nombre y la actividad ficticia aparecen claramente en el contenido visible.
8. El JSON-LD es válido, usa el tipo `Person`, coincide con el contenido ficticio visible y no representa el perfil como real; la página indica a los buscadores que no la indexen.
9. No existe un JSON de datos ni una ruta de servidor para cargar contenido: los textos de muestra se editan directamente en `index.html`.
