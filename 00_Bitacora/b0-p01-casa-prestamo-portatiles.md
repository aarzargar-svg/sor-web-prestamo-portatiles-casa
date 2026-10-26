- **Alumno:** Aarón Zaragoza García
- **Bloque:** Practica_01_Casa_Prestamo_Portatiles
- **Fase / ejercicio:** Fase 0.2
- **Fecha de inicio:** 26/10/2026
- **Fecha de entrega:** 26/10/2026

---

## 🎯 Qué se pedía

Crear una bóveda nueva en Obsidian con un proyecto HTML para gestionar el préstamo de portátiles. Había que crear un repositorio Git, conectarlo con GitHub y guardar tres versiones de la web, comprobando los cambios y recuperando la primera versión. También había que crear páginas nuevas, añadir una imagen y evitar que los vídeos se subieran a GitHub.

## ⌨️ Comandos y pasos importantes

- `pwd`: comprobar en qué carpeta estoy.
    
- `git init`: crear el repositorio local.
    
- `git branch -M main`: establecer el nombre de la rama principal.
    
- `git status`: ver el estado de los archivos.
    
- `git remote add origin`: conectar el proyecto con GitHub.
    
- `git add`: preparar los archivos que quiero guardar.
    
- `git diff`: comprobar los cambios realizados.
    
- `git diff --cached --stat`: ver un resumen de los archivos preparados.
    
- `git commit -m "mensaje"`: guardar una versión del proyecto.
    
- `git push`: subir los commits a GitHub.
    
- `git log --oneline`: consultar el historial.
    
- `git check-ignore -v`: comprobar qué regla ignora los vídeos.
    
- `git switch --detach`: visitar una versión anterior.
    
- `git switch main`: volver a la versión actual.


## 🛠️ Qué he hecho

He creado la bóveda `Boveda_HTML_Casa` y el proyecto dentro de `01_Proyecto`. Después, he creado la página inicial y he configurado Git y la conexión con mi repositorio de GitHub.

He guardado tres versiones de la web: la inicial con el portátil disponible, otra con el portátil reservado para mantenimiento y una última con las páginas de normas y contacto, además de una imagen. Por último, he comprobado el historial y he vuelto a la rama `main`.


## 🚩 Qué me ha fallado y cómo lo he resuelto

He tenido un problema con la carpeta SOR_casa y a sido que al poner dentro de documentos, cuando tenia que hacer ls -l la carpeta no aparecia, pero he descubierto que si en vez de guardarla en documentos, la guardaba en descargas si aparecia.



## 🤔 Respuestas a las preguntas

¿Por qué git init se hizo en 01_Proyecto y no en la raíz de la bóveda?

Porque quería que Git controlara únicamente los archivos del proyecto y no las configuraciones de Obsidian ni las grabaciones. Así mantengo todo organizado.

Antes de `add`, mostró los archivos nuevos sin seguimiento o los cambios sin preparar. Después de `add`, aparecieron como preparados para el siguiente commit. Después de `commit`, el estado quedó limpio, sin cambios pendientes.

¿Qué mostró git status antes de add , después de add y después de commit ?

Porque la práctica de casa debía tener un repositorio independiente del proyecto del centro. Con `git remote add origin` guardé la dirección de ese repositorio para poder subir los cambios con `git push`.

¿Por qué creaste un repositorio de GitHub propio y lo conectaste con git remote add origin ?

¿Por qué las páginas nuevas aparecen en git status pero no en git diff -- web/index.html ?

Porque `git status` muestra también los archivos nuevos sin seguimiento, mientras que `git diff -- web/index.html` muestra los cambios de ese archivo concreto, no el contenido de las páginas nuevas.

¿Cómo has comprobado que los vídeos existen pero no se van a subir?

He comprobado que los vídeos están en la carpeta `web/videos` y he utilizado `git check-ignore -v` para verificar que la regla `*.mp4` de `.gitignore` los excluye de Git.

¿Qué muestra git diff --cached --stat después de preparar los cuatro archivos?

Muestra un resumen de los cuatro archivos preparados: `index.html`, `normas.html`, `contacto.html` y `imagenes/portatil.png`, indicando las modificaciones y las líneas añadidas o eliminadas.

¿Qué cambia al visitar el primer commit y qué recuperas al volver a main ?

Al visitar el primer commit, la web vuelve a su estado inicial, con el portátil disponible y sin la imagen ni los enlaces nuevos. Al regresar a `main`, recupero la versión actualizada con el estado de mantenimiento, la imagen y las páginas adicionales.

¿Por qué esta web necesita historial? ¿Qué aportaría GitHub si otro técnico trabajase contigo?

Porque la web puede cambiar y el historial permite saber qué se ha modificado, comparar versiones y recuperar una anterior si algo falla. GitHub permitiría compartir el código y los cambios con otros técnicos para trabajar de forma coordinada.

Si mañana corriges una errata en normas.html , ¿qué pasos repites y cuáles no?

Repetiría la edición del archivo, la comprobación con `git status` y `git diff`, el `git add`, el `git commit` y el `git push`. No tendría que repetir `git init` ni `git remote add origin`, porque el repositorio y la conexión con GitHub ya están configurados.


## 🔗 Enlaces


- **Vídeo de esta fase:**  https://youtu.be/Y6i3a02aeNQ
- **Playlist:** https://www.youtube.com/playlist?list=PLCxp8AVxoTh4

## 💭 Dudas / a repasar


- [ ]  nada.