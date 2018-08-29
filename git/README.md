# GIT-COMMAND

## Tabla De Contenidos

1. [Git Commit](#git-commit)
1. [Git Merge](#git-merge)
1. [Git Branch](#git-branch)
1. [Git Stash](#git-stash)
1. [Git Tags](#git-tags)
1. [Git Show](#git-show)
1. [Git Config](#git-config)
1. [Git Reflog](#git-reflog)

## Git Commit

Sirve realizar el commit sobre los cambios que tenemos en local.

```bash
$> git commit
```

Este comando permite una serie de parámetros

### -m

Para incluir un comentario en nuestro commit

```shell
$> git commit -m '[Nuestro comentario]'
```

### --amend

Sirve para modificar el log de un commit que hayamos realizado. Luego podremos editar el último commit y si deseamos corregir algún error que hayamos cometido.

```shell
$> git commit --amend
```

**[⬆ back to tabla de contenidos](#tabla-de-contenidos)**

## Git Merge

Este comando se usa para realizar los merge entre ramas.

```shell
$> git merge [Nombre de la rama que queremos mergear]
```

### --abort

Con este comando podemos abortar un merge en curso. Si el merge nos ha dado conflicto y no queremos volvernos locos haciendo el merge, podemos abortarlo con este comando.

```shell
$> git commit --abort
```

Si el merge se ha realizado correctamente, este comando no realizará ninguna acción

**[⬆ back to tabla de contenidos](#tabla-de-contenidos)**

## Git Branch

Este comando nos sirve para trabaja con las ramas de nuestro proyecto.

Si lo ejecutamos sin ningún flag, nos mostrará un listado de las ramas que tenemos en local.

```shell
$> git branch
```

### -r

Con este flag nos listará unicamente las ramas remotas de nuestro repositorio

```shell
$> git branch -r
```

### -a

Con este flag nos listará todas las ramas que tenemos en nuestro repositorio, tanto las locales como las remotas.

```shell
$> git branch -a
```

### [Nombre de la ramma]

Si a continuación de branch le añadimos el nombre de una rama nos creará la rama a partir de la rama que tenemos.

```shell
$> git branch [nombre de la rama]
```

### -d [nombre de la rama]

Con este comando eliminará un rama de manera local.

```shell
$> git branch -d [nombre de la rama]
```

### -D [nombre de la rama]

Con este comando eliminará un rama de manera forzada.

```shell
$> git branch -D [nombre de la rama]
```

### -m [nombre nuevo]

Con este comando podremos modicar el nombre de una rama mientras estamos situados encima de ella.

```shell
$> git branch -m [nombre nuevo]
```

### -m [nombre anterion] [nombre nuevo]

Con este comando podremos modicar el nombre de una rama sin estar posicionados en ella.

```shell
$> git branch -m [nombre anterion] [nombre nuevo]
```

**[⬆ back to tabla de contenidos](#tabla-de-contenidos)**

## Git Stash

Sirve para guardar el estado actual de tus cambio sin tener que realizar un commit en tu proyecto, al usarlo devuelves el puntero hacia el último commit realizado como si nada hubiera pasado. Así los cambios que se realizaron se quedan guardados en una rama temporal de Git y los puedes recuperar cuando desees, con los siguientes comandos `git stash apply` o `git stash pop`

```shell
$> git stash
```

### apply

Con este comando recuperas los cambios que habias guardado de manera temporal.

```shell
$> git stash apply
```

**[⬆ back to tabla de contenidos](#tabla-de-contenidos)**

## Git Tags

Con este comando podemos etiquetar versiones que hayamos realizado en nuestro repositorio.

```shell
$> git tag
```

### -a v.0.0.1 -m "[Comentario de la nueva etiqueta]"

Con este comando recuperas los cambios que habias guardado de manera temporal.

```shell
$> git tag -a v.0.0.1 -m "[Comentario de la nueva etiqueta]"
```

### push origin tag v0.0.1

Una vez que lo tenemos etiquetado correctamente podemos subirlo al servidor con el siguiente comando.

```shell
$> git push origin tag v0.0.1
```

**[⬆ back to tabla de contenidos](#tabla-de-contenidos)**

## Git Show

Con este comando podemos ver la información de varios tipos de objetos GIT

```shell
$> git show v0.0.1 -s
```

**[⬆ back to tabla de contenidos](#tabla-de-contenidos)**

## Git Config

Con este comando podemos leer y escribir las configuraciones de GIT, por usuario y por repositorio.

### config --global user.name 'John Doe'

Con este comando podemos definir el nombre con que será identificado la persona que realiza los commits.

```shell
$> git config --global user.name 'John Doe'
```

### config --global user.email "email@dominio.com"

Con este comando podemos definir el mail.

```shell
$> git config --global user.email "email@dominio.com"
```

**[⬆ back to tabla de contenidos](#tabla-de-contenidos)**

## Git Log

**[⬆ back to tabla de contenidos](#tabla-de-contenidos)**

## Git Reflog


**[⬆ back to tabla de contenidos](#tabla-de-contenidos)**
