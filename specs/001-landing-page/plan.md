# Plan técnico aprobado: landing page de Milo Vértice

## Objetivo

Construir una landing page estática en el navegador, accesible y adaptable, con contenido ficticio de demostración redactado directamente en HTML. La página no utilizará JavaScript ejecutable ni frameworks de interfaz.

## Enfoque

Mantener una página estática en `index.html` y `styles.css`. Escribir el contenido de muestra directamente en el HTML, identificarlo visiblemente como ficticio y no presentarlo como información factual sobre Milo Vértice. No crear JSON de datos ni modificar `server.py`. El JSON-LD de Schema.org `Person` se incluye en el HTML como datos estructurados, no como JavaScript ejecutable, y debe describir explícitamente un ejemplo ficticio.

## Archivos previstos

- Crear `index.html` con contenido ficticio escrito directamente en sus secciones: identidad, biografía, trayectoria, eventos y contacto. Identificar la página como demostración y usar un correo bajo `example.com`.
- Añadir metadatos de demostración, directiva para evitar indexación como perfil real y JSON-LD `Person` coherente con el contenido visible, describiéndolo como ficticio.
- Crear `static/styles.css` separado, con diseño mobile-first, Flexbox y media queries.
- No crear `data/artist.json` ni `templates/index.html`; no modificar `server.py` ni añadir JavaScript ejecutable o dependencias.
- Mantener como referencias [AGENTS.md](../../AGENTS.md) y [spec.md](spec.md). No modificar otros archivos salvo que la implementación lo requiera y se acuerde.

## Pasos principales

1. Redactar el contenido ficticio directamente en `index.html`, manteniendo coherencia entre secciones y marcándolo como demostración.
2. Construir la estructura semántica de navegación, hero, «Sobre mí», «Trayectoria», «Próximas presentaciones» y contacto.
3. Implementar los estilos responsive: secciones de contenido con escala aproximada de un viewport, permitiendo que crezcan para no recortar texto; foco visible y contraste suficiente.
4. Añadir metadatos que identifiquen el mock, la directiva de no indexación y JSON-LD `Person` que describa explícitamente el ejemplo ficticio y coincida con el contenido visible.
5. Verificar accesibilidad, presentación responsive, metadatos y coherencia del JSON-LD.

## Criterios de aceptación y verificación

- Los datos ficticios se encuentran directamente en `index.html`; no existe un archivo JSON de datos ni código de carga dinámica.
- La página identifica el contenido como demostración y no lo presenta como real ni permite indexarlo como perfil real.
- La navegación lleva a las secciones correctas; el correo confirmado ofrece un enlace `mailto:`.
- La página se adapta a móvil y escritorio, no tiene desbordamiento horizontal y el contenido no se recorta aunque una sección supere la altura de un viewport.
- La navegación por teclado funciona, el foco es visible y la imagen informativa tiene texto alternativo útil.
- El título y la descripción identifican el contenido como demostración. El JSON-LD es válido, usa `Person` y coincide con los datos ficticios visibles.
- Iniciar `python3 server.py` y revisar la página en `http://localhost:3000` en tamaños móvil y escritorio.

## Consideración técnica

El contenido vive directamente en el HTML y se modifica allí. El bloque JSON-LD se conserva únicamente para cumplir el requisito de datos estructurados; no es un archivo de datos de artista ni código ejecutable.
