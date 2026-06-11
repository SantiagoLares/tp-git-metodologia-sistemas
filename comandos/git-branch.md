# git branch

## ¿Qué es una rama en Git?

Una rama en Git es básicamente una línea de desarrollo independiente dentro de un mismo repositorio. Podés pensarlo como una copia del proyecto en un momento dado, sobre la cual podés trabajar libremente sin afectar el resto del código.

Por defecto, todo repositorio arranca con una rama principal llamada `main` (o `master` en versiones más antiguas de Git).

## ¿Para qué sirve trabajar con ramas?

Trabajar con ramas permite que varias personas (o vos mismo en distintos momentos) puedan desarrollar funcionalidades, corregir bugs o hacer experimentos de forma paralela, sin pisarse el trabajo entre sí. Una vez que los cambios están listos y revisados, se integran a la rama principal mediante un merge o rebase.

Esto hace que el historial del proyecto sea más ordenado y que sea mucho más fácil revertir cambios si algo sale mal.

## ¿Cómo ver las ramas existentes?

Para listar todas las ramas locales del repositorio:

```bash
git branch
```

La rama activa aparece marcada con un asterisco (`*`).

Si también querés ver las ramas remotas (las que están en GitHub, por ejemplo), usás:

```bash
git branch -a
```

## ¿Cómo crear una rama?

Para crear una rama nueva a partir de la rama en la que estás parado actualmente:

```bash
git branch nombre-rama
```

Esto **solo crea** la rama, pero no te mueve a ella. Para empezar a trabajar en ella, hay que cambiar a esa rama (ver `git-checkout-switch.md`).

## Ejemplos

```bash
# Ver todas las ramas locales
git branch

# Crear una rama llamada feature/login
git branch feature/login
```
