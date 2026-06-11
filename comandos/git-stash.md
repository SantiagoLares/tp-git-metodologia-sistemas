# git stash

## ¿Para qué sirve `git stash`?

`git stash` permite guardar temporalmente los cambios que tenés en tu directorio de trabajo sin necesidad de hacer un commit. Los cambios quedan "en pausa", tu directorio vuelve al estado del último commit, y después podés recuperarlos cuando quieras.

## ¿En qué situación conviene usarlo?

El caso más típico es cuando estás trabajando en algo a mitad de camino y de repente necesitás cambiar de rama (por ejemplo, para revisar algo urgente o ayudar a un compañero), pero todavía no querés hacer un commit porque el trabajo está incompleto.

Sin `git stash`, Git no te dejaría cambiar de rama si tenés cambios sin commitear que entren en conflicto. Con `git stash` guardás todo temporalmente, hacés lo que necesitás, y después retomás desde donde lo dejaste.

## ¿Cómo guardar cambios temporalmente?

```bash
git stash
```

Esto guarda todos los cambios rastreados (tracked) que tengas sin commitear y limpia el directorio de trabajo. Si también querés incluir archivos nuevos que todavía no fueron agregados con `git add`, usás:

```bash
git stash -u
```

## ¿Cómo recuperar esos cambios?

Para traer de vuelta los últimos cambios guardados en el stash y aplicarlos sobre la rama actual:

```bash
git stash pop
```

Esto recupera los cambios **y los elimina del stash**. Si en cambio querés aplicarlos pero mantenerlos guardados (por ejemplo, para aplicarlos en más de una rama), usás:

```bash
git stash apply
```

Para ver qué tenés guardado en el stash:

```bash
git stash list
```

## Ejemplos

```bash
# Guardar los cambios actuales en el stash
git stash

# Recuperar los cambios y eliminarlos del stash
git stash pop
```
