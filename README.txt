DYSONREPAIR SERVICIO TÉCNICO DYSON BILBAO
=========================================

Web de una sola página (HTML/CSS/JS estático + función serverless en Vercel)
para DysonRepair, servicio técnico y reparación de equipos Dyson con recogida
y entrega en Bilbao y área metropolitana.

Dominio: https://soportetecnico.com.es/
Marca: DysonRepair Servicio Técnico Dyson Bilbao
Ficha de Google: https://maps.app.goo.gl/NxVLpcdji8otnxqd8
Mapa: iframe de Google Maps de la ficha "DysonRepair Servicio Técnico",
insertado tal cual en la sección de contacto (ancho 100% vía CSS).

DATOS DE CONTACTO
- WhatsApp: +34 649 97 01 28.
- Teléfono: +34 910 05 48 17.
- Recogida a domicilio: https://sis.redsys.es/tiendaWeb/item/NDk4OzI=
  (botón "Solicita tu recogida ahora" del hero, siempre en negro).
- Horario: lunes a viernes de 09:30 a 18:00.
- Política de privacidad: https://kelatos.com/privacy-policy/.

DIRECCIÓN: no se muestra dirección postal. La web indica "Bilbao y área
metropolitana" y servicio de recogida y entrega; el taller está en Madrid.
Si se confirma una dirección en Bilbao, añadirla al hero, footer y JSON-LD.

ESTRUCTURA
- index.html: toda la página (hero, ventajas, reparación rápida, confianza,
  servicios, por qué elegirnos, cómo trabajamos, contacto + mapa, FAQ, texto
  SEO, footer, cookies y JSON-LD).
- style.css: base de la plantilla.
- mobile-navigation.css, social-footer.css, cal-booking.css: ajustes compartidos.
- dysonrepair.css: identidad visual de la marca (una sola capa, sin
  sobrescrituras en cascada).
- dysonrepair-header-hero.css: cabecera grafito con logotipo blanco.
- dysonrepair.js: menú móvil (se cierra al pulsar un enlace), formulario y
  preferencias de cookies (clave localStorage "dysonrepair_cookie_preference").
- dysonrepair-n8n-chat.js / .css: chatbot n8n con webhook compartido del grupo
  y botón de respaldo.
- api/contacto.js: envío del formulario por SMTP (variables SMTP_HOST,
  SMTP_PORT, SMTP_SECURE, SMTP_USER, SMTP_PASS y CONTACT_EMAIL en Vercel).
- img/: isotipo, patrón e ilustraciones SVG de la marca.
- robots.txt y sitemap.xml apuntan a https://soportetecnico.com.es/.

PALETA: violeta índigo y grafito, con acento lavanda.
- Marca #5B3FC4 · oscuro #4530A0 · muy oscuro #2E2170
- Lavanda #B7A8F4 · fondo suave #F3F0FD
- Grafito (cabecera, footer, cookies) #16141F
Excepciones: WhatsApp conserva su verde y YouTube su rojo corporativo.
