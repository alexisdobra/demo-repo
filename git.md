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

## branches

### Las ramas son utilizadas para desarrollar funcionalidades aisladas unas de otras. La rama master es la rama "por defecto" cuando creas un repositorio. Crea nuevas ramas durante el desarrollo y fusiónalas a la rama principal cuando termines.

### Crea una nueva rama nueva y cámbiate a ella

\$git checkout -b <name>

### Muévete a una rama deseada

\$git checkout <name>

### Borra la rama

\$git branch -d <name>

### Una rama nueva no estará disponible para los demás a menos que subas (push) la rama a tu repositorio remoto

\$git push origin <branch>
