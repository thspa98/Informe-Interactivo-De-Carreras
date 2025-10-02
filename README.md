# Informe-Interactivo-De-Carreras
README — Comparador de Carreras (Aeroespacial vs Industrial)

Proyecto web de una landing minimalista, moderna y responsive inspirada en el estilo Apple. Compara Ingeniería Aeroespacial e Ingeniería Industrial con video de portada, bloques de contenido enfrentados (izq./der.), parallax con imágenes de fondo, timelines con guiones y halo animado al pasar el mouse, y una sección destacada con links oficiales de la UNC.

✨ Características

Video de fondo oscuro y título centrado.

Índice fijo (auto-ocultable): se esconde al bajar y reaparece al subir; resalta la sección activa.

Comparación lado a lado (grid 2 columnas):

Imágenes de fondo apiladas con parallax sutil, visibles a partir de “Motivación e Intereses”, siempre detrás del contenido.

Timelines : guiones centrados sobre la línea vertical con halo animado en hover.

Estadísticas en Argentina: tarjetas con barras y links a fuentes.

Links oficiales UNC en “pills” grises:

Accesible y responsive (desktop y mobile).

🗂 Estructura

Un único archivo HTML con CSS y JS embebidos.

index.html
├─ (video)  video ingenierias.mp4
├─ (img)    wp8215382-spacex-starship-wallpapers.jpg       # nave
└─ (img)    ingenieria-industrial-datos-desconocidos-678x381.jpg  # operario/industrial

Importante: guardá el video e imágenes en la misma carpeta que index.html y con exactamente esos nombres (o actualizá las rutas en el HTML).

🔗 Links UNC (editar textos/URLs)

Sección “Links oficiales de la UNC”:

<a class="link-pill pill-aero" href="URL_AERO" target="_blank">Ingeniería Aeroespacial — UNC</a>
<a class="link-pill pill-industrial" href="URL_IND" target="_blank">Ingeniería Industrial — UNC</a>

📊 Estadísticas (fuentes y edición)

Las tarjetas están en la sección “Estadísticas en Argentina”.
Podés cambiar valores y fuentes (se muestran como enlaces):

Graduados aeroespaciales: Infobae (2018), Min. Ciencia, IUA.

Graduados totales de Ingeniería y egreso a tiempo: CAI, CIN, Min. Educación, Infobae (2018).

Nota: Las cifras están presentadas como órdenes de magnitud para contexto comparativo. Actualizá con fuentes más recientes si lo necesitás.

🧩 Dependencias

AOS (Animate on Scroll) vía CDN:

<link href="https://unpkg.com/aos@2.3.1/dist/aos.css" rel="stylesheet">
<script src="https://unpkg.com/aos@2.3.1/dist/aos.js"></script>
<script>AOS.init({ duration: 1200, once: true });</script>

No requiere build ni paquetes adicionales.

♿ Accesibilidad

Contraste alto en textos clave (amarillo/violeta sobre fondos oscuros).

Enlaces con texto descriptivo y rel="noopener" en targets externos.

Video con aria-label.

Animaciones discretas; se pueden reducir bajando opacidades o desactivando animation/box-shadow en CSS.

🧱 Secciones principales del HTML (para ubicarte)

<header>: video y título.

#motivacion: comparación inicial (grid 2 columnas).

Parallax container (desde aquí aparecen los fondos).

#estadisticas: tarjetas con barras y links.

#links-unc: pills con enlaces oficiales.

#instituciones: dónde se cursa y duración.

#planes: timelines con guiones + halo.

#conclusion: cierre.

<nav.topnav>: índice fijo (autohide + sección activa).

🐞 Problemas comunes

No se ve el video: confirmá que el archivo se llama video ingenierias.mp4 y que el navegador permite reproducir autoplay muted.

Fondos no aparecen: verificá los nombres de las imágenes y rutas.

Fuentes no resaltan: CDN de AOS bloqueado; probá otra conexión o quitá data-aos="..." (funciona igual sin animaciones).

📄 Licencia y créditos

El diseño y el código de esta landing pueden usarse libremente para fines educativos.

Imágenes y video: reemplazá por material propio o con licencia compatible (las rutas usadas son ejemplos provistos por el usuario).

Librería AOS se usa desde su CDN oficial.

✍️ Autor

Por Thomás Spalletti — 2025.
