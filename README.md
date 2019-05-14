# Chuleta de Comandos de GIT

- https://git-scm.com/book/es/v1/Empezando-Configurando-Git-por-primera-vez
- Autogenerador .gitignore: https://gitignore.io

## Iniciar

    git init

<strong>Añadir</strong> repositiorio remoto: (origin es el nombre por defecto)

    git remote add origin https://github.com/tollelle/repositorio.git

<strong>Listar</strong> repositorio remoto:

    git remote -v

<strong>Modificar</strong> repositorio remoto

    git remote set-url origin https://github.com/tollelle/nuevoRepositorio.git

Definiendo <strong>identidad</strong> global:

    git config --global user.name "Jorge"
    
    git config --global user.email "correo@correo.com"

    git config --global github.user usergithub
    
Definiendo <strong>identidad en repositorio específico</strong>:

    git config user.name "Jorge"
    
    git config user.email "correo@correo.com"

    git config github.user usergithub
    
Forzar introducir <strong>usuario y contraseña</strong>:
Útil para cambiar de usuario

    git config --local credential.helper ""

## Monitorizar

<strong>Escuchando</strong> cambios de todo

    git add . 

<strong>Escuchando</strong> cambios de archivo

    git add README

<strong>Confirmar</strong> cambios y <strong>Commit</strong> inicial

    git commit –m 'versión inicial del proyecto'

## Clonar

<strong>Clonado</strong> repositorio en carpeta actual con directorio grit

    git clone git://github.com/schacon/grit.git

<strong>Clonando</strong> repositorio y rama específica

    git clone -b RAMA it://github.com/schacon/grit.git

<strong>Clonando</strong> repositorio en carpeta definida

    git clone git://github.com/schacon/grit.git carpeta


## Info

<strong>Comprobar</strong> estado de archivos

    git status

Ver lo que has <strong>modificado</strong> pero aún no has preparado

    git diff

<strong>Rehaciendo</strong> última confirmación

    git commit --amend

## Repositorios 

<strong>Mostrando</strong> repositorios remotos definidos:

    git remote

<strong>Recibiendo</strong> repositorio remoto y estados:

    git fetch [remote-name]

<strong>Enviando</strong> cambios a repositorio remoto

    git push origin master

<strong>Inspeccionando</strong> repositorio remoto

    git remote show origin

<strong>Eliminando y renombrando</strong> repositorios remotos

    git remote rename NOMBREVIEJO NOMBRENUEVO

<strong>Borrar</strong> repositorio remoto de la lista

    git remote rm origin

## Ramas

<strong>Creando</strong> nueva rama

    git branch testing


<strong>Cambiar</strong> a nueva rama

    git checkout testing


<strong>Creando</strong> rama y cambiando a la nueva rama

    git checkout -b 'nuevaRAMA'

<strong>Fusionar</strong> ramas a master con merge

    git checkout master

    git merge nuevaRAMA


<strong>Borrar</strong> rama local nueva tras ser fusionada

    git branch -d nuevaRAMA

<strong>Borrar</strong> rama local nueva SIN ser fusionada

    git branch -D nuevaRAMA


<strong>Borrar</strong> rama remota

    git push origin :rama


Mostrar <strong>listado</strong> de ramas del repositorio

    git branch


<strong>Publicando</strong> desde rama actual

    git push (remoto) (rama)

    git push origin master


<strong>Reorganizar</strong> rama sobre master sin comprobar previamente

    git rebase master rama

<strong>Deshacer</strong> cambios locales y commits y sincronizar con repositorio remoto
    
    git fetch origin
    
    git reset --hard origin/master


