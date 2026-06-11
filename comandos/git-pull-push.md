# git pull / git push

## ¿Para qué sirve `git pull`?

`git pull` se usa para traer los cambios que están en el repositorio remoto (por ejemplo, GitHub) y aplicarlos en tu rama local. Es la forma de mantener tu copia del proyecto actualizada con lo que hicieron los demás integrantes del equipo.

Internamente, `git pull` hace dos cosas seguidas: primero descarga los cambios (`git fetch`) y después los integra en tu rama actual (`git merge`).

## ¿Para qué sirve `git push`?

`git push` es el proceso inverso: sube los commits que hiciste en tu máquina al repositorio remoto. De esta forma, tus cambios quedan disponibles para el resto del equipo y quedan registrados en GitHub.

## ¿Cuándo se usan?

- Usás `git pull` **antes de ponerte a trabajar**, para asegurarte de que tenés la versión más reciente del proyecto. También es buena práctica hacerlo antes de un merge, para evitar conflictos innecesarios.

- Usás `git push` **cuando terminaste de trabajar en algo** y querés compartir tus cambios con el equipo o simplemente tenerlos respaldados en el remoto. Lo normal es hacer push después de uno o varios commits relacionados.

## Ejemplos

```bash
# Traer los últimos cambios del remoto a tu rama actual
git pull

# Subir los commits locales de una rama al repositorio remoto
git push origin nombre-rama
```

> **Nota:** la primera vez que hacés push de una rama nueva que creaste localmente, Git puede pedirte que indiques el destino remoto. En ese caso podés usar:
> ```bash
> git push --set-upstream origin nombre-rama
> ```
> o en su forma corta:
> ```bash
> git push -u origin nombre-rama
> ```
