### Sincronicacion

- incronizar los cambios del código con GitHub y Visual Studio

Una vez que instalaste los paquetes nuget puedes sincronizar tus cambios con el servidor de GitHub para que esté disponible para los demás.

En visual studio se agrega una palomita de color rojo al lado del archivo para indicar cuales archivos han sido cambiados y aún no han sido sincronizados con el servidor.

### Sincronizar  desde Visual Studio

1. Dar clic derecho sobre el proyecto. Luego en la opción Control de Código Fuente -> Confirmar

![git](../images/image.png)

2. Al lado derecho te muestra una ventana en la cual puedes escribir la descripción del cambio, y te muestra los archivos que han cambiado. Tecleamos como descripción: Instalación de paquetes Nuget desde Visual Studio Comunity luego damos clic en Confirmar Todo 

![git](../images/image1.png)

3. De esta forma los cambios están solamente en tu computadora. Para publicarlos en github da clic en Sincronizar


4. Damos clic en Insertar

![git](../images/image3.png)


---

### Visual Studio Code

1. Cree un directorio donde se guardarán los repositorios

![git](../images/vsc-repos-clonar-01.png)

)

2. Abra el directorio en Visual Studio Code (menú Archivo > Abrir carpeta ...):

![git](../images/vsc-repos-clonar-02.png)

3. Para clonar el repositorio necesitará dos rutas (el origen y el destino):

- La URL de repositorio, que se puede copiar desde el propio repositorio haciendo clic en el botón "Clone or download".

- Esta URL es la misma URL que aparece en el navegador pero terminada en .git.

- En la captura de ejemplo, la URL de origen es https://github.com/NumaNigerio/test-01.git

![git](../images/vsc-repos-clonar-03.png)

La ruta del directorio de destino, es decir, la ruta de la carpeta en la que se va a crear la carpeta que contendrá la copia del repositorio. Esta ruta se puede copiar del Explorador de Windows.

En la captura de ejemplo, el directorio de destino es C:\Users\Barto\Documents\LMSGI\Barto\Repositorios

![git](../images/vsc-repos-clonar-04.png)


4. En Visual Studio abra la ventana de comandos con Ctrl+May+p

![git](../images/vsc-repos-clonar-05.png)

5. Escriba el comando git:clone y pulse Intro:

![git](../images/vsc-repos-clonar-06.png)

6.Escriba la URL del repositorio de origen y pulse Intro:

![git](../images/vsc-repos-clonar-07.png)

7. Escriba la ruta del directorio que contendrá la copia y pulse Intro:

![git](../images/vsc-repos-clonar-08.png)

8. En unos segundos se mostrará la carpeta del repositorio clonado en la barra del explorador y se ofrecerá la posibilidad de abrir la carpeta del repositorio clonado. Haga clic en "Abrir repositorio"

![git](../images/vsc-repos-clonar-09.png)

9. Visual Studio Code abrirá la carpeta del repositorio clonado, mostrando su contenido (en el ejemplo, el repositorio contiene únicamente el fichero README.md.

![git](../images/vsc-repos-clonar-10.png)


### Realizar commits en el repositorio remoto

En git, un commit es un conjunto de cambios que se realizan en los ficheros del repositorio.

En Visual Studio Code podemos realizar commits, que se guardan en el repositorio local. Para sincronizar nuestros cambios en el repositorio, debemos identificarnos como usuario del repositorio.

El proceso en Visual Studio Code sería el siguiente:

Abra una ventana de Terminal e indique a git la dirección de correo del usuario (la dirección de correo vinculada a su cuenta en GitHub):

```powershell
git config --global user.email SU-CORREO-ELECTRONICO
```

![git](../images/vsc-repos-commit-01.png)


- Modifique los archivos del repositorio o añada nuevos archivos

En la captura del ejemplo, en el icono Control de código fuente se nos indica el número de ficheros con cambios (3). En la barra del Explorador se indica qué ficheros son nuevos (con la letra U) o se han modificado (con la letra M).

![git](../images/vsc-repos-commit-02.png)

- Abra la barra lateral de Control de código fuente haciendo clic en el icono correspondiente. Se mostrará la lista de ficheros con cambios:

![git](../images/vsc-repos-commit-03.png)

- Seleccione los ficheros cuyos cambios formarán parte del commit (puede elegir todos los ficheros modificados o sólo una parte) haciendo clic en el icono +:

![git](../images/vsc-repos-commit-04.png)

- Los ficheros seleccionados se muestran en un apartado "Cambios almacenados provisionalmente". Escriba el mensaje descriptivo del commit en la caja superior y pulse Ctrl+Intro

![git](../images/vsc-repos-commit-05.png)

- Los ficheros incluidos en el commit dejan de mostrarse en la parte superior y en el contador del icono Control de código fuente:

![git](../images/vsc-repos-commit-06-a.png)

- En la barra inferior, Visual Studio Code nos avisa que el repositorio local ya no está sincronizado con el repositorio remoto y nos indica el número de commits de diferencia:

![git](../images/vsc-repos-commit-06-b.png)

- Podemos hacer nuevos commits hasta que no queden cambios pendientes.

![git](../images/vsc-repos-commit-07-a.png)

- Haga clic en el icono de la barra lateral inferior para sincronizar el repositorio remoto con el local

![git](../images/vsc-repos-commit-08.png)

- Visual Studio Code mostrará un aviso indicando que al sincronizar se producirán cambios en el repositorio remoto. Para no volver a ver este aviso, haga clic en "De acuerdo, no volver a ver este mensaje":

![git](../images/vsc-repos-commit-09.png)

- La primera vez que sincronicemos, deberemos introducir el usuario y contraseña de GitHub.

![git](../images/vsc-repos-commit-10.png)

- Una vez realizada la sincronización, el contador deja de mostrarse.

![git](../images/vsc-repos-commit-11.png)


### Borrar credencial de Windows 

La identificación en GitHub que utiliza Visual Studio Code se guarda como credencial de Windows, por lo que si estamos utilizando un ordenador al que tienen acceso otras personas, es muy importante que eliminemos la credencial antes de abandonar el ordenador o nos arriesgamos a que otro usuario nos suplante y acceda a los repositorios remotos

- Abra el panel de control clásico (Menú de inicio > panel de control)

![git](../images/vsc-repos-credencial-1.png)


- Haga clic en el icono de Cuentas de usuario

![git](../images/vsc-repos-credencial-2.png)

- Haga clic en el enlace "Administrar credenciales"

![git](../images/vsc-repos-credencial-3.png)

Haga clic en el icono "Credenciales de Windows"

![git](../images/vsc-repos-credencial-4.png)

- Haga clic en la credencial genérica de github

![git](../images/vsc-repos-credencial-5.png)

- Haga clic en el enlace "Quitar"

![git](../images/vsc-repos-credencial-7.png)

- Confirme la eliminación

Compruebe que la credencial ha sido eliminada

![git](../images/vsc-repos-credencial-8.png)
