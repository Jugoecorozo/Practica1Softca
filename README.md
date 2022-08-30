# Practica1Softca
Softcaribbean: practica 1, Git

# Practica1Softca
SCrear repositorio

1. Crear un repositorio en vuestro GitHub llamado Practica1Softca
2. Clonar vuestro repositorio en local.
'git clone https://github.com/Jugoecorozo/Practica1Softca.git'

 

# README
3. Crear (si no lo habéis creado ya) en vuestro repositorio
local un documento README.md.
El documento README.md se creó junto al repositorio

# Commit inicial
4. Añadir al README.md los comandos utilizados hasta ahora
y hacer un commit inicial con el mensaje commit inicial.
Entramos a la carpeta del repositorio con 
'cd Practica1Softca/'

Abrimos README.md con Visual Studio Code para editarlo
code README.md

luego lo agregamos y creamos el commit
'git add README.md
git commit -m "commit inicial"'


# Push inicial
5. Subir los cambios al repositorio remoto.

'git push origin main'

# Ignorar archivos

6. Crear en el repositorio local un fichero llamado privado.txt.
7. Crear en el repositorio local una carpeta llamada privada.
8. Realizar los cambios oportunos para que tanto el archivo

como la carpeta sea ignorada por git.
'touch privado.txt
mkdir privada'
Para desarrollar el punto 8 crearemos el archivo de texto .gitignore
'touch .gitignore
code .gitignore'

luego agregaremos tanto el archivo como la carpeta al contenido de este
'privado.txt
privada/
'

# Añadir fichero 1.txt

9. Añadir fichero 1.txt al repositorio local.
'touch 1.txt
git add 1.txt
git commit -m "Añadido fichero 1.txt"
'
# Crear el tag v0.1
10. Crear un tag v0.1.

'git tag v0.1'


# Subir el tag v0.1
11. Subir los cambios al repositorio remoto.
'git push --tag origin main
git add .'

# Crear una rama v0.2
12. Crear una rama v0.2.
13. Posiciona tu carpeta de trabajo en esta rama.
'git branch v0.2
git checkout v0.2'

# Añadir fichero 2.txt
14. Añadir un fichero 2.txt en la rama v0.2.
'touch 2.txt
git commit -m "añadido 2.txt en rama v0.2"'

# Crear rama remota v0.2
15. Subir los cambios al repositorio remoto.
'git push origin v0.2'

16. Posicionarse en la rama main.

'git checkout main'

# Merge directo
17.Hacer un merge de la rama v0.2 en la rama main.

'git merge v0.2'

# Merge con conflicto
18. En la rama main poner Hola en el fichero
1.txt y hacer commit. 

'code 1.txt'

dentro del editor añadimos ”hola” y guardamos

'git add .
git commit -m "Añadido 'hola' en 1.txt"'

19. Posicionarse en la rama v0.2 y poner Adios
en el fichero "1.txt" y hacer commit.

'git checkout v0.2
code 1.txt'

dentro del editor añadimos ”adios” y guardamos

'git add .
git commit -m "añadido 'adios' en 1.txt en la rama v0.2"'


20. Posicionarse de nuevo en la rama main y hacer
un merge con la rama v0.2

'git checkout main
git merge v0.2'

lanza lo siguiente
Auto-merging 1.txt
CONFLICT (content): Merge conflict in 1.txt
Automatic merge failed; fix conflicts and then commit the result.

# Listado de ramas

21. Listar las ramas con merge y las ramas sin merge.

'git branch –merged'

Regresa lo siguiente

* main

'git branch --no-merged'

Regresa lo siguiente

  v0.2

# 
Arreglar conflicto
22. Arreglar el conflicto anterior y hacer un commit.
'code 1.txt'

Dentro del editor aceptaremos ambos cambios, con esto tanto ‘hola’ como ‘adios’ estarán en el fichero
'git add .'
'git commit -m "Conflicto solucionado, se aceptaron ambos cambios"
'
# Borrar rama
23. Crear un tag v0.2

'git tag v0.2'

24. Borrar la rama v0.2

'git branch -d v0.2'

Regresa lo siguiente

Deleted branch v0.2 (was 8e40b50).


Listado de cambios
25. Listar los distintos commits con sus ramas y sus tags.

'git log --oneline --graph'
