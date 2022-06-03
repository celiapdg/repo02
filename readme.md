## Comandos de Git utilizados
***
### Configuración del dispositivo
Estos comandos normalmente solo se van a realizar una vez por máquina. Sirven para configurar el usuario que estará usando Git.

* `git config --global user.name IntroducirNombreAquí` para añadir un nombre al usuario, su identificación
* `git condig --global user.email "correo@electrónico.com"` el correo de la cuenta que queremos asociar. Cuando intentemos conectar con el repositorio de la nube por primera vez, nos pedirá la contraseña. Alternativamente, podemos configurarla con `git config --global user.password "ContraseñaAquí"`

***

### Configuración del repositorio
Comandos que se utilizan (normalmente) una sola vez cuando empezamos a trabajar con un repositorio nuevo.
* `git init` Inicializa un repositorio en la carpeta actual. No servirá si ya se ha inicializado alguno
* `git remote add origin URL` para conectar el repositorio local con el repositorio online (que previamente habremos creado en GitHub)
* `git clone URL` para clonar un repositorio remoto en nuestro dispositivo. Para ello, antes deberá existir en GitHub. Cuando lo clonemos, ya estará inicializado y vinculado al repositorio remoto.

