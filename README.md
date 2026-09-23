# Nordic Gaming Browser

Sitio público: https://nordicbrowser.com/

## Contenido

- `index.html`: producto, funciones, plan mensual, entrega y activación, reembolsos, contacto y privacidad.
- `styles.css` y `redesign.css`: diseño adaptable y navegación accesible.
- `assets/`: logo y capturas reales de Nordic.
- Sitio estático sin dependencias ni compilación.

## Datos utilizados (23 de septiembre de 2026)

- Soporte: `noordicdev@gmail.com`, tomado del comando `access.support` del navegador y su documentación.
- Acceso ligado a Discord: documentación de integración y cliente Commercial.
- Mensual de $2.999 CLP, actualizado por indicación del titular. Se mantienen las condiciones publicadas de un equipo, una sesión y sin renovación automática.
- Hay una diferencia documental entre mes calendario y 30 días. El sitio describe un periodo mensual y exige confirmar fechas exactas antes del pago; conviene unificar esta definición en el producto.
- Por indicación del titular, el sitio informa pagos a través de Webpay e inicio de sesión con Discord y compra de suscripción dentro de Nordic Gaming Browser. El sitio no implementa login ni checkout.
- No se publica una versión o enlace de instalador no verificado. El enlace oficial se entrega por soporte.

## Condiciones comerciales iniciales

Por autorización del titular para definir condiciones sencillas donde faltaban:
- El instalador se obtiene por Discord; el usuario inicia sesión y compra desde Nordic. Se reemplazó la descripción anterior de contratación manual por este flujo, indicado por el titular.
- Devolución íntegra solicitada dentro de 10 días corridos, incluso con acceso activado.
- Casos de no entrega, cobros duplicados o problemas no solucionados se atienden también después.
- Respuesta a reembolsos: hasta 2 días hábiles. Inicio de devolución: hasta 5 días hábiles tras aprobación; el abono depende del proveedor.
- No se limitan los derechos legales del cliente.

Estos plazos son decisiones iniciales para revisar con el titular; no se extrajeron como políticas preexistentes del código. Mantener condiciones publicadas coherentes con la atención real. Completar identidad comercial/tributaria y documentación de contratación antes de habilitar cobros automatizados.

## Formulario y activación pendiente

El formulario HTML hace POST por HTTPS a FormSubmit, con CAPTCHA del proveedor, campos obligatorios, límites de longitud, correo de respuesta y consentimiento. No contiene secretos y no utiliza `mailto:` como mecanismo de envío. El correo y Discord también están disponibles como canales alternativos.

**La recepción extremo a extremo queda pendiente hasta activar el formulario en `noordicdev@gmail.com`.** No afirmar que se recibe correo sin completar estos pasos:

1. Enviar una consulta de prueba desde la web publicada.
2. Abrir la casilla de soporte y confirmar el correo de activación de FormSubmit (revisar spam).
3. Repetir el envío y verificar la recepción y que Responder apunta al correo del remitente.
4. Si FormSubmit entrega un identificador opaco, se puede sustituir el correo en el `action` manteniendo visible el contacto público.

La validación del HTML y el contrato POST se probaron interceptando la solicitud localmente: esas pruebas no envían correo ni demuestran entrega.
Documentación: https://formsubmit.co/documentation y https://formsubmit.co/help.

## Verificación y mantenimiento

- Revisar 320, 390, 768 y 1440 px, imágenes, anclas, foco y validación del formulario.
- Comprobar que HTTP redirige a HTTPS y que la publicación responde 200.
- No publicar módulos propietarios, datos de usuarios ni funciones exclusivas de Owner.
- El HTTPS lo gestiona el alojamiento; un texto o badge en HTML no lo activa.

## Cloudflare Pages

Configuración: rama `main`, framework `None`, comando `exit 0`, salida `.`.
`canonical`, `og:url` y el campo `_url` del formulario apuntan a `https://nordicbrowser.com/`. `.assetsignore` incluye las hojas de estilo y todas las imágenes públicas utilizadas.

## Diseño y capturas

El inicio sigue la referencia suministrada por el titular: marca Nordic Gaming Browser, fondo oscuro, azul eléctrico, emblema original y CTA a Discord. Se conserva el lema solicitado: “The first optimized gaming browser. Built for performance, built to win.”

Las capturas de juegos, rendimiento, resolución y niveles fueron suministradas por el titular para su publicación. El panel de niveles se presenta como ejemplo; los datos visibles no representan la cuenta del visitante. Se conservan las funciones de HaxBall, contacto, reembolsos y privacidad. No se prometen mejoras cuantificadas de FPS ni reducción del ping.
