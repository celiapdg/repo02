## Comandos de Git utilizados
***
### Configuración del dispositivo
Estos comandos normalmente solo se van a realizar una vez por máquina. Sirven para configurar el usuario que estará usando Git.

* `git config --global user.name IntroducirNombreAquí` para añadir un nombre al usuario, su identificación
* `git config --global user.email "correo@electrónico.com"` el correo de la cuenta que queremos asociar. Cuando intentemos conectar con el repositorio de la nube por primera vez, nos pedirá la contraseña. Alternativamente, podemos configurarla con `git config --global user.password "ContraseñaAquí"`

***

### Configuración del repositorio
Comandos que se utilizan (normalmente) una sola vez cuando empezamos a trabajar con un repositorio nuevo.
* `git init` Inicializa un repositorio en la carpeta actual. No servirá si ya se ha inicializado alguno
* `git remote add origin URL` para conectar el repositorio local con el repositorio online (que previamente habremos creado en [GitHub](https://github.com/))
* `git clone URL` para clonar un repositorio remoto en nuestro dispositivo. Para ello, antes deberá existir en [GitHub](https://github.com/). Cuando lo clonemos, ya estará inicializado y vinculado al repositorio remoto.

***
### Trabajando en el repositorio
Cuando trabajemos en el repositorio local. Tenemos que utilizar distintos comandos para ir pasando por los distintos estados.
1. Para pasar a la Staging Area, tenemos que utilizar `git add .` aunque previamente debe haberse hecho algún cambio en los archivos.
2. Para tomar una snapshot y "guardar" el estado actual `git commit -m "mensaje descriptivo"`
3. Para subir los cambios al repositorio remoto, haremos un `git push`

Por el contrario, si hemos hecho cambios en el repositorio remoto (o algún compañero de equipo ha subido los suyos), tendremos que traerlos a nuestra máquina. Para ello, utilizaremos `git pull`

Además, para chequear el estado del repositorio y los commits realizados, existen también los comandos `git status` y `git log` que nos ayudarán a saber el registro de eventos, los archivos trackeados, si hay alguna incidencia, y qué hacer a continuación en base a ello.

### Tabla resumen

| Comando | Descripción |
|:-------:|:------------|
|`git config --global user.name IntroducirNombreAquí`| Añadir un nombre al usuario |
|`git config --global user.email "correo@electrónico.com"`| Añadir correo electrónico |
|`git config --global user.password "ContraseñaAquí"`| Añadir contraseña para vincular completamente la cuenta |
|`git init`| Inicializa un repositorio en la carpeta actual |
|`git remote add origin URL`| Conecta el repositorio local con el remoto |
|`git clone URL`| Clona un repositorio remoto en la ubicación actual |
|`git add .`| Añadir archivos y actualizaciones de los mismos a la staging area |
|`git commit -m "mensaje descriptivo"`| Toma una snapshot de lo que se haya añadido a la staging area |
|`git push`| Sube los cambios al repositorio remoto |
|`git pull`| Trae los cambios del repositorio remoto |
|`git status`| Ver el estado actual del repositorio: archivos cambiados, incidencias... |
|`git log`| Registro de commits: autor, hora, fecha y comentario |