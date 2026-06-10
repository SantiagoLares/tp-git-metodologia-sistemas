# git add y git commit

Los comandos `git add` y `git commit` trabajan en conjunto para guardar de manera definitiva los cambios en el historial del repositorio. Mientras trabajas en un proyecto, Git detecta esas modificaciones en tu directorio de trabajo. Sin embargo, no las guarda automáticamente. Primero entra en juego `git add`, cuya función es tomar esos archivos modificados y moverlos a un area de preparación o "staging area".

Una vez que los archivos están preparados, se utiliza el comando `git commit`. Su proposito es confirmar esos cambios de manera permanente, viendo como están los archivos en ese instante y agregandolo al historial cronológico del proyecto. La diferencia fundamental entre ambos pasos es que preparar los cambios (`add`) te permite armar un paquete a medida, decidiendo exactamente qué modificaciones van juntas, mientras que confirmarlos (`commit`) es el acto de sellar esa caja con una etiqueta descriptiva (el mensaje) para que quede registrada.

### Ejemplo de uso

`bash`
`git add .`
`git commit -m "feat: agregar explicacion de comandos basicos"`
