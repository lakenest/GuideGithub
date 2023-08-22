Curso Git
nndevs@DESKTOP-ROAL6TG MINGW64 ~
$ git --version
git version 2.39.1.windows.1

nndevs@DESKTOP-ROAL6TG MINGW64 ~
$ git config --global user-name "Nestor Nieri"
error: key does not contain a section: user-name

nndevs@DESKTOP-ROAL6TG MINGW64 ~
$ git config --global user.name "Nestor Nieri"

nndevs@DESKTOP-ROAL6TG MINGW64 ~
$ git config --global user.email nraulnieri@gmail.com

nndevs@DESKTOP-ROAL6TG MINGW64 ~
$ git config --global core.editor "code --wait"

nndevs@DESKTOP-ROAL6TG MINGW64 ~
$ git config --global -e

nndevs@DESKTOP-ROAL6TG MINGW64 ~
$ git config--global core.autocrlf true
git: 'config--global' is not a git command. See 'git --help'.

nndevs@DESKTOP-ROAL6TG MINGW64 ~
$ git config --global core.autocrlf true


computer	stage	commit	server
computer
git add . | pasar a stage

stage
etapa intermedia
git commit -m "msj" | pasar a commit, se borra de stage


commit
repositorios locales
git push | pasar a repositorio en la nube


server

nndevs@DESKTOP-ROAL6TG MINGW64 /c/Users/Public/Documents/lakenest/cursoholamundo/miweb (master)
$ code .

nndevs@DESKTOP-ROAL6TG MINGW64 /c/Users/Public/Documents/lakenest/cursoholamundo/miweb (master)
$ git status /*añade archivo al seguimiento de git, etapa stage.


nndevs@DESKTOP-ROAL6TG MINGW64 /c/Users/Public/Documents/lakenest/cursoholamundo/miweb (master)
$ git add styles.css /*añade archivos al stage.

nndevs@DESKTOP-ROAL6TG MINGW64 /c/Users/Public/Documents/lakenest/cursoholamundo/miweb (master)
$ git commit -m "Commit inicial" /*cambios en el commit o comprometidos

nndevs@DESKTOP-ROAL6TG MINGW64 /c/Users/Public/Documents/lakenest/cursoholamundo/miweb (master)
$ rm styles.css /*eliminar o remover archivos

nndevs@DESKTOP-ROAL6TG MINGW64 /c/Users/Public/Documents/lakenest/cursoholamundo/miweb (master)
$ git restore index.html /*restaurar archivos eliminados mientras estas en el stage

nndevs@DESKTOP-ROAL6TG MINGW64 /c/Users/Public/Documents/lakenest/cursoholamundo/miweb (master)
$ mv index.html page.html /*renombrar archivo

nndevs@DESKTOP-ROAL6TG MINGW64 /c/Users/Public/Documents/lakenest/cursoholamundo/miweb (master)
$ git add index.html page.html /*añadir cuando se modificar el nombre

nndevs@DESKTOP-ROAL6TG MINGW64 /c/Users/Public/Documents/lakenest/cursoholamundo/miweb (master)
$ git add .gitignore

nndevs@DESKTOP-ROAL6TG MINGW64 /c/Users/Public/Documents/lakenest/cursoholamundo/miweb (master)
$ git commit -m "agregando archivo ignore" /*enumerar archivos que no van a ser subidos a git

nndevs@DESKTOP-ROAL6TG MINGW64 /c/Users/Public/Documents/lakenest/cursoholamundo/miweb (master)
$ git status -s  	/*similar a status muestra mas resumido
 M .gitignore
 M index.html
?? styles.css

nndevs@DESKTOP-ROAL6TG MINGW64 /c/Users/Public/Documents/lakenest/cursoholamundo/miweb (master)		/*ver cambios entre estado a y b
$ git diff

nndevs@DESKTOP-ROAL6TG MINGW64 /c/Users/Public/Documents/lakenest/cursoholamundo/miweb (master)		/*ver cambios entre a y b en stage
$ git diff --staged

nndevs@DESKTOP-ROAL6TG MINGW64 /c/Users/Public/Documents/lakenest/cursoholamundo/miweb (master)
$ git log --oneline			/*ver listado de commit realizados
0f4e94b (HEAD -> master) mostrando status corto 
f91682d agregando archivo ignore
1fefa46 devolviendo el nombre a pagina de inicio
9f20dd8 renombrando pagina de inicio
f4ebf2c eliminando hoja de estilos
3f06867 Agregando estilo para h1 y h2
f1d80a1 Commit inicial

nndevs@DESKTOP-ROAL6TG MINGW64 /c/Users/Public/Documents/lakenest/cursoholamundo/miweb (master) 
$ git branch	/*ver las ramas creadas y en donde nos ubicamos

nndevs@DESKTOP-ROAL6TG MINGW64 /c/Users/Public/Documents/lakenest/cursoholamundo/miweb (master)
$ git checkout -b ramab		/*crear una nueva rama, te mueves ahi por defecto. 

nndevs@DESKTOP-ROAL6TG MINGW64 /c/Users/Public/Documents/lakenest/cursoholamundo/miweb (ramab)	
$ git checkout master		/*moverse a otra rama

nndevs@DESKTOP-ROAL6TG MINGW64 /c/Users/Public/Documents/lakenest/cursoholamundo/miweb (master)
$ cat styles.css		/*ver contenido de un archivo

nndevs@DESKTOP-ROAL6TG MINGW64 /c/Users/Public/Documents/lakenest/cursoholamundo/miweb (master)
$ git merge ramab		/* unir rama secundaria a la rama principal.


nndevs@DESKTOP-ROAL6TG MINGW64 /c/Users/Public/Documents/lakenest/cursoholamundo/miweb (master)
$ git remote add origin https://github.com/lakenest/ob-curso-git.git

/*indicar a git que vamos a añadir un repositorio en la nube

nndevs@DESKTOP-ROAL6TG MINGW64 /c/Users/Public/Documents/lakenest/cursoholamundo/miweb (master)
$ git push -u origin master

/*subir el repositorio del equipo a la nube creando una rama master en origin || para subir a otra rama debes posicionarte ahi.




