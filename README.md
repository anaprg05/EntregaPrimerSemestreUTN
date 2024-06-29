# EntregaPrimerSemestreUTN
# CLASE 1
## CREACIÓN DE CARPETAS
### cd ..
### cd ..
### cd /mnt/c
### cd ~ -> Vamos a la raíz
### mkdir Tecnicatura -> Recordar que en window las mayúsculas no tienen relevancia, pero si en Linux
### cd tecnicatura
### mkdir Python
### mkdir Java
### mkdir JavaScript

# CLASE 2
## REPOSITORIO DE GIT Y PRIMER COMMIT
### cd tecnicatura
### mkdir class-git
### cd class-git -> Entramos en la carpeta que necesitamos trabajar
### git init -> Creamos un repositorio en la carpeta central, se crea el archivo .git
### code . -> Abrimos VSC, el punto hace que se abra el archivo en el que estamos situados
### ctrl + n -> Creamos un archivo nuevo y escribimos en el, como lo hicimos antes
### ctrl + s -> Guardamos poniendo el nombre: historia.txt
### git status -> Vemos el estado del proyecto en tiempo real, esta en el área de trabajo
### git add historia.txt -> Enviamos el archivo al área de preparación
### git status -> Para ver el estado de cambios
### git rm --cached historia.txt -> Quitamos el archivo del área de preparación, cached significa que esta en memoria ram
### git config ### Tedremos la lista de como funciona la configuración
### git config --list -> Configuraciones por defecto, faltan cosas importantes
### git config --list --show-origin -> Veremos donde están las configuraciones guardadas
### git config --global user.name "Ana Paula Ríos Garín"
### git config --global user.email "anapaulariosgarin@gmail.com" -> El correo debe ser el mismo que usaremos en GitHub
### git config --list -> Ahora veremos que ya están todos los datos completos
### git add . -> Ingresamos todos los archivos al área de preparación (ram)
### git commit -m "Mensaje importante del commit" -> El primer commit esta hecho
### code . -> Hacemos cambios en el archivo y guardamos
### git status -> Hay cambios para commitear
### git add .
### git commit -m "Mi segundo commit"
### git log historia.txt -> Vemos toda la historia de este archivo, el número largo es el hash del commit

# CLASE 3
## CARGAR LOS COMANDOS EN EL README Y COMMITEAR
### git status
### git add .
### git status
### git commit -m "Cargamos el README dentro del directorio class-git"
### git status
### git log -> Para ver los dos commits hechos: Si tienes commiteada alguna clase anterior veras mas commits de los que yo tengo.
### cd ..
### cd ..

# CLASE 4
### cd tecnicatura
### cd class-git
### ls
### touch historia.txt
### code .
### -> Modificamos el archivo historia.txt colocando lo siguiente: Bienvenido mi nombre es Ana
### ctrl + s
### git status
### git add .
### git status
### git commit -> Sin agregar -m veremos que pasa
### -> Agregar mensaje y salir con
### Esc -> Presionamos Escape 
### :wq! + enter -> Y ya salimos si estamos en git bash con window
### Esc + shift + z + z -> Salimos del mensaje para el commit, en linux, esto anda en algunas terminales
### -> Agregamos otra línea de mensaje en historia.txt desde VSC: estoy estudiando programación
### ctrl + s
### git add .
### git commit
### -> Se abre un editor de código basado en línea de comandos, editor de texto como VSC llamado vim
### Esc + i -> Para comenzar a escribir mensaje del commit, no suele ser necesario
### ctrl + x -> Para salir en linux
### s + enter -> Para decir si al cambio y aceptar el nombre, ósea no cambiamos el nombre, la (s) es de si y la (y) es de yes, no olvidar enter en linux
### git show -> Vemos todos los cambios en el último commit
### git log historia.txt -> Vemos todos los commit
### q -> Para salir del registro de commits
### -> Copiamos un hash mas antoguo y otro reciente, ingresamos el siguiente comando
### git diff hash_commit_numerico hash_commit_numerico -> Comparamos diferentes commits y sus cambios, poner la versión mas vieja primero, luego la mas nueva
### q -> Para salir
### cd ..
### cd ..

# CLASE 5
## CLASE DE TEORÍA
### ¿Qué es Gitflow?
### ¿Qué es branch (rama) y cómo funciona un merge en git?
### Tipos de ramas

# CLASE 6

# CLASE 7

# CLASE 8

# CLASE 9

# CLASE 10

# CLASE 11

# CLASE 12

# CLASE 13-

