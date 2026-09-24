DYSONREPAIR — SERVICIO TÉCNICO DE ASPIRADORAS DYSON EN BILBAO
========================================================

Repositorio clonado originalmente de PowerFlow (Grupo N8nLabs, automatización
Power Automate). Se ha reconvertido por completo a DysonRepair, servicio técnico de
reparación de aspiradoras Dyson en Bilbao. Ningún texto de negocio ni enlace
del repositorio original se ha mantenido salvo la infraestructura compartida
de la familia (política de privacidad, patrón de checklist, chat n8n).

Dominio: https://soportetecnico.com.es/
Marca: DysonRepair Servicio Técnico de Aspiradoras Dyson en Bilbao
Ficha de Google: https://maps.app.goo.gl/NxVLpcdji8otnxqd88

DATOS DE CONTACTO
- WhatsApp: +34 649 97 01 28.
- Teléfono: +34 910 05 48 17 (el mismo número usado en otros repos de
  reparación Dyson de la familia, ej. DysonValladolid — confirmado que es
  correcto, no un error de copia).
- Recogida a domicilio: https://sis.redsys.es/tiendaWeb/item/NDk4OzI= (botón
  "Solicita tu recogida ahora" en el hero, dado explícitamente por el
  cliente).
- Reserva de citas: https://cal.com/kelatos/30min (patrón de la familia de
  reparaciones, no el cal.com de N8nLabs que usaba el repo original).
- Política de privacidad: https://kelatos.com/privacy-policy/.

DIRECCIÓN — PENDIENTE DE CONFIRMAR: no se ha mostrado una dirección postal
exacta (calle y número) porque no se facilitó y no se ha podido obtener de
forma fiable desde el enlace corto de Google Maps (pantalla de consentimiento
bloquea el scraping). Por geocodificación inversa de las coordenadas del
enlace, el negocio está en la zona de Calle del Emigrante / San Antón,
Bilbao (CP 30009), pero NO se ha inventado un número de portal. El
hero/footer/schema.org usan "Bilbao y área metropolitana" en su lugar. Si el
cliente da la dirección exacta, añadirla al hero-info, footer y JSON-LD.

RENOMBRADO DE ARCHIVOS (limpieza de contaminación "powerflow"):
powerflow.css→dysonrepair.css, powerflow.js→dysonrepair.js, powerflow-clients.css→
dysonrepair-clients.css, powerflow-header-hero.css→dysonrepair-header-hero.css,
powerflow-n8n-chat.css/.js→dysonrepair-n8n-chat.css/.js, powerflow-restoration.css/
.js→dysonrepair-restoration.css/.js, powerflow-social-colors.css→
dysonrepair-social-colors.css, img/powerflow-hero-pattern.svg→
img/dysonrepair-hero-pattern.svg. Referencias actualizadas en index.html y en la
carga dinámica de dysonrepair.js. Variables CSS --pf-*→--dp-*.

COLOR — cobre y grafito (nueva paleta, distinta de toda la familia):
Se ha sustituido la identidad azul/magenta de PowerFlow por una paleta cobre
(--green:#ad592a y derivados) + grafito oscuro + acento verde azulado
(--dp-magenta:#3ccec2), aplicada mediante rotación de tono (HSL) sobre TODOS
los colores de marca (hex y rgba) de dysonrepair.css, dysonrepair-header-hero.css,
dysonrepair-restoration.css, dysonrepair-n8n-chat.css y el patrón SVG del hero —
preservando saturación y luminosidad exactas, así que todos los contrastes,
degradados y estados hover quedan intactos, solo cambia el matiz. El verde de
WhatsApp y los colores reales de cada red social (Facebook, YouTube, etc. en
dysonrepair-social-colors.css) se han dejado sin tocar a propósito.

LOGOTIPO: se ha sustituido el logo de imagen (webp heredado de PowerFlow) por
un isotipo SVG propio (img/dysonrepair-isotype.svg, y su versión inline en
cabecera/footer): un motivo de ciclón/espiral (alusión a la tecnología
ciclónica de Dyson) en cobre y verde azulado sobre grafito, junto al
logotipo "DysonRepair" en texto. Pensado para poder reutilizar la misma forma con
otro color en futuras marcas de la familia.

CONTENIDO: reescrito por completo (hero, servicios, por qué elegirnos, cómo
funciona, texto SEO, footer, schema.org) para reparación de aspiradoras
Dyson, no automatización de procesos. El formulario de contacto cambia el
campo "empresa" (sin sentido para un cliente particular) por "modelo"
(modelo de la aspiradora, opcional) — actualizado también en
api/contacto.js.

SECCIONES AÑADIDAS (a petición del cliente, con capturas de referencia de un
sitio hermano de la familia — adaptadas al contexto de DysonRepair, sin copiar
literalmente donde no aplicaba):
- "Reparación en 2 horas" (#rapidez), justo después del hero.
- "Confianza" (#confianza), sustituye la antigua tarjeta única de Google por
  dos tarjetas (Google Business + YouTube), con el estilo cobre/grafito.
- Preguntas frecuentes (#faq), antes de la sección SEO final. Se ha ajustado
  la pregunta "¿Qué productos Dyson reparáis?" a "¿Qué aspiradoras Dyson
  reparáis?", porque DysonRepair es específicamente servicio técnico de
  aspiradoras (no seca­dores Supersonic/Airwrap como el sitio de referencia).

ELIMINADO A PETICIÓN DEL CLIENTE: las dos imágenes decorativas del hero
(hero1/hero2, .hero-side-img) y sus reglas CSS asociadas en dysonrepair.css y
dysonrepair-header-hero.css (huérfanas tras quitar las imágenes). Borrados también
los archivos de imagen ya sin ninguna referencia: hero1/hero2-powerflow-*.webp,
logo-1ok-PowerFlow-*.webp (logo antiguo, sustituido por el SVG) e icono.jpg
(favicon antiguo, sustituido por dysonrepair-isotype.svg). NO se ha tocado
img/icono-automatizacion-tuerca-foco.svg (decoración de fondo de la sección
"por qué elegirnos"): sigue enlazada desde dysonrepair-restoration.css, no estaba
huérfana — se borró por error en un primer barrido y se restauró.

CHATBOT: dysonrepair-n8n-chat.js usa el webhook real compartido del grupo
(sswebhookss.affirmatechnology.com), el mismo que el resto de la familia.
Se ha eliminado el script de chat inline y roto que tenía el index.html
original (placeholder 'PENDIENTE_URL_WEBHOOK_N8N_POWERFLOW' nunca
configurado); el chat real ya lo carga dysonrepair.js de forma dinámica, como en
el resto de repos de la familia.

PENDIENTE DE VALORAR POR EL CLIENTE:
- Confirmar la dirección postal exacta (ver arriba).
- La franja "trusted"/clientes (dysonrepair-clients.js, vía dysonrepair-clients.css) usa
  el mismo listado de marcas del Grupo Kelatos que otros repos (Kelatos,
  GameFix, Start Monitor, Surface Labs, DellTech, Video Convert, Alquiler
  Ordenadores Madrid). Se ha mantenido igual que en PowerFlow por ser
  infraestructura compartida de familia, no específica de automatización.
