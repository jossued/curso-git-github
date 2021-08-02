## Comandos fundamentales
- git status -> Ve cambios y la rama
- git commit -m -> Hace un commit con un mensaje
- git add -A -> añade al stage todos los cambios
- git reset -> quita del stage los archivos
- git diff -> compara los cambios (para ver en el stage añadir --staged) (se pueden comparar tambien commits ids y ramas)
- git checkout -- .  -> restablece los cambios de los archivos

## Otros comandos
- git commit ammend -m "" -> corrige el nombre del commit
- git reset --soft HEAD^ -> se mueve a otro commit pero conserva los cambios, si se quiere se puede restablecer el HEAD a un commit específico se puede poniendo el id, así git reset --soft HEAD 1234
- git reset --hard -> se mueve a otro commit y no conserva los cambios
- git mv archivo archivo -> cambia el nombre del archivo
- git rm archivo -> borra el archivo
- git add -u -> actualiza archivos borrados o renombrados
- .gitignore -> archivo en donde se especifica lo que se va a ignorar del seguimiento de archivos y carpetas

## Ramas
- git branch nombre -> crea una rama en el HEAD, git branch -> lista las ramas, git checkout nombre -> se mueve a la rama (con el comando -b también la crea).
- git merge nombre -> une la rama del nombre con la rama actual
- git branch -d nombre -> borra la rama

## Etiquetas
- git tag -> lista etiquetas (versiones)
- git tag -d nombre -> borra el tag
- git tag -a v1.0.0 (commitId) -m "Versión 1.0.0" ->  realiza un tag más específico
- git show nombreTag -> muestra información del commit del tag

## Stash y Rebase
- git stash -> crea un WIP de los cambios actuales
- git stash pop -> trae los cambios del stash y elimina el sstash de la lista
- git stash list -> lista los stash
- git show stash -> muestra el último stash a detalle
- git stash drop -> borra el stash de la posición 0
- git stash clear -> borra todos los stash
- git stash apply stash@{1} -> aplica los cambios del stash id
- --keep-index -> guarda tdo menos los del stage