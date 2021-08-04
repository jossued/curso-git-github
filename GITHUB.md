## Comandos remoto
- git remote add origin https... -> añade un nuevo repositorio remoto a nuestro repositorio
- git remote -v -> lista los remotos de nuestro repositorio
- git push -u origin master -> envía los commits al remoto, -u establece la rama por defecto, origin es el nombre del remoto y master la rama
- git remote add upstream -> añade otro remoto que sirve para actualizar mi fork, por convención se llama upstream
- git branch -a -> lista todas las ramas incluidas las remotas
- git push origin :rama -> borra la rama de origin
- git remote prune origin -> limpia las referencias locales de ramas que se han eliminado en el remoto.