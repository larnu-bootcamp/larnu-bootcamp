![LarnU](_src/assets/00-PrimerosPasos/logo_LarnU.png)

<br>
<br>

# Bienvenido al bootcamp de LarnU 馃懡

## Desaf铆os

En este [link](https://github.com/larnu-bootcamp/larnu-bootcamp.git) vas a encontrar el repositorio con los desafi贸s de cada unidad en su correspondiente carpeta.

## Canales de DISCORD

![LarnU](_src/assets/00-PrimerosPasos/discord.png)


## Editores de Texto

Los editores de c贸digo son programas que nos ayudan a gestionar el c贸digo fuente de nuestros proyectos. Son ideales cuando se trabaja con diferentes lenguajes de programaci贸n, altern谩ndolos o en un solo proyecto (por ejemplo, en un proyecto web es muy habitual combinar html, javascript, css, php, etc.).

Hay varios editores de c贸digo, pero en este bootcamp trabajaremos con Visual Studio Code.

### Visual Studio Code

![VSC Console](_src/assets/00-PrimerosPasos/vsc_console.png)

Es un editor desarrollado por Microsoft.

Tiene integrado el control de versiones mediante Git y Github para tener un seguimiento de tus proyectos. Brinda una cantidad de extensiones que facilitan el trabajo de un desarrollador.

Para descargarlo, nos dirigimos al sitio oficial, en la secci贸n Dowload y descargamos el instalador seg煤n nuestro Sistema Operativo:

<https://code.visualstudio.com/download>

![VSC Download](_src/assets/00-PrimerosPasos/vsc_download.png)

Una vez finalizada la descarga, procedemos a ejecutar el instalador.

## Instalando Node.JS

Para instalar Node js en nuestra computadora, nos dirigimos al sitio oficial:

<https://nodejs.org/es/>

Al ingresar, el sitio detectar谩 nuestro Sistema Operativo y nos sugerir谩 que descarguemos el instalador adecuado.

![Node.JS Screen](_src/assets/00-PrimerosPasos/nodejs_screen.png)

Para proceder a la descarga, seleccionamos la versi贸n LTS, que es la versi贸n estable.
Una vez finalizada la descarga, procedemos a ejecutar el instalador.

Para corroborar que Node js se instal贸 correctamente, procedemos a ejecutar el siguiente comando por la consola o terminal de nuestro sistema operativo:

```shell
node -v
```

Y si seguimos los pasos anteriores, la consola o terminal, nos devolver谩 la versi贸n de Node js que tenemos instalada:

```shell
v12.18.3
```

<br>
<br>

# GIT

## 驴Por qu茅 usar un sistema de control de versiones como Git?
Un sistema de control de versiones como Git nos ayuda a guardar el historial de cambios y crecimiento de los archivos de nuestro proyecto.

En realidad, los cambios y diferencias entre las versiones de nuestros proyectos pueden tener similitudes, algunas veces los cambios pueden ser solo una palabra o una parte espec铆fica de un archivo espec铆fico. Git est谩 optimizado para guardar todos estos cambios de forma at贸mica e incremental, o sea, aplicando cambios sobre los 煤ltimos cambios, estos sobre los cambios anteriores y as铆 hasta el inicio de nuestro proyecto.

## 驴Qu茅 es Git?

Git es un sistema de control de versiones distribuido, dise帽ado por Linus Torvalds. Est谩 pensando en la eficiencia y la confiabilidad del mantenimiento de versiones de aplicaciones cuando estas tienen un gran n煤mero de archivos de c贸digo fuente.

Git est谩 optimizado para guardar cambios de forma incremental.

Permite contar con un historial, regresar a una versi贸n anterior y agregar funcionalidades.

Lleva un registro de los cambios que otras personas realicen en los archivos.

Git fue dise帽ado para operar en un entorno Linux. Actualmente, es multiplataforma, es decir, es compatible con Linux, MacOS y Windows. En la m谩quina local se encuentra Git, se utiliza bajo la terminal o l铆nea de comandos y tiene comandos como merge, pull, add, commit y rebase, entre otros.

## Instalaci贸n

### Para Mac y Linux

Ver estos enlaces:

<https://git-scm.com/book/es/v2/Inicio---Sobre-el-Control-de-Versiones-Instalaci%C3%B3n-de-Git>

<https://www.youtube.com/watch?v=PSULlxUk744>

<https://www.youtube.com/watch?v=oV0spTF71AI>

### Para Windows

Ingreso a <https://git-scm.com> y descargo la 煤tlima versi贸n.

![installGit](_src/assets/00-PrimerosPasos/instalar_window.png)

Una vez descargado, se abre el archivo .exe y van a visualizar la siguiente ventana

![installGit](_src/assets/00-PrimerosPasos/1.png)

Clickeamos 鈥淣ext鈥? hasta que llegamos a esta parte:

![installGit](_src/assets/00-PrimerosPasos/2.png)

En este momento de la instalaci贸n si quieres puedes elegir el editor de texto que van a usar. (Importante, t茅nganlo instalado antes de instalar Git)

Seguimos clickeando 鈥淣ext鈥? y luego 鈥淚nstall鈥?

![installGit](_src/assets/00-PrimerosPasos/3.png)

Por 煤ltimo, finalizar! Si seleccionan la opci贸n "Launch Git Bash", una vez que finalizan la instalaci贸n se va a abrir la consola

![installGit](_src/assets/00-PrimerosPasos/4.png)

Otra forma de abrir la consola es haciendo click derecho sobre el escritorio y elegir la opci贸n "Git Bash Here"

![installGit](_src/assets/00-PrimerosPasos/consola.png)

Una vez instalado Git van a poder visualizar la consola: ingresamos el comando `git --version` para chequear que est谩 instalado. Si ven la consola as铆, ya est谩n listos para comenzar a trabajar!

![installGit](_src/assets/00-PrimerosPasos/5.png)


## Uso de Git

Existen muchas formas de usar Git. Por un lado tenemos las herramientas originales de l铆nea de comandos, y por otro lado tenemos una gran variedad de interfaces de usuario con distintas capacidades. 

## Historia de Git

Como muchas de las grandes cosas en esta vida, **Git** comenz贸 con un poco de destrucci贸n creativa y encendida pol茅mica. El n煤cleo de Linux es un proyecto de software de c贸digo abierto con un alcance bastante grande. Durante la mayor parte del mantenimiento del n煤cleo de Linux (1991-2002), los cambios en el software se pasaron en forma de parches y archivos. En 2002, el proyecto del n煤cleo de Linux empez贸 a usar un DVCS propietario llamado **BitKeeper**.

En 2005, la relaci贸n entre la comunidad que desarrollaba el n煤cleo de Linux y la compa帽铆a que desarrollaba BitKeeper se vino abajo, y la herramienta dej贸 de ser ofrecida gratuitamente. Esto impuls贸 a la comunidad de desarrollo de Linux (y en particular a Linus Torvalds, el creador de Linux) a desarrollar su propia herramienta basada en algunas de las lecciones que aprendieron durante el uso de BitKeeper. Algunos de los objetivos del nuevo sistema:

- Velocidad
- Dise帽o sencillo
- Fuerte apoyo al desarrollo no lineal (miles de ramas paralelas)
- Completamente distribuido
- Capaz de manejar grandes proyectos (como el n煤cleo de Linux) de manera eficiente (velocidad y tama帽o de los datos)

Desde su nacimiento en 2005, Git ha evolucionado y madurado para ser f谩cil de usar y a煤n conservar estas cualidades iniciales. Es tremendamente r谩pido, muy eficiente a gran escala, y tiene un incre铆ble sistema de ramificaci贸n (branching) para desarrollo no lineal.

## Comenzando a usar Git

## Conceptos importantes de Git

- Bug: Error en el c贸digo

- Repository: Donde se almacena todo el proyecto, el cual puede vivir tanto en local como en remoto. El repositorio guarda un historial de versiones y, m谩s importante, de la relaci贸n de cada versi贸n con la anterior para que pueda hacerse el 谩rbol de versiones con las diferentes ramas.

- Fork: Si en alg煤n momento queremos contribuir al proyecto de otra persona, o si queremos utilizar el proyecto de otro como el punto de partida del nuestro. Esto se conoce como 鈥渇ork鈥?.

- Clone: Una vez se decide hacer un fork , hasta ese momento s贸lo existe en GitHub. Para poder trabajar en el proyecto, toca clonar el repositorio elegido al computador personal.

- Branch: Es una bifurcaci贸n del proyecto que se est谩 realizando para anexar una nueva funcionalidad o corregir un bug.

- Master: Rama donde se almacena la 煤ltima versi贸n estable del proyecto que se est谩 realizando. La rama master es la que est谩 en producci贸n en cada momento (o casi) y deber铆a estar libre de bugs. As铆, si esta rama est谩 en producci贸n, sirve como referente para hacer nuevas funcionalidades y/o arreglar bugs de 煤ltima hora.

- Commit: consiste en subir cosas a la versi贸n local del repositorio. De esta manera se puede trabajar en la rama de forma local sin tener que modificar ninguna versi贸n en remoto ni tener que tener la 煤ltima versi贸n remota, cosa muy 煤til en grandes desarrollos trabajados por varias personas.

- Push: Consiste en enviar todo lo que se ha confirmado con un commit al repositorio remoto. Aqu铆 es donde se une nuestro trabajo con el de los dem谩s.

- Checkout: Acci贸n de descargarse una rama del repositorio GIT local (s铆, GIT tiene su propio repositorio en local para poder ir haciendo commits) o remoto.

- Fetch: Actualiza el repositorio local bajando datos del repositorio remoto al repositorio local sin actualizarlo, es decir, se guarda una copia del repositorio remoto en el local.

- Merge: La acci贸n de merge es la continuaci贸n natural del fetch. El merge permite unir la copia del repositorio remoto con tu repositorio local, mezclando los diferentes c贸digos.

- Pull: Consiste en la uni贸n del fetch y del merge, esto es, recoge la informaci贸n del repositorio remoto y luego mezcla el trabajo en local con esta.

- Diff: Se utiliza para mostrar los cambios entre dos versiones del mismo archivo.
## Comandos b谩sicos

- `git init`: se utiliza para iniciar nuestro repositorio.
- `git add ArchivoEjemplo.html`: crea el archivo pero no lo guarda de forma definitiva, lo almacena en (Staging Area).
- `git commit -m "versi贸n 1"`: aqu铆 se generan cambios de "Staging Area" y con ( -m "") se deja un mensaje que nos sea 煤til.
- `git add .`: Agrega los archivos actualizados al repositorio, pero 煤nicamente en la carpeta que te encuentras.
- `git commit -m "Cambios v1"`: sirve para generar cambios sobre la versi贸n antigua.
- `git status`: sirve para revisar si has modificado o guardado los cambios hechos.
- `git log "archivo.txt"`: sirve para ver el historial del archivo.
- `git push`: sirve para enviar cambios al repositorio remoto.
- `git pull`: sirve para recibir cambios de repositorio remoto a local.
- `ls`: listado de carpetas en donde me encuentro. Es decir, como emplear dir en windows.
- `pwd`: ubicaci贸n actual
- `mkdir`: make directory nueva carpeta
- `touch archivo.extensi贸n`: crear archivo vac铆o
- `cat archivo.extensi贸n`: muestra el contenido del archivo
- `history`: historial de comandos utilizados durante esa sesi贸n
- `rm archivo.extensi贸n`: Eliminaci贸n de archivo
- `--help`: ayuda sobre el comando
- `git checkout`: traer cambios realizados
- `git rm --cached archivo.extensi贸n`: se utiliza para devolver el archivo que se tiene en ram. Cuando escribimos git add, lo devuelve a estado natural mientras est谩 en staging.
- `git config --list`: muestra la lista de configuraci贸n de git
- `git config --list --show-origin`: rutas de acceso a la configuraci贸n de git
- `git log archivo.extensi贸n`: muestra la historia del archivo

## Ciclos de vida o estados de los archivos en Git

Para iniciar un repositorio, o sea, activar el sistema de control de versiones de Git en tu proyecto, solo debes ejecutar el comando `git init`.

Este comando se encargar谩 de dos cosas: primero, crear una carpeta `.git`, donde se guardar谩 toda la base de datos con cambios at贸micos de nuestro proyecto; y segundo, crear un 谩rea que conocemos como Staging, que guardar谩 temporalmente nuestros archivos (cuando ejecutemos un comando especial para eso) y nos permitir谩, m谩s adelante, guardar estos cambios en el repositorio (tambi茅n con un comando especial).

Por otro lado cuando trabajamos con Git nuestros archivos pueden vivir y moverse entre 4 diferentes estados (cuando trabajamos con repositorios remotos pueden ser m谩s estados, pero lo estudiaremos m谩s adelante):

- **Archivos** ***Tracked***: son los archivos que viven dentro de Git, no tienen cambios pendientes y sus 煤ltimas actualizaciones han sido guardadas en el repositorio gracias a los comandos `git add` y `git commit`.

- **Archivos** ***Staged***: son archivos en staging. Viven dentro de Git y hay registro de ellos por que han sido afectados por el comando `git add`, aunque no sus 煤ltimos cambios. Git ya sabe de la existencia de estos 煤ltimos cambios, pero todav铆a no han sido guardados definitivamente en el repositorio por que falta ejecutar el comando `git commit`.

- **Archivos** ***Unstaged***: entiendelos como archivos "Traked pero Unstaged". Son archivos que viven dentro de Git pero no han sido afectados por el comando `git add` ni mucho menos por `git commit`. Git tiene un registro de estos archivos, pero esta desactualizado, sus 煤ltimas versiones solo estan guardadas en su disco duro.

- **Archivos** ***Untracked***: son archivos que NO viven dentro de Git, solo en el disco duro. Nunca han sido afectados por `git add`, asi que Git no tiene registro de su existencia. 
Recuerda que hay un caso muy raro donde los archivos tienen dos estados al mismo tiempo: Staged y Untracked. Esto pasa cuando guardas los cambios de un archivo en el 谩rea de Staging (con el comando `git add`), pero antes de hacer commit para guardar los cambios en el repositorio haces nuevos cambios que todav铆a no han sido guardados en el 谩rea de Staging (en realidad, todo sigue funcionando igual pero es un poco divertido).

### Comandos para mover archivos entre los estados de Git

- `git status`: nos permite ver el estado de todos nuestros archivos y carpetas.

- `git add`: nos ayuda a mover archivos del Untracked o Unstaged al estado Staged. Podemos usar git nombre del archivo o carpeta para a帽adir archivos y carpetas individuales o git add -a para mover todos los archivos de nuestro proyecto ( tanto Untrackeds como Unstageds).

- `git reset HEAD`: nos ayuda a sacar los archivos del estado Staged para devolverlos a su estado anterior. Si los archivos venian de Unstaged, vuelven alli. Y lo mismo si venian de Untracked.

- `git commit`: nos ayuda a mover archivos de Unstaged a Tracked. Esta es una ocasi贸n especial, los archivos han sido guardados o actualizados en el repositorio. Git nos pedira que dejemos un mensaje para recordar los cambios que hicimos y podemos usar el argumento -m para describirlo ( git commit -m "mensaje").

- `git rm`: este comando necesita algunos de los argumentos para poder ejecutarse correctamente:

- `git rm --cached`: Mueve los archivos que le indiquemos al estado Untracked.
- `git rm --force`: Elimina los archivos de Git y del disco duro. Git guarda el registro de la existencia de los archivos, por lo que podremos recuperarlos si es necesario (pero debemos usar comandos m谩s avanzados).

## Qu茅 es un Branch y c贸mo funciona un Merge?

En otras palabras, un branch o rama en Git es una rama que proviene de otra. Imagina un 谩rbol, que tiene una rama gruesa, y otra m谩s fina, en la rama m谩s gruesa tenemos los commits principales y en la rama fina tenemos otros commits que pueden ser de hotfix, devlopment entre otros.銋?
Estas son las ramas base de un proyecto en Git:

Est谩ndar de equipos de desarrollo..

- Rama ***Master*** o ***Main***: Por defecto, el proyecto se crea en una rama llamada Main (anteriormente conocida como Master). Cada vez que a帽ades c贸digo y guardas los cambios, est谩s haciendo un commit, que es a帽adir el nuevo c贸digo a una rama. Esto genera nuevas versiones de esta rama o branch, hasta llegar a la versi贸n actual de la rama Main.
- Rama ***Development***: Cuando decides hacer experimentos, puedes generar ramas experimentales (usualmente llamadas development), que est谩n basadas en alguna rama main, pero sobre las cuales puedes hacer cambios a tu gusto sin necesidad de afectar directamente al c贸digo principal.
- Rama ***Hotfix***: En otros casos, si encuentras un bug o error de c贸digo en la rama Main (que afecta al proyecto en producci贸n), tendr谩s que crear una nueva rama (que usualmente se llaman bug fixing o hot fix) para hacer los arreglos necesarios. Cuando los cambios est茅n listos, los tendr谩s que fusionar con la rama Main para que los cambios sean aplicados. Para esto, se usa un comando llamado Merge, que mezcla los cambios de la rama que originaste a la rama Main.

### C贸mo hacer merge

Producir una nueva rama se conoce como Checkout. Unir dos ramas lo conocemos como Merge.

Cuando haces merge de estas ramas con el c贸digo principal, su c贸digo se fusiona originando una nueva versi贸n de la rama master (o main) que ya tiene todos los cambios que aplicaste en tus experimentos o arreglos de errores.

Podemos generar todas las ramas y commits que queramos. De hecho, podemos aprovechar el registro de cambios de Git para producir ramas, traer versiones viejas del c贸digo, arreglarlas y combinarlas de nuevo para mejorar el proyecto.

Solo ten en cuenta que combinar estas ramas (hacer 鈥渕erge鈥?) puede generar conflictos. Algunos archivos pueden ser diferentes en ambas ramas. Git es muy inteligente y puede intentar unir estos cambios autom谩ticamente, pero no siempre funciona. En algunos casos, somos nosotros los que debemos resolver estos conflictos a mano.

## Analizar cambios en los archivos de tu proyecto con Git

El comando git show nos muestra los cambios que han existido sobre un archivo y es muy 煤til para detectar cu谩ndo se produjeron ciertos cambios, qu茅 se rompi贸 y c贸mo lo podemos solucionar. Pero podemos ser m谩s detallados.

Si queremos ver la diferencia entre una versi贸n y otra, no necesariamente todos los cambios desde la creaci贸n del archivo, podemos usar el comando git diff commitA commitB.

Recuerda que puedes obtener el ID de tus commits con el comando git log.

## Volver en el tiempo en nuestro repositorio utilizando reset y checkout

El comando `git checkout` + `ID del commit` nos permite viajar en el tiempo. Podemos volver a cualquier versi贸n anterior de un archivo espec铆fico o incluso del proyecto entero. Esta tambi茅n es la forma de crear ramas y movernos entre ellas.

Tambi茅n hay una forma de hacerlo un poco m谩s 鈥渞uda鈥?: usando el comando `git reset`. En este caso, no solo 鈥渧olvemos en el tiempo鈥?, sino que borramos los cambios que hicimos despu茅s de este commit.

Hay dos formas de usar `git reset`: con el argumento `--hard`, borrando toda la informaci贸n que tengamos en el 谩rea de staging (y perdiendo todo para siempre). O, un poco m谩s seguro, con el argumento `--soft`, que mantiene all铆 los archivos del 谩rea de staging para que podamos aplicar nuestros 煤ltimos cambios pero desde un commit anterior.

C贸mo usar Git Reset
Para volver a commits previos, borrando los cambios realizados desde ese commit, podemos utilizar:

- `git reset --soft [SHA 1]`: elimina los cambios hasta el staging area
- `git reset --mixed [SHA 1]`: elimina los cambios hasta el working area
- `git reset --hard [SHA 1]`: regresa hasta el commit del [SHA-1]
Donde el SHA-1 es el identificador del commit

## Git reset vs. Git rm

### git rm

Este comando nos ayuda a eliminar archivos de Git sin eliminar su historial del sistema de versiones. Esto quiere decir que si necesitamos recuperar el archivo solo debemos 鈥渧iajar en el tiempo鈥? y recuperar el 煤ltimo commit antes de borrar el archivo en cuesti贸n.

Recuerda que git rm no puede usarse as铆 nom谩s. Debemos usar uno de los flags para indicarle a Git c贸mo eliminar los archivos que ya no necesitamos en la 煤ltima versi贸n del proyecto:

- `git rm --cached`: Elimina los archivos de nuestro repositorio local y del 谩rea de staging, pero los mantiene en nuestro disco duro. B谩sicamente le dice a Git que deje de trackear el historial de cambios de estos archivos, por lo que pasaran a un estado untracked.
- `git rm --force`: Elimina los archivos de Git y del disco duro. Git siempre guarda todo, por lo que podemos acceder al registro de la existencia de los archivos, de modo que podremos recuperarlos si es necesario (pero debemos usar comandos m谩s avanzados).

### git reset

Este comando nos ayuda a volver en el tiempo. Pero no como git checkout que nos deja ir, mirar, pasear y volver. Con git reset volvemos al pasado sin la posibilidad de volver al futuro. Borramos la historia y la debemos sobreescribir. No hay vuelta atr谩s.

Este comando es muy peligroso y debemos emplearlo solo en caso de emergencia. Recuerda que debemos usar alguna de estas dos opciones:

Hay dos formas de utilizar git reset: con el argumento --hard, borrando toda la informaci贸n que tengamos en el 谩rea de staging (y perdiendo todo para siempre). O, un poco m谩s seguro, con el argumento --soft, que mantiene all铆 los archivos del 谩rea de staging para que podamos aplicar nuestros 煤ltimos cambios pero desde un commit anterior.

- `git reset --soft`: Borramos todo el historial y los registros de Git pero guardamos los cambios que tengamos en Staging, as铆 podemos aplicar las 煤ltimas actualizaciones a un nuevo commit.
- `git reset --hard`: Borra todo. Todo todito, absolutamente todo. Toda la informaci贸n de los commits y del 谩rea de staging se borra del historial.

隆Pero todav铆a falta algo!

- `git reset HEAD`: Este es el comando para sacar archivos del 谩rea de staging. No para borrarlos ni nada de eso, solo para que los 煤ltimos cambios de estos archivos no se env铆en al 煤ltimo commit, a menos que cambiemos de opini贸n y los incluyamos de nuevo en staging con git add, por supuesto.

## 驴Por qu茅 esto es importante?

### Imagina el siguiente caso:

Hacemos cambios en los archivos de un proyecto para una nueva actualizaci贸n. Todos los archivos con cambios se mueven al 谩rea de staging con el comando git add. Pero te das cuenta de que uno de esos archivos no est谩 listo todav铆a. Actualizaste el archivo, pero ese cambio no debe ir en el pr贸ximo commit por ahora.

### 驴Qu茅 podemos hacer?

Bueno, todos los cambios est谩n en el 谩rea de Staging, incluido el archivo con los cambios que no est谩n listos. Esto significa que debemos sacar ese archivo de Staging para poder hacer commit de todos los dem谩s.

隆Al usar git rm lo que haremos ser谩 eliminar este archivo completamente de git! Todav铆a tendremos el historial de cambios de este archivo, con la eliminaci贸n del archivo como su 煤ltima actualizaci贸n. Recuerda que en este caso no busc谩bamos eliminar un archivo, solo dejarlo como estaba y actualizarlo despu茅s, no en este commit.

En cambio, si usamos git reset HEAD, lo 煤nico que haremos ser谩 mover estos cambios de Staging a Unstaged. Seguiremos teniendo los 煤ltimos cambios del archivo, el repositorio mantendr谩 el archivo (no con sus 煤ltimos cambios, pero s铆 con los 煤ltimos en los que hicimos commit) y no habremos perdido nada.

Conclusi贸n: Lo mejor que puedes hacer para salvar tu puesto y evitar un incendio en tu trabajo es conocer muy bien la diferencia y los riesgos de todos los comandos de Git.

## Flujo de trabajo b谩sico con un repositorio remoto

Cuando empiezas a trabajar en un entorno local, el proyecto vive 煤nicamente en tu computadora. Esto significa que no hay forma de que otros miembros del equipo trabajen en 茅l.

Para solucionar esto, utilizamos los servidores remotos: un nuevo estado que deben seguir nuestros archivos para conectarse y trabajar con equipos de cualquier parte del mundo.

Estos servidores remotos pueden estar alojados en GitHub, GitLab, BitBucket, entre otros. Lo que van a hacer es guardar el mismo repositorio que tienes en tu computadora y darnos una URL con la que todos podremos acceder a los archivos del proyecto. As铆, el equipo podr谩 descargarlos, hacer cambios y volverlos a enviar al servidor remoto para que otras personas vean los cambios, comparen sus versiones y creen nuevas propuestas para el proyecto.

Esto significa que debes aprender algunos nuevos comandos

### Comandos para trabajo remoto con GIT

- `git clone url_del_servidor_remoto`: Nos permite descargar los archivos de la 煤ltima versi贸n de la rama principal y todo el historial de cambios en la carpeta .git.
- `git push`: Luego de hacer git add y git commit debemos ejecutar este comando para mandar los cambios al servidor remoto.
- `git fetch`: Lo usamos para traer actualizaciones del servidor remoto y guardarlas en nuestro repositorio local (en caso de que hayan, por supuesto).
- `git merge`: Tambi茅n usamos el comando git merge con servidores remotos. Lo necesitamos para combinar los 煤ltimos cambios del servidor remoto y nuestro directorio de trabajo.
- `git pull`: B谩sicamente, git fetch y git merge al mismo tiempo.

## Introducci贸n a las ramas o branches de Git

Las ramas son la forma de hacer cambios en nuestro proyecto sin afectar el flujo de trabajo de la rama principal. Esto porque queremos trabajar una parte muy espec铆fica de la aplicaci贸n o simplemente experimentar.

La cabecera o HEAD representan la rama y el commit de esa rama donde estamos trabajando. Por defecto, esta cabecera aparecer谩 en el 煤ltimo commit de nuestra rama principal. Pero podemos cambiarlo al crear una rama (`git branch rama`, `git checkout -b rama`) o movernos en el tiempo a cualquier otro commit de cualquier otra rama con los comandos (`git reset id-commit`, `git checkout rama-o-id-commit`).

### C贸mo funcionan las ramas en GIT

Las ramas son la manera de hacer cambios en nuestro proyecto sin afectar el flujo de trabajo de la rama principal. Esto porque queremos trabajar una parte muy espec铆fica de la aplicaci贸n o simplemente experimentar.

- `git branch -nombre de la rama-`: Con este comando se genera una nueva rama.
- `git checkout -nombre de la rama-`: Con este comando puedes saltar de una rama a otra.
- `git checkout -b rama`: Genera una rama y nos mueve a ella autom谩ticamente, Es decir, es la combinaci贸n de git brach y git checkout al mismo tiempo.
- `git reset id-commit`: Nos lleva a cualquier commit no importa la rama, ya que identificamos el id del tag., eliminando el historial de los commit posteriores al tag seleccionado.
- `git checkout rama-o-id-commit`: Nos lleva a cualquier commit sin borrar los commit posteriores al tag seleccionado.

## Fusi贸n de ramas con Git merge

El comando git merge nos permite crear un nuevo commit con la combinaci贸n de dos ramas o branches (la rama donde nos encontramos cuando ejecutamos el comando y la rama que indiquemos despu茅s del comando).

C贸mo usar Git merge
En este ejemplo, vamos a crear un nuevo commit en la rama master combinando los cambios de una rama llamada cabecera:

```shell
git checkout master
git merge cabecera
```

Otra opci贸n es crear un nuevo commit en la rama cabecera combinando los cambios de cualquier otra rama:

```shell
git checkout cabecera
git merge cualquier-otra-rama
```

Asombroso, 驴verdad? Es como si Git tuviera superpoderes para saber qu茅 cambios queremos conservar de una rama y qu茅 otros de la otra. El problema es que no siempre puede adivinar, sobre todo en algunos casos donde dos ramas tienen actualizaciones diferentes en ciertas l铆neas en los archivos. Esto lo conocemos como un conflicto.

Recuerda que al ejecutar el comando git checkout para cambiar de rama o commit puedes perder el trabajo que no hayas guardado. Guarda siempre tus cambios antes de hacer git checkout.

<br>
<br>

# GITHUB

Github es una plataforma que nos permite guardar repositorios de git que podemos usar como servidores remotos y ejecutar algunos comandos de forma visual e interactiva (sin necesidad de consola de mandos).

Luego de crear nuestra cuenta, podemos crear o importar repositorios, crear organizadores y proyectos de trabajo, descubrir respositorios de otras personas, contribuir a esos proyectos, dar estrellas y muchas otras cosas.

El Readme.md es el archivo que veremos por defecto al entrar en un repositorio. Es una muy buena pr谩ctica configurarlo para describir el proyecto, los requerimientos y las instrucciones que debemos seguir para contribuir correctamente.

Para clonar un repositorio desde GitHub (o cualquier otro servidor remoto) debemos copiar el URL (por ahora, usando HTTPS) y ejecutar el comando git clone + la URL que acabamos de copiar. Esto descargara la versi贸n de nuestro proyecto que se encuentra en GitHub.

Sin embargo, esto solo funciona para las personas que quieren empezar a contribuir en el proyecto. Si queremos conectar el repositorio de GitHub con nuestro repositorio local, el que creamos con git init, debemos ejecutar las siguientes instrucciones:

- **Primero:** Guardar la URL del repositorio de GitHub con el nombre de origin

```bash
git remote add origin <URL>
```

- **Segundo**: Verificar que la URL se haya guardado correctamente

```bash
git remote
git remote -v
```

- **Tercero**: Traer la versi贸n del repositorio remoto y hacer merge para crear un commit con los archivos de ambas partes. Podemos usar git fetch y git merge o solo git pull con el flag --allow-unrelated-histories:

```bash
git pull origin master--allow-unrelated-histories
```

- Por 煤ltimo, ahora s铆 podemos hacer git push para guardar los cambios de nuestro repositorio local en GitHub

```bash
git push origin master
```

## Comenzando

1. Para comenzar nos creamos una cuenta --- > <https://github.com> 馃殌

![GitHub-Register](_src/assets/00-PrimerosPasos/github_register.png)

2. Una vez registrados, ingresamos con usuario y contrase帽a:

![GitHub-Login](_src/assets/00-PrimerosPasos/github_login.png)

3. Listo! Ahora vemos una p谩gina de inicio como la siguiente:

![GitHub-Home](_src/assets/00-PrimerosPasos/github_home.png)

A la izquierda tenemos un acceso r谩pido a **mis repositorios**.

En el centro vemos la actividad de los usuarios a quienes seguimos.

En la parte superior derecha, vemos nuestra imagen de perfil. Desde ah铆 podemos desplegar opciones para gestionar nuestro perfil, repositorios y configuraci贸n. Si accedemos a nuestro perfil encontramos algo parecido a esto:

![GitHub-profile](_src/assets/00-PrimerosPasos/github_profile.png)

Podemos poner una foto de perfil, editar el nombre, agregar la ubicaci贸n, link y organizaciones a las que pertenecemos. En el centro podemos fijar los repositorios que queremos mostrar para que est茅n visibles en nuestro perfil.

M谩s abajo se muestra un diagrama de todas las contribuciones que vamos haciendo a los repositorios.

Si accedemos a la pesta帽a de arriba que dice `repositorios` veremos una lista de todos ellos. Cuando elegimos un repositorio para ver, nos lleva a una p谩gina como esta:

![GitHub-repo](_src/assets/00-PrimerosPasos/github_repo.png)

As铆 se ve un repositorio. Arriba a la izquierda tenemos el `nombre de usuario/nombre del repo`.

En el centro podemos ver todos los archivos que tiene dentro el repo. El bot贸n verde que dice `Code` es importante, si clickeamos ah铆 vamos a poder obtener la url del repo, para as铆 poder **_clonarlo_** (esto lo veremos m谩s adelante).

Arriba a la derecha encontramos tres botones. `Watch` nos permite seguir un repositorio, mientras que con `Star` podemos marcar como favorito un repo que nos guste. Por 煤ltimo tenemos `Fork`, este es **muy** importante, lo vamos a necesitar cuando hagamos el **_Challenge!_**

Ya tenemos todo para empezar... 脡xitos!!! 馃崁

### Manejo de ramas en GitHub

Puedes trabajar con ramas que nunca enviamos a GitHub, as铆 como pueden haber ramas importantes en GitHub que nunca usas en el repositorio local. Lo importante es que aprendas a manejarlas para trabajar profesionalmente.

- **Crear una rama en el repositorio local**:

```bash
git branch "nombre de la rama" 
o 
git checkout -b "nombre de la rama"
```

- **Publicar una rama local, al repositorio remoto**:

```bash
git push origin "nombre de la rama"
```

Recuerda que podemos ver gr谩ficamente nuestro entorno y flujo de trabajo local con Git usando el comando `gitk`.

#### Configurar m煤ltiples colaboradores en un repositorio de GitHub

Por defecto, cualquiera puede clonar o descargar tu proyecto desde GitHub, pero no pueden crear commits, ni ramas ni nada.

Existen varias formas de solucionar esto para poder aceptar contribuciones. Una de ellas es a帽adir a cada persona de nuestro equipo como colaborador de nuestro repositorio.

Solo debemos entrar a la configuraci贸n de colaboradores de nuestro proyecto (Repositorio > Settings > Collaborators) y a帽adir el email o username de los nuevos colaboradores.

#### Flujo de trabajo profesional con ***pull requests***

En un entorno profesional normalmente se bloquea la rama master, y para enviar c贸digo a dicha rama pasa por un code review y luego de su aprobaci贸n se unen c贸digos con los llamados merge request.

Para realizar pruebas enviamos el c贸digo a servidores que normalmente los llamamos Staging develop (servidores de pruebas) luego de que se realizan las pruebas pertinentes tanto de c贸digo como de la aplicaci贸n estos pasan a el servidor de producci贸n con el ya antes mencionado merge request.

#### Ignorar archivos en el Repositorio con ***.gitignore***

No todos los archivos que agregas a un proyecto deber铆an ir a un repositorio, por ejemplo cuando tienes un archivo donde est谩n tus contrase帽as que com煤nmente tienen la extensi贸n ***.env*** o cuando te estas conectando a una base de datos, son archivos que nadie debe ver.

#### Reconstruir commits en Git con ***amend***

A veces hacemos un commit, pero resulta que no quer铆amos mandarlo porque faltaba algo m谩s. Utilizamos `git commit --amend`, amend en ingl茅s es remendar y lo que har谩 es que los cambios que hicimos nos los agrega al commit anterior.

#### Git ***reset*** y ***reflog***: 煤sese en caso de emergencia

驴Qu茅 pasa cuando todo se rompe y no sabemos qu茅 est谩 pasando?

Con git reset hashDelHEAD nos devolvemos al estado en que el proyecto funcionaba.

- `git reset --soft <hashDelHEAD>` te mantiene lo que tengas en Staging ah铆.
- `git reset --hard <hashDelHEAD>` resetea absolutamente todo incluyendo lo que tengas en Staging.

Git reset es una mala pr谩ctica, no deber铆as usarlo en ning煤n momento; debe ser nuestro 煤ltimo recurso.

#### Buscar en archivos y commits de Git con ***grep*** y ***log***

A medida que nuestro proyecto se hace grande vamos a querer buscar ciertas cosas.

Por ejemplo: 驴Cu谩ntas veces en nuestro proyecto utilizamos la palabra color?

Para buscar utilizamos el comando git grep color y nos buscar谩 en todo el proyecto los archivos en donde est谩 la palabra color.

- **Con git grep -n color** nos saldr谩 un output el cual nos dir谩 en que l铆nea est谩 lo qu茅 estamos buscando.
- **Con git grep -c color** nos saldr谩 un output el cual nos dir谩 cuantas veces se repite esa palabra y en qu茅 archivo.

Si queremos buscar cu谩ntas veces utilizamos un atributo de HTML lo hacemos con **git grep -c "atributo"**.

## Lectura recomendada

- [Git: sitio oficial](https://git-scm.com/)
- [Git: documentaci贸n](https://git-scm.com/book/es/v2)
- [Github: sitio oficial](https://github.com/)

<br>
<br>

<table class="hide" width="100%" style='table-layout:fixed;'>
  <tr>
    <td>
      <img src="https://static.thenounproject.com/png/288029-200.png" width="50"/>
      <br>
      <a href="https://forms.gle/MY9PJuXbMnD17e548">
        Has click ac谩 para dejar tu feedback sobre esta clase.
      </a>
    </td>
  </tr>
</table>

---

#### Si tienes dudas sobre este tema, puedes consultarlas en el canal **_Preguntas_** de Discord