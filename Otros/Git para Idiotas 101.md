# Pasos a seguir.
## Paso 1: Abrir Git Bash.
## Paso 2: Acceder al Repositorio.

```bash
cd Desktop/Juegos/Dragones\ \&\ Mazmorras/
```

## Paso 3: Comprobar estado del Repositorio.
Este paso es importante, nos muestra los cambios que se han realizado en la bóveda.
```bash
git status
```

### Atención.
Si muestra un mensaje diciendo:
```bash
On branch master
nothing to commit, working tree clean
```
es que no hay cambios que añadir y no es necesario continuar con los siguientes pasos.

## Paso 4: Guardar cambios y hacer Commit.

### Paso 4.1: Add.
Este comando "reconoce" los cambios dentro de la bóveda y permite guardarlos en el futuro commit. 
```bash
git add .
```

### Paso 4.2: Commit.
El commit sirve para confirmar el guardado de los cambios dentro del repositorio, para que el sistema "Se quede tranquilo". Viene adjunto a un mensaje que se debe configurar en cada commit de la siguiente manera:

```bash
git commit -m "Insertar Mensaje"
```

Este mensaje es una especie de título que sirve para identificar el nombre del cambio, para poder identificar que se ha hecho en cada cambio. 

Un ejemplo es el siguiente: Hemos asignado al primer commit el nombre de "Primer Commit", lo que nos sirve para identificarlo, sin embargo, si después del primer commit trabajamos y añadimos notas para Gael, el commit podría llamarse "Añadida información de Gael".

### ¿Quieres guardar cosas SOLO para alguien específico?
Al realizar git add. guardas **todos** los cambios realizados independientemente de en que carpeta o grupo de notas hayas trabajado. Para guardar los cambios con add de solo un grupo de carpetas, en lugar de utilizar un punto, pondremos la ruta de la carpeta. Ejemplo:

```bash
git add Razas/
```

#### IMPORTANTE
Git Bash, la aplicación que usamos, posee un autocompletado, es decir, si le damos al tabulador nos autocompleta la ruta con una que posea suficientes semejanzas.

También debes asegurarte de que las carpetas dentro de otras no sean del estilo "Razas Básicas" y "Razas Extras", pues git se confunde con el espacio. Si vas a tener subcarpetas con nombres así **dentro de la misma carpeta padre**, mejor sepáralas con guiones y no espacios.

## Paso 5: Repite paso 3 por seguridad.

## Paso 6: Subir los cambios al Repositorio Online.
Utiliza el siguiente comando:
```bash
git push origin master
```
