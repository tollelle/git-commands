# git-commands
Chuleta Comandos de GIT

- https://git-scm.com/book/es/v1/Empezando-Configurando-Git-por-primera-vez
- https://gitignore.io

### Iniciar:

`git init`

Añadir repositiorio remoto: (origin es el nombre por defecto)

`git remote add origin https://github.com/tollelle/repositorio.git`

Listar repositorio remoto:

`git remote -v`

Modificar repositorio remoto

`git remote set-url origin https://github.com/tollelle/nuevoRepositorio.git`

Definiendo identidad:

`git config --global user.name "John Doe"`

`git config --global user.email johndoe@example.com`

* Sin --global compruebas el valor

Escuchando cambios de todo

`git add .` 

Escuchando cambios de archivo

`git add README`

Confirmar cambios y Commit inicial

`git commit –m 'versión inicial del proyecto'`


Clonado repositorio en carpeta actual con directorio grit

`git clone git://github.com/schacon/grit.git`

Clonando repositorio y rama específica

`git clone -b RAMA it://github.com/schacon/grit.git`


Clonando repositorio en carpeta definida

`git clone git://github.com/schacon/grit.git carpeta`


Comprobar estado de archivos

`git status`


Ver lo que has modificado pero aún no has preparado

`git diff`


Rehaciendo última confirmación

`git commit --amend`


Mostrando repositorios remotos definidos:

`git remote`


Recibiendo repositorio remoto y estados:

`git fetch [remote-name]`


Enviando cambios a repositorio remoto

`git push origin master`


Inspeccionando repositorio remoto

`git remote show origin`


Eliminando y renombrando repositorios remotos

`git remote rename NOMBREVIEJO NOMBRENUEVO`


Borrar repositorio remoto de la lista

`git remote rm origin`


Creando nueva rama

`git branch testing`


Cambiar a nueva rama
`git checkout testing`

Creando rama y cambiando a la nueva rama
`git checkout -b 'nuevaRAMA'`

Fusionar a master con merge
`git checkout master`
`git merge nuevaRAMA`

Borrar rama local nueva tras ser fusionada
`git branch -d nuevaRAMA`

Borrar rama local nueva SIN ser fusionada
`git branch -D nuevaRAMA`

Borrar rama remota
`git push origin :rama`

Mostrar listado de ramas del repositorio
`git branch`

Publicando desde rama actual
`git push (remoto) (rama)`
`git push origin master`

Reorganizar rama sobre master sin comprobar previamente
`git rebase master rama`



