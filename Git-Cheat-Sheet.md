# Git sheatsheet

## INDICE

1. Instalacion de Git
2. Configuracion
3. Inicializar Repositorio
4. Revisar el estado de cambios
5. Como crear commits
6. Como subir respositorios a las nube
7. Como trabajar con ramas



## Instalacion de Git
 
 En el día a día del trabajo con Git una de las cosas útiles que podemos hacer es trabajar con ramas. Las ramas son caminos que puede tomar el desarrollo de un software, algo que ocurre naturalmente para resolver problemas o crear nuevas funcionalidades. En la práctica permiten que nuestro proyecto pueda tener diversos estados y que los desarrolladores sean capaces de pasar de uno a otro de una manera ágil.

 GitHub for Windows
htps://windows.github.com

GitHub for Mac
htps://mac.github.com
For Linux and Solaris platforms, the latest release is available on
the official Git web site.
Git for All Platforms


## configuracion

Si quieres comprobar tu configuración, puedes usar el comando 
`git config --list` para mostrar todas las propiedades que Git ha configurado: `$ git config --list user.name=John Doe user.`

`git init`

Utilizar git init para inicializar un repositorio vacio

`git clone [url]`

Utilizar git clone para copiar un repositorio existente


## inicializar respositocio
Inicio de un nuevo repositorio: git init
Para crear un nuevo repositorio, usa el comando git init . git init es un comando que se utiliza una sola vez durante la configuración inicial de un repositorio nuevo. Al ejecutar este comando, se creará un nuevo subdirectorio . git en tu directorio de trabajo actual.
 
 1- git config --global user.name “[firstname lastname]”

 2-git config --global user.email “[valid-email]”

 3-git config --global color.ui auto

 ## Revisar el estado de cambios

 Se suele utilizar después de ver los cambios que ha habido en los archivos con el comando status. Puedes emplear git diff [archivo] para precisar la muestra. El comando git diff --cached mostrará el contenido que se ha añadido al área de ensayo, es decir, los cambios que se incluirán en el historial si se hace commit.


## Como hacer los commit

 1-Usa el verbo imperativo ( Add , Change , Fix , Remove , …).

2-No uses punto final ni puntos suspensivos en tus mensajes. 

3-Usa como máximo 50 carácteres para tu mensaje de commit.

4-Añade todo el contexto que sea necesario en el cuerpo del mensaje de commit.

5- Usa un prefijo para tus commits para hacerlos más semánticos

6-Considera usar utilidades para hacer commit

## Como subir el respositorio a las nubes

Crear Repositorio Remoto de Git
Podemos añadir todos los ficheros al repositorio local con los siguientes comandos: git add . De esta manera, cada vez que hagamos push para subir los cambios al repositorio remoto de git, los ficheros se sincronizarán automáticamente en la nube.

1-git init

2-git add .

3-git commit -m "first commit"

4-git remote add origin https://github.com/NOMBRE_USUARIO/NOMBRE_PROYECTO.git

5-git push -u origin master


## Como trabajar con ramas

En el día a día del trabajo con Git una de las cosas útiles que podemos hacer es trabajar con ramas. Las ramas son caminos que puede tomar el desarrollo de un software, algo que ocurre naturalmente para resolver problemas o crear nuevas funcionalidades. En la práctica permiten que nuestro proyecto pueda tener diversos estados y que los desarrolladores sean capaces de pasar de uno a otro de una manera ágil.

Nuevas ramas

El comando git branch permite crear una rama nueva. Si quieres empezar a trabajar en una nueva función, puedes crear una rama nueva a partir de la rama main con git branch new_branch . Una vez creada, puedes usar git checkout new_branch para cambiar a esa rama.