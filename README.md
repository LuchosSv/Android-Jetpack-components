# Android Jetpack

## Creación del proyecto en android studio.

Abrimos android studio y creamos un nuevo proyecto, seleccionamos empty activity le ponemos un nombre, dejamos con lenguaje kotlin y ponemos minimo SDK API 15.

## Creación del repositorio en github.

Perfil, tus repositorios y nuevo.
Le ponemos un nombre, una pequeña descripción, lo dejamos en publico no inicializamos en readme.md y creamos el repositorio.

1) Ahora vamos a la consola de comandos (git bash), y nos movemos a la carpeta del proyecto ~/AndroidStudioProjects/tuproyecto dentro de la carpeta de proyecto con git bash usas el comando 
```bash
git init
```
para iniciar un repositorio en tu maquina te pondrá que estas en master. Puede dar seguimiento al estado de tu proyecto con git status

2) Luego opcionalmente podemos incluir un readme.md para hablar un poco mas afondo de la aplicacion con el comando 
```bash
echo "# Android-Jetpack-components" >> README.md
```

3) Luego de haber hecho el primer paso (2 opcional) ejecutamos el comando 
```bash
git add .
```
con esto le decimos que queremos añadir nuestro proyecto al staging area que es un paso antes de añadirlo al repositorio y con el . le decimos que añada todo lo que se encuentra en la carpeta.
Si usas el comando 
```bash
git status
```
te pondra todo en verde que significa que ya estas en staging area a un paso de añadirlo a tu repositorio local si algo queda en rojo es que git lo le esta dando seguimiento y es tu decidion tranckarlo o no.

4) El siguiente comando
```bash
git commit -m "first commit"
```
estamos terminando de añadir nuestro proyecto al repositorio local con la bandera -m le decimos que vamos a añadirle un comentario entre las comillas y como comentario en recomendable ser descriptivo a lo que se hiso de cambio, en este caso como es nuestro primer commit ponemos "first commit" en comillas porque es texto.

5) Ahora para subir tu repositorio local a tu repositorio creado en github primero hay que crear el enlace con el comando git remote add
quedaria asi:
```bash
git remote add origin git@github.com:LuchosSv/Android-Jetpack-components.git
```
(tambien puedes usar la opcion https) primero el comando ya mencionado luego le ponemos nombre por defecto se le deja origin y por ultimo la ruta del repositorio.
Y por ultimo paso el comando
```bash
git push -u origin master
```
que lo que hace es empujar todo tu repositorio local al remoto por medio de git push y usando la rama master con el remote creado anteriormente que es origin.
