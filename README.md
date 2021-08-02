## Comandos fundamentales
- git status -> Ve cambios y la rama
- git commit -m -> Hace un commit con un mensaje
- git add -A -> añade al stage todos los cambios
- git reset -> quita del stage los archivos
- git diff -> compara los cambios (para ver en el stage añadir --staged)
- git checkout -- .  -> restablece los cambios de los archivos

## Otros comandos
- git commit ammend -m "" -> corrige el nombre del commit
- git reset --soft HEAD^ -> se mueve a otro commit pero conserva los cambios, si se quiere se puede restablecer el HEAD a un commit específico se puede poniendo el id, así git reset --soft HEAD 1234
- git reset --hard -> se mueve a otro commit y no conserva los cambios
