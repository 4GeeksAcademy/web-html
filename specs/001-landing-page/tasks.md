# Tareas: landing page de Milo Vértice

## Contenido HTML

- [X] Redactar datos ficticios coherentes para la identidad, biografía, retrato, trayectoria, presentaciones y contacto.
- [X] Añadir los datos de muestra directamente al contenido de `index.html`, sin crear un JSON de datos.
- [X] Identificar visiblemente la página como una demostración ficticia.
- [X] Usar un correo de ejemplo bajo `example.com` y no incluir datos personales reales de terceros.

## Estructura de la página

- [X] Crear `index.html` con idioma, metadatos de demostración y estructura HTML semántica.
- [X] Añadir navegación por anclas a «Sobre mí», «Trayectoria» y «Próximas presentaciones».
- [X] Añadir las secciones hero, «Sobre mí» con biografía y retrato, «Trayectoria», «Próximas presentaciones» y pie de contacto.
- [X] Añadir una directiva para impedir la indexación como perfil real mientras el contenido sea ficticio.
- [X] Añadir JSON-LD Schema.org `Person` dentro de `index.html`, describiendo el perfil como ficticio y manteniéndolo coherente con el contenido visible.
- [X] Añadir un enlace `mailto:` con el correo reservado de ejemplo.

## Presentación y accesibilidad

- [X] Crear `static/styles.css` separado con estilos mobile-first.
- [X] Distribuir el contenido con Flexbox y añadir media queries para móvil y escritorio.
- [X] Dar a las secciones de contenido una altura aproximada a un viewport, permitiendo que crezcan sin recortar contenido.
- [X] Comprobar que navegación, textos, imágenes y eventos no provoquen desbordamiento horizontal.
- [X] Añadir texto alternativo útil al retrato y asegurar contraste suficiente, foco visible y navegación por teclado.
- [X] Revisar el idioma del documento y mantener un único encabezado principal con jerarquía coherente.

## SEO, GEO y publicación

- [X] Redactar título y descripción coherentes con el contenido mostrado.
- [X] Revisar que el contenido y los metadatos identifiquen claramente la página como demostración y no prometan posicionamiento.
- [X] Comprobar que el JSON-LD sea válido, use `Person` y coincida con el contenido ficticio visible.
- [X] Revisar que el contenido textual describa la obra y trayectoria sin depender solo de imágenes.

## Verificación final

- [X] Iniciar `python3 server.py` y revisar la página en `http://localhost:3000`.
- [X] Comprobar los enlaces de navegación, el contacto, la adaptación móvil/escritorio y que no haya contenido recortado.
- [X] Recorrer la página con teclado y revisar foco, contraste, nombres de enlaces y texto alternativo.
- [X] Validar metadatos y JSON-LD; confirmar que el mock no se presente ni se indexe como perfil real.
- [X] Confirmar que no se haya añadido un archivo JSON de datos ni JavaScript ejecutable.
