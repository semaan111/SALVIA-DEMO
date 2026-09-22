# Luma · Corporación Savia

Front completo y responsive. El personaje de Luma es el botón para iniciar la conversación por voz con el agente de ElevenLabs configurado.

## Archivos

- `index.html`: página completa con HTML, CSS, JavaScript e imagen de Luma integrada. No requiere instalar paquetes ni compilar.
- `luma.webp`: copia del personaje para futuras ediciones. El HTML ya contiene la imagen y no depende de este archivo.
- `.nojekyll`: permite servir el sitio estático directamente.

## Subir a GitHub y publicar

1. Descomprime este ZIP.
2. Crea un repositorio en GitHub o abre el repositorio donde publicarás la página.
3. Sube el contenido descomprimido a la raíz del repositorio y guarda los cambios. `index.html` debe quedar en la raíz, no dentro de una carpeta adicional. No subas únicamente el ZIP.
4. En **Settings → Pages → Build and deployment**, selecciona **Deploy from a branch**.
5. Selecciona la rama **main** (o la rama que estés usando), la carpeta **/(root)** y pulsa **Save**.
6. Cuando GitHub muestre el enlace publicado, ábrelo, toca a Luma y autoriza el micrófono.

Guía oficial: https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site

## Conversación

La imagen activa el mismo control de inicio del widget de ElevenLabs. Se conservan las condiciones de uso, permisos, errores y controles para finalizar la conversación. No se inicia ninguna llamada al cargar la página.

El agente configurado es `agent_1501kpvhvndjfddvgdkf9je5anrd`. Para conectar otro agente, cambia el atributo `agent-id` en `index.html`. La voz, instrucciones y conocimiento se administran en ElevenLabs.

Se necesita conexión a internet para cargar el widget, las fuentes y el servicio de voz. Prueba el micrófono en la URL HTTPS publicada. Si tu agente restringe los dominios autorizados, revisa que permita el dominio donde publiques esta página. El funcionamiento de las llamadas depende también de la disponibilidad y configuración del agente.

El adaptador visual usa la versión fijada `@elevenlabs/convai-widget-embed@0.18.2`. Si actualizas esa versión, revisa la integración del botón del personaje antes de publicar.

## Personalización

Los colores están en las variables CSS de `:root`. El texto principal, las etiquetas y la marca se editan en el mismo HTML. El mensaje sobre preguntas relacionadas con el crédito ya está incluido.

Marca ficticia · Experiencia de demostración.
