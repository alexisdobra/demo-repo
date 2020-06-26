# GIT

## clone

### Clona en el directorio local donde nos encontramos situados, una copia del repositorio indicado por URL o SSH key

\$ git clone HTTP/SSH

## init

### Se indica que el directorio local debe agregar un .git ya que se agregará a un repositorio

\$ git init

## add

### Registra cambios y agrega nuevos documentos al repositorio, se puede especificar los archivos o indicar que se realizará para todos los archivos nuevos o con cambios pendientes de registro

\$ git add <filename>
\$ git add .

## commit

### Commitea los cambios, una vez realizado los archivos con cambios o nuevos serán agregados al HEAD, pero aun permanecerán en el repositorio local. (-m) se utiliza para agregar título y descripción, en caso de ir una sola referencia a la descripción

\$git commit -m "Title" -m "Description"

## push

### Tus cambios están ahora en el HEAD de tu copia local. Para enviar estos cambios a tu repositorio remoto ejecuta push, reemplaza master por la rama a la que quieres enviar tus cambios.

\$git push origin master

## add remote

### Si no has clonado un repositorio ya existente y quieres conectar tu repositorio local a un repositorio remoto, luego podrás subir tus cambios al repositorio remoto seleccionado.

\$git remote add origin <server>

## Branches

### Las ramas son utilizadas para desarrollar funcionalidades aisladas unas de otras. La rama master es la rama "por defecto" cuando creas un repositorio. Crea nuevas ramas durante el desarrollo y fusiónalas a la rama principal cuando termines.

### Crear una nueva rama nueva y cambiar a ella

\$git checkout -b <branch>

### Cambiar a una rama deseada

\$git checkout <branch>

### Borrar rama

\$git branch -d <branch>

### Una rama nueva no estará disponible para los demás a menos que subas (push) la rama a tu repositorio remoto

\$git push origin <branch>

## pull

### Para actualizar tu repositorio local al commit más nuevo, se debe ejecutar pull en el directorio de trabajo para bajar y fusionar los cambios remotos

\$git pull

## merge

### Se utiliza para fusionar otra rama a tu rama activa, git intentará fusionar automáticamente los cambios

\$git merge <branch>

### Desafortunadamente, no siempre será posible y se podrán producir conflictos. Tú eres responsable de fusionar esos conflictos manualmente al editar los archivos mostrados por git. Después de modificarlos, necesitas marcarlos como fusionados con

\$git add <filename>

### Antes de fusionar los cambios, puedes revisarlos usando

\$git diff <source_branch> <target_branch>

## status

### Ver el status de git

\$git status

## Unstage files using git reset

### The easiest way to unstage files on Git is to use the “git reset” command and specify the file you want to unstage.

\$git reset <commit> -- <path>

### By default, the commit parameter is optional : if you don’t specify it, it will be referring to HEAD.

### This command will reset the index entries (the ones you added to your staging area) to their state at the specified commit (or HEAD if you didn’t specify any commits).

## Unstage all files on Git

### To unstage all files, use the “git reset” command without specifying any files or paths.

\$ git reset

## Remove unstaged changes on Git

### In some cases, after unstaging files from your staging area, you may want to remove them completely.

### In order to remove unstaged changes, use the “git checkout” command and specify the paths to be removed.

\$ git checkout -- <path>

### Alternatively, if you want to discard your entire working directory, head back to the root of your project and execute the following command.

\$ git checkout -- .

## Unstage commit on Git

### In some cases, you actually committed files to your git directory (or repository) but you want to unstage them in order to make some modifications to your commit.

## Unstage commits softly

### To unstage commits on Git, use the “git reset” command with the “–soft” option and specify the commit hash.

\$ git reset --soft <commit>

### Alternatively, if you want to unstage your last commit, you can the “HEAD” notation in order to revert it easily.

\$ git reset --soft HEAD~1

### Using the “–soft” argument, changes are kept in your working directory and index.

### As a consequence, your modifications are kept, they are just not in the Git repository anymore.

## Unstage commits hardly

### To unstage commits on Git and discard all changes, use the “git reset” command with the “–hard” argument.

\$ git reset --hard <commit>

### Note : be careful when using the reset hard command, you will lose all your changes when hard resetting.
