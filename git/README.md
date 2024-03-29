# Comandos git

#### Comandos iniciales

+ Para ver el estado de repositorio se usa:
```Shell
git status
```
+ Para clonar un repositorio de manera local se usa:
```Shell
git clone [Aqui va la URL del repositorio]
```
+ Para saber en que rama estoy se usa, lo señala con un asterisco
 ```Shell
git branch
```

#### Comandos para subir informacion al repositorio

1. Revisar el estado en el que se encuentra el repositorio.
```Shell
git status
```
2. Debemos de agregar el estadonuevo al commit, con el siguiente Comandos
```Shell
git add [Ruta completa del archivo]
```
2.1 Para agregar **todos** los cambios es con el siguietne comando
```Shell
git add .
```
3. Una vez que se agregaron los archivos se debe hacer commit
```Shell
git commit -m "[Aqui va el mensaje del commit]"
```
4. Para subir el commit al servidor es con el siguiente comando
```Shell
git push origin [nombre de la rama]
```

### Gestion de ramas
#### Crear rama
1.Para crear una rama se usa el siguiente comando
```Shell
git branch [Nombre rama]
```
2. Para cambiarnos a otra rama se usa
```Shell
git checkout [Nombre rama]
```
2.1 Para hacer los puntos 1 y 2 en un solo comando es el siguiente
```Shell
git checkout -b [Nombre de la rama]
```
3. Para publicar la rama en el servidor se usa
```Shell
git push origin [Nombre de la rama]
```

#### Borrar ramas

+ Para borrar la rama localmente es
```Shell
git branch -d [Nombre de la rama]
```
+ Para borrar la rama en el servidor es con
```Shell
git push origin --delete [Nombre rama]
```

#### Integracion de ramas / Mezcla
1. Ir a la rama donde se integraran los cambios
```Shell
git checkout [Nombre rama]
```
2. Para hacer la integracion de los cambios se usa el comando
```Shell
git merge [Nombre de la rama de la que traemos los cambios]
```
> Notas: Si el cambio **no** genera conflictos podemos hacer el push sin problema.
3. Para subir los cambios se usa
```Shell
git push origin [Nombre de rama que recibe los cambios]
```
