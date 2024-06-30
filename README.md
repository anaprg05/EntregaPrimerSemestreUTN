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
### cd tecnicatura
### cd class-git
### ls
### code .
### git log -> Vemos los commit hechos hasta ahora
### Copiar el hash -> El número largo que tiene el commit
### git reset hash-nombre-commit -> Este nos permite volver a una versión anterior, hay 2 tipos de reset: el duro y el suave
### git status
### git add .
### git commit -m "Agregamos datos de estudios en historia.txt"
### git config --list -> Veremos la configuración que ya hemos hecho con en nombre y email
### git reset hash-nombre-commit --hard -> Es el duro, todo vuelve a su estado anterior, es el más usado, desaparece todo
### git reset hash-nombre-commit --soft -> Este es el suave, lo que tengamos en staging segirá allí
### crear un archivo #portafolio.html introducir el código y
### touch portafolio.html
### html : 5 -> Con esto se carga el código básico de html y modificamos
### ctrl + s -> Guardamos
### Clic derecho en VSC Open with Live Server para ver en el navegador
### git status
### ls
### ls -al
### git add .
### git status
### git commit -m "Agregamos el html para nuestro portafolio"
### creamos CSS -> Este es un archivo de estilos, para esto creamos una nueva carpeta llamada css
### mkdir css
### ls
### cd css
### touch style.css -> creamos un archivo dentro: estilos.css le cargamos el código.
### ctrl + s -> abrimos en el navegador y todo esta allí, pero todo esto supuestamente en git no existe.
### git status -> tenemos cosas en el área de trabajo, en staging distintas
### git diff + enter -> y nos muestra los cambios en memoria ram y en disco
### git add . -> Agregamos todo al staging
### git status -> Ya esta todo en memoria ram, a git solo le importan los archivos, guarda las carpetas como rutas y automaticamente las crea
### git commit -m "Creamos el css para darle algo de estilo a nuestro portafolio"
### git log -> vemos lo nuevo que hemos hecho sin lo que borramos con el reset fuerte
### hacer cambios en historia.txt -> Cambiamos la última línea y
### ctrl + s 
### git diff
### git commit -am "cambio en la última línea del historia.txt"
### git log
### q  #Esto para salir
### git log --stat -> veremos los cambios especificos que hicimos en cuales archivos por medio del commit y veremos los cambios en bits
### q -> salimos de la línea de commits, ahora queremos ver como era originalmente el archivo, osea la primera versión, copiamos el nombre del primer commit
### git checkout hash-nombre-commit historia.txt -> Veremos el archivo en su estado original
### git status -> Nos sugiere hacer un commit, si lo hacemos borramos todo lo que hicimos antes, debemos seguir con el siguiente commando
### git checkout master historia.txt -> Volvemos a la versión master del archivo historia.txt, esto es muy peligroso
### git checkout hash-nombre-commit historia.txt -> Volvemos a hacer esto y cambiamos cosas del archivo
### git commit -am "Reemplazo de una versión por otra de la historia"
### git log -> Veremos los cambios sin tocar ningun otro archivo, esta es la forma de volver a una versión hacía atrás y llevarla a la cabeza de la master
### cd ..
### cd ..

# CLASE 7
### mkdir git_reset_test -> Vamos a hacer pruebas, es por esto que creamos una carpeta nueva
### cd git_reset_test -> Entramos en la carpeta
### git init -> Inicializamos el repositorio
### touch reset_file.txt
### git add reset_file.txt
### git commit -m "Iniciando el primer commit"

## CLASE DE TEORÍA
### GIT RESET

# CLASE 8

# CLASE 9

# CLASE 10

# CLASE 11

# CLASE 12

# CLASE 13

