# mI Amigo

Web informativa de asistentes de IA por suscripción mensual. Inglés US$4,99/mes, Gimnasio US$9,99/mes y Chef US$9,99/mes. Binance Pay como medio previsto, QR original con nombre visible Cripto Agency Auto y confirmación manual prevista al +591 62230618, pendiente de activar.

## Estado
Código cargado; alojamiento externo aún pendiente. No se ha activado GitHub Pages ni Cloudflare. No se ha confirmado que Meta acepte una URL nueva. La contratación sigue en prelanzamiento hasta completar identidad legal, condiciones y canal activo. La web no procesa pagos ni activa asistentes.

## Publicar en Cloudflare Pages desde GitHub
1. En Cloudflare: Workers & Pages → Create application → Pages → Import an existing Git repository.
2. Seleccionar CarvajalAutomatizaciones/mI-Amigo. Autorizar solo este repositorio si es suficiente.
3. Configurar: rama main; preset None; Build command exit 0; Build output directory public; Root directory vacío.
4. Save and Deploy. Usar la URL exacta devuelta por Cloudflare, no adivinar un subdominio.
5. Verificar acceso anónimo HTTP 200 a portada y páginas legales; después probar la URL en el formulario de Meta. No se garantiza aceptación de Meta sin esa comprobación.

No activar analítica, píxeles, Access ni desafíos interactivos sin evaluar su necesidad y los efectos sobre privacidad/acceso público. No se promete que ningún proveedor vaya a aceptar todos los rastreadores.

## Por qué no GitHub Pages
La política oficial no permite usar Pages como alojamiento gratuito para operar un negocio online o un sitio principalmente dirigido a transacciones comerciales o SaaS comercial. Esta web incluye planes y medios de pago; GitHub se usa como repositorio, no como hosting comercial.
https://docs.github.com/en/pages/getting-started-with-github-pages/github-pages-limits

## Seguridad y recursos
public/ contiene el sitio listo para publicar, banner estático original optimizado para escritorio/móvil y siete páginas legales. Sin WebGL, vídeo, frameworks, fuentes remotas ni rastreadores añadidos. El QR se conserva íntegro. _headers incorpora CSP, frame-ancestors, nosniff, referrer y permisos para Cloudflare Pages; su aplicación debe verificarse después del despliegue. No es una auditoría de backend ni garantía de ausencia de multas o vulnerabilidades.

## Comprobaciones
python verify.py
python verify-commercial.py
node verify-selector.cjs

Fuentes de despliegue: https://developers.cloudflare.com/pages/framework-guides/deploy-anything/ y https://developers.cloudflare.com/pages/configuration/headers/
