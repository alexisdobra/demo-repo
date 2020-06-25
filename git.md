# GIT

## clone

S

### Clona en el directorio local donde nos encontramos situados, una copia del repositorio indicado por URL o SSH key

\$ git clone HTTP/SSH

## init

### Se indica que el directorio local debe agregar un .git ya que se agregará a un repositorio

\$ git init

## add

### Registra cambios y agrega nuevos documentos al repositorio, se puede especificar los archivos o indicar que se realizará para todos los archivos nuevos o con cambios pendientes de registro

\$ git add <filename>
\$ git add .

##commit

### Commitea los cambios, una vez realizado los archivos con cambios o nuevos serán agregados al HEAD, pero aun permanecerán en el repositorio local. (-m) se utiliza para agregar título y descripción, en caso de ir una sola referencia a la descripción

\$git commit -m "Title" -m "Description"
