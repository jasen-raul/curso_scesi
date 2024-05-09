# PRIMEROS PASOS PARA EL MUNDO DE GIT
## Que es git?
git es un software de control de versiones de codigo abierto.
## Que es un control de versiones?
Es un sistem que registra cada cambio que se realiza en el codigo fuente de un proyecto.<br>
***-sistema de control de versiones centralizado:***<br>
Hay un repositorio centralizado al que los desarrolladores se conectan para colaborar.<br>
***-sistema de control de versiones distribuido:***<br>
Cada desarrollador tiene su propido repositorio completo y puede trabajarlo de forma independinte.
## Que es un repositorio?
Un repositorio es una carpeta en le que se almacenan las diferentes versiones de los ficheros de un proyecto y el historico de los cambios que se han realizado en ellos.
# Comandos
#### Muestra la version de git instalada
```
git --version 
```
#### muestra los comados basicos de uso
```
git --help
```
#### Configuracion de usuario y correo
```
git config --global user.name <usuario>
```
```
git config --global user.email <tu_correo>
```
#### Muestra la configuracion global que tienes
```
git config --global --list
```
#### Iniciar un nuevo repositorio en la carpeta actual
```
git init 
```
#### Lista el estado de nuestros archivos
```
git status
```
#### Agrega todos los archivos pendientes desde la carpeta actual
```
git add .
```
#### Agrega solo el archivo indicado
```
git add tu_archivo
```
#### Guarda en el repositorio local todos los archivos agregados
```
git commit -m "<tu_descripcion>"
```
#### Abre un editor y permite modificar el último commit (Reemplaza el último commit)
```
git commit --amend
```
#### lista tag
```
git tag
```
#### borra un tag en especifico
```
git tag -d <tag>
```
#### Deshace el ultimo commit, elimina los cambios en el area de preparacion
```
git reset
```
#### muestra los commits realizados sin muchos detalles
```
git log --oneline
```
#### Muestra los commits de forma grafica
```
git log --graph --oneline
```
#### Crea una nueva rama
```
git branch <nombre_rama>
```
#### Crear una nueva rama y cambia a ella en una sola operación
```
git checkout -b nombre_rama
```
#### Cambiar a otra rama
```
git checkout nombre_rama
```
```
git switch nombre_rama
```
#### Muestra en que rama estamos y lista las demas
```
git branch
```
#### Renombrar la rama actual
```
git branch -m <rama>
```
#### Permite juntar dos ramas. Trae los cambios de la rama especificada a la rama actual
```
git merge <rama>
```
#### Permite juntar dos ramas, pero las mantiene. Genera un commit del merge en la rama actual
```
git merge --no-ff <rama>
```
#### Cancelar una fusión en curso y volver al estado anterior al inicio de la fusión.
```
git merge --abort
```
#### Eliminar una rama (solo si ya combinaste la rama)
```
git branch -d nombre_rama
```
#### Forzar la eliminacion de una rama 
```
git branch -D nombre_rama  
```
#### Listar todas las ramas incluyendo las del repositorio remoto
```
git branch -a
```
## Comandos para Repositorio remoto
#### Vincular repositorio remoto con repositorio local
```
git remote add origin <url>
```
#### Cambiar url del repositorio remoto
```
git remote set-url origin <url>
```
#### Muestra en que repositorio estamos enlazados remotamente
```
git remote -v 
```
#### Sube los cambios del repositorio local al remoto de una rama específica
```
git push origin <rama>
```
#### Sube los cambios del repositorio local al remoto y especifica la rama principal
```
git push -u origin <rama>
```
