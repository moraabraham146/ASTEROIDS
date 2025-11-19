# Anuncios (Google AdSense) — notas rápidas

- He insertado tu snippet de Google AdSense en el pie de `index.html` y `ASTEROIDS.html`.
- Para que los anuncios se muestren en producción necesitas verificar el dominio en tu cuenta de AdSense y esperar la activación.
- Para desactivar los anuncios temporalmente durante pruebas, comenta o elimina el bloque que contiene:

```html
<script async src="https://pagead2.googlesyndication.com/pagead/js/adsbygoogle.js?client=ca-pub-7949714288717188" crossorigin="anonymous"></script>
<ins class="adsbygoogle" ...></ins>
<script>(adsbygoogle = window.adsbygoogle || []).push({});</script>
```

- Ten en cuenta las políticas de privacidad y GDPR: si tu sitio tiene visitantes en la UE podrías necesitar un aviso de cookies/consentimiento.
