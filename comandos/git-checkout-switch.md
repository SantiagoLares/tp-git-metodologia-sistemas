# git checkout / git switch

## ¿Para qué sirve cambiar de rama?

Cuando estás trabajando en un repositorio con varias ramas, necesitás "moverte" de una a otra para trabajar en distintas partes del proyecto. Cambiar de rama actualiza los archivos de tu directorio de trabajo para que reflejen el estado de la rama a la que te moviste.

## Diferencia básica entre `checkout` y `switch`

- `git checkout` es el comando clásico y más antiguo. Sirve para cambiar de rama, pero también tiene otros usos (como restaurar archivos), lo que puede generar confusión.
- `git switch` fue introducido en Git 2.23 específicamente para cambiar de rama, con una sintaxis más clara e intuitiva. Es la opción recomendada cuando solo querés moverte entre ramas.

En la práctica, los dos funcionan bien para este propósito. La diferencia es de claridad y semántica.

## ¿Cómo crear y cambiarse a una rama al mismo tiempo?

En lugar de crear la rama con `git branch` y luego cambiarse, podés hacerlo en un solo paso:

Con `checkout`:

```bash
git checkout -b feature/nueva-rama
```

Con `switch`:

```bash
git switch -c feature/nueva-rama
```

Ambos crean la rama y te mueven a ella directamente.

## Ejemplos

```bash
# Crear una nueva rama y moverse a ella (con checkout)
git checkout -b feature/nueva-rama

# Cambiarse a la rama main (con switch)
git switch main

# Crear una nueva rama y moverse a ella (con switch)
git switch -c feature/nueva-rama
```
