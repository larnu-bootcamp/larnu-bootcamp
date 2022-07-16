# Desafío: Git

### Pre-requisitos

* Crear una cuenta en [Github.com](https://www.github.com/).
* Si usas una computadora con Windows, puedes instalar la terminal de comandos _git-bash_ haciendo click [acá](https://git-for-windows.github.io/).
* Si usas Mac, `git` viene pre-instalado y puedes acceder desde la terminal pulsando ⌘+Espacio y escribiendo "terminal". Puedes asegurarte de que git está instalado escribiendo `which git` en la terminal y pulsando Enter, si aparece la ruta de un archivo está todo correcto. En algunas ocasiones, podrías ser redireccionado a la descarga de la línea de comandos de Xcode, sigue las instrucciones.
* Si usas Linux, tal vez necesites instalar git accediendo a tu terminal e ingresado `apt-get install git`
* Si tienes problemas instalando Git, este recurso puede servir de ayuda: [Instalación de Git](https://git-scm.com/book/es/v2/Inicio---Sobre-el-Control-de-Versiones-Instalaci%C3%B3n-de-Git)


### Comandos básicos de terminal

> Usaremos la "terminal" o "línea de comandos" durante tu tiempo en LarnU. Si estás en una computadora con Mac o Linux, deberías tener la terminal y git ya instalados. Si estás en una máquina con Windows, te recomendamos instalar ["git-bash"](https://gitforwindows.org/).

Dentro de nuestra terminal podemos: revisar nuestra estructura de archivos, añadir, eliminar y modificar archivos, y muchas cosas más. La terminal es una herramienta muy poderosa para los desarrolladores y vas a usarla mucho en tu carrera profesional. Al principio puede parecer aterrador, pero con el tiempo terminarás disfrutando su uso, así que es mejor acostumbrarse ahora. Para comenzar, aprenderemos los comandos "básicos":

"List": Nos permite ver el contenido de la carpeta donde nos encontramos.
```bash
  $ ls
```


"Change Directory": Nos permite movernos a una nueva carpeta o "directorio"
```bash
  $ cd [carpeta]
```

"Make Directory": Crea una nueva carpeta en el directorio donde nos encontramos actualmente.
```bash
  $ mkdir [nombre de la carpeta]
```

"Touch" creará un nuevo archivo.
```bash
  $ touch [nombre del archivo]
```

"Remove": Elimina permanentemente un archivo. ¡CUIDADO! Esto traspasa cualquier "papelera de reciclaje" que exista en el sistema y elimina los archivos PERMANENTEMENTE. Como nota, esto no eliminará carpetas, necesitamos un comando especial para eso que aprenderemos más adelante.

```bash
  $ rm [nombre del archivo]
```

## Crea un repositorio de Git y haz tu primer commit

Le indicaremos a Git que queremos crear un nuevo repositorio para utilizar un sistema de control de versiones.
Solo debemos posicionarnos en la carpeta raíz de nuestro proyecto y ejecutar el comando git init.

Recuerda que al ejecutar este comando (y de aquí en adelante) vamos a tener una nueva carpeta llamada **.git** con toda la base de datos con cambios atómicos en nuestro proyecto.

Recuerda que Git está optimizado para trabajar en equipo, por lo tanto, debemos darle un poco de información sobre nosotros. No debemos hacerlo todas las veces que ejecutamos un comando, basta con ejecutar solo una vez los siguientes comandos con tu información:

```shell
git config --global user.name "tu nombre"
git config --global user.email "tu@email.com"
```

Existen muchas otras configuraciones de Git que puedes encontrar en el comando git config --list (o solo git config para ver una explicación más detallada)

## Ejercicio

En este ejercicio crearemos un nuevo repositorio en Github y a partir de la linea de comandos crearemos un nuevo archivo y lo agregaremos a nuestro nuevo repositorio.

Iniciaremos creando una carpeta desde la consola llamada: "LarnU"

Para ello primero iremos a la carpeta de nivel superior, escribe en la consola:

```bash
  cd ~
```

y presiona Enter. Una vez estés en el nivel superior, escribe:

```bash
  mkdir LarnU
```

y presiona Enter. ¡Felicitaciones, has creado un directorio!

### Crear un Repositorio

Entra a github.com y logueate con tu usuario. Luego en la parte de arriba a la derecha buscá el signo '+' y elige 'new repository'.

![alt](../../_src/assets/01-Git/repo-create.png)

En la nueva pantalla, vas a tener que seleccionar el nombre de tu nuevo repo. Crea un repo que se llame: `repositorio-LarnU`. Puedes agregarle una descripción también, pero no es obligatoria.

![alt](../../_src/assets/01-Git/create-repository-name.png)

Luego elige la visibilidad del proyecto como público.

Por último haz clic en **Crear repositorio**.

Listo ya tienes tu propio repo. Ahora vas a poder clonarlo con las intrucciones de más abajo.

### Clonar

Para poder trabajar en un proyecto debes clonarlo (descargarlo) a tu máquina local. Para ello, accede al repositorio que creaste en tu cuenta, y haz click en el botón de la esquina superior derecha que dice "Clonar o descargar". Un dropdown aparecerá y podemos clickear en el icono del clipboard para copiar la dirección del repo. O, si el repo esta vacio vas a ver en el medio de la pantalla la URL con la dirección de tu repositorio.

Una vez tengas la dirección copiada, abre una terminal nueva y escribe lo siguiente:


```bash
  $ cd ~

  $ cd LarnU

  $ git clone [dirección copiada]
```

Esto descargará el repositorio y tendrás disponible una copia local guardada en tu máquina.

### Comandos de git:

Durante estas lecciones interactuaremos con git a través de la terminal. En el futuro, podrías estar interesado en usar una interfaz visual/gráfica, pero durante estas lecciones necesitaremos usar la terminal para acceder a todas las funciones de git.

En este ejercicio, añadiremos un archivo a nuestro proyecto y crearemos un commit para cambiar la "memoria" de git.

A continuación, escribe lo siguiente en tu terminal:

```bash
  $ cd rrepositorio-LarnU
  
  $ touch archivo-ejemplo.html
```

Esto añadirá un nuevo archivo llamado "archivo-ejemplo.html" a tu proyecto.

En este momento, podemos usar el comando de git "status", esto nos mostrará los cambios hechos en el repositorio local. Usa "status" si no estás seguro de que algo haya funcionado y necesitas saber qué pasó.

```bash
  $ git status
```

Deberías ver algo parecido a estas líneas:

```bash
  Changes not staged for commit:
    (use "git add <file>..." to update what will be committed)
    (use "git checkout -- <file>..." to discard changes in working directory)

    modified:   README.md

  Untracked files:
    (use "git add <file>..." to include in what will be committed)

    archivo-ejemplo.html

  no changes added to commit (use "git add" and/or "git commit -a")
```

Esto nos dice que tenemos un archivo que ha cambiado, pero todavía no ha sido guardado en el historial de git.

Para hacer esto, usaremos el comando "add":


```bash
  git add archivo-ejemplo.html
```

Esto agregó nuestros cambios al historial. Ahora, para guardar el historial, usaremos el comando "commit". Commit agarrará todos nuestros cambios y los guardará en el historial de git. Para futuras referencias, podrás añadir un mensaje acerca de los cambios hechos, esto facilitará ir atrás en el historial y encontrar los cambios que tú (o cualquiera) busque en el futuro en caso de necesitarlo. Siempre es una buena idea hacer una descripción clara y concisa de los cambios. Un _shorthand_ para añadir un mensaje, es usar la bandera (flag) "-m" y escribir el mensaje a continuación usando comillas.

```bash
  git commit -m 'Agregado nuevo archivo, archivo-ejemplo.html'
```

Ahora que guardamos nuestros cambios localmente, vamos a querer compartir esos cambios en Github. Para ello, usaremos "push":

```bash
  git push
```

La terminal te preguntará tu usuario y contraseña (En el caso de la contraseña cuando la estemos escribiendo por consola, por cuestiones de seguridad no se verá lo que estamos escribiendo). Escribimos estos datos y a continuación le damos enter y veremos un mensaje si todo fue "pusheado" correctamente:

```bash
  Counting objects: 5, done.
  Delta compression using up to 8 threads.
  Compressing objects: 100% (4/4), done.
  Writing objects: 100% (5/5), 2.97 KiB | 0 bytes/s, done.
  Total 5 (delta 1), reused 0 (delta 0)
  remote: Resolving deltas: 100% (1/1), completed with 1 local object.
  To git@github.com:[your username]/Precourse.git
    cccc682..283b9dd  master -> master
```

¡Felicitaciones, acabas de subir tu primer git commit!
