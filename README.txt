PIQUE v08 — URBAN ROUTE + ONLINE LOBBY + LEGAL STARTER

INCLUIDO
- index.html: juego base con mapa de campaña más urbano, detalles de asfalto/calles y ventanas de edificios.
- Pestaña MULTIJUGADOR: interfaz para crear/copiar un código de sala y unirse. Importante: los códigos todavía son locales de demostración; no conectan dos dispositivos. El juego online real requiere un backend realtime configurado.
- Pestaña PRIVACIDAD y páginas privacy.html, terms.html, cookies.html.
- Aviso inicial de privacidad/cookies que recuerda que esta build no carga anuncios.

IMPORTANTE SOBRE GITHUB PAGES Y MONETIZACIÓN
GitHub Pages sirve archivos estáticos y no ejecuta un servidor propio. No puede gestionar por sí solo un matchmaking online seguro. Además, la documentación oficial de GitHub indica que Pages no está destinado a alojar sitios principalmente comerciales o transacciones. Antes de monetizar, revisá sus términos y considerá un hosting de estáticos apto para el proyecto junto con backend separado. Referencia: https://docs.github.com/en/pages/getting-started-with-github-pages/github-pages-limits

MULTIJUGADOR REAL — SIGUIENTE PASO TÉCNICO
La interfaz visual está preparada, pero no se debe anunciar como funcional hasta conectarla a un backend realtime (por ejemplo, Supabase Realtime o Firebase) y probarlo con dos dispositivos. Debe añadirse:
1. Proyecto backend y variables públicas de cliente (nunca incluir claves secretas/service-role en HTML ni GitHub).
2. Salas con código aleatorio generado y validado en backend, expiración, límite de jugadores y reglas de acceso.
3. Sincronización de estado de carrera, reconexión, salida de sala y protección básica contra mensajes falsificados.
4. Pruebas con dos navegadores/dispositivos y mala conexión.

PRIVACIDAD / TÉRMINOS
Los documentos son borradores iniciales, no asesoría legal ni garantía de cumplimiento. Reemplazá [RESPONSABLE], [CORREO DE CONTACTO] y [PAÍS]. Actualizalos si activás un proveedor realtime, cuentas, chat, analítica o anuncios. No cargues scripts de anuncios antes de implementar el consentimiento requerido por el proveedor y las leyes aplicables. El aviso actual no activa anuncios ni es una CMP certificada.

PROBAR LOCALMENTE
Abrí index.html en un navegador moderno. Para probar en servidor local desde una carpeta con Python:
  python -m http.server 8000
Abrí http://localhost:8000

ANTES DE LANZAR
- Probar los 27 circuitos en escritorio y móvil.
- Verificar que el mapa y todas las pestañas respondan bien.
- Configurar backend real y testear sala entre dos dispositivos.
- Completar información legal y revisar privacidad/cookies con asesoría adecuada.
- Elegir una red publicitaria compatible con juegos y su política de tráfico/consentimiento.


PIQUE v09 — RECOMPENSAS Y COLECCIÓN
- Se amplía la colección de naves con 10 diseños adicionales, desde épicos hasta míticos.
- Se amplían los logros con recompensas de monedas por hitos de partidas, fragmentos, victorias, campaña y colección.
- Las compras usan monedas ficticias del juego; no hay pagos reales ni valor monetario.


PIQUE v10 — VEHICLE LAB & DAILY ROTATION
- Garage expanded: motorcycles, cars, helicopter, hovercraft and mech; vehicle purchases change the player sprite in gameplay.
- Character collection includes human, android, cybernetic, robot elite and synthetic AI pilot; selected robot/cyber pilots display a small avatar marker.
- Daily contracts rotate through seven deterministic sets based on the local date; each day changes mission names, goals and rewards. No backend required, local device date is used.
- All prices use fictional gameplay coins; no real-money purchases are implemented.


PIQUE v11 — ORIGINAL SOUNDTRACK
- Added original procedural synth music generated with Web Audio (no external music files or copyrighted tracks).
- Three different loops, one per season: Neon Rush, Jump Circuit and Shard Hunt.
- New footer button toggles background music independently from sound effects. Music starts only after the player clicks the music control, respecting browser autoplay restrictions.
- Music loops are synthesized in-browser; no network requests or music cookies are used.


PIQUE v12 — OVERDRIVE MIX
- Faster original synthesized soundtrack: 148–170 BPM with stronger bass, brighter lead synth and kick/snare-like electronic percussion.
- Master music gain increased from 0.045 to 0.14 (subject to device/browser output volume).
- Music remains separately toggleable from sound effects; no external copyrighted tracks are loaded.
