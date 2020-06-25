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

###
