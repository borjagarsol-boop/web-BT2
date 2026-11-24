# Web de BT2 Inversiones (bt2.es)

Web estática (HTML + CSS, sin JavaScript ni cookies).

- `index.html` — página principal
- `aviso-legal.html`, `privacidad.html`, `404.html`
- `assets/` — estilos, tipografías y logos
- `.htaccess` — HTTPS, cabeceras de seguridad y caché (Apache / Arsys)

## Publicación

Cada cambio en la rama `main` se sube automáticamente a Arsys por SFTP
(`.github/workflows/publicar.yml`). Necesita estos secretos en
GitHub → Settings → Secrets and variables → Actions:

| Secreto | Qué es |
|---|---|
| `FTP_SERVER` | Servidor FTP de Arsys |
| `FTP_USERNAME` | Usuario FTP |
| `FTP_PASSWORD` | Contraseña FTP |
| `FTP_SERVER_DIR` | (Opcional) carpeta de la web en el servidor, terminada en `/`. Si no se pone, se detecta sola |
