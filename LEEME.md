# Sitio el geek. — cómo publicarlo en GitHub Pages

## 1. Sube el sitio
1. En github.com crea un repositorio **público** llamado `elgeekmarketer-web`.
2. Botón **Add file → Upload files** y arrastra todo el contenido de esta carpeta (index.html, img, video, CNAME, .nojekyll). Confirma con **Commit changes**.
3. En el repo: **Settings → Pages → Build and deployment → Source: Deploy from a branch**, rama `main`, carpeta `/ (root)`. Guarda.
4. En 1–2 minutos queda en `https://TU-USUARIO.github.io/elgeekmarketer-web/`.

## 2. Conecta tu dominio (elgeekmarketer.com)
El archivo `CNAME` ya dice `elgeekmarketer.com`. En el panel donde compraste el dominio, configura el DNS:

| Tipo | Nombre | Valor |
|---|---|---|
| A | @ | 185.199.108.153 |
| A | @ | 185.199.109.153 |
| A | @ | 185.199.110.153 |
| A | @ | 185.199.111.153 |
| CNAME | www | TU-USUARIO.github.io |

Luego en **Settings → Pages** escribe `elgeekmarketer.com` en *Custom domain* y activa **Enforce HTTPS** cuando aparezca (puede tardar hasta 24 h).

Ojo: si ya usas el dominio para correo, **no toques los registros MX**.

## 3. Pega el formulario de charlas
En `index.html` busca `PEGA AQUÍ EL IFRAME` y reemplaza el comentario por el iframe de Brevo o monday. Borra la línea "Aquí va el formulario…".

## 4. Cómo actualizar (y tus versiones)
Edita el archivo en GitHub (ícono de lápiz) o sube la nueva versión con **Upload files**. Cada cambio queda en **History**: ahí puedes ver y regresar a cualquier versión anterior.
