# git status

El comando `git status` funciona como una herramienta de diagnóstico que te permite conocer el estado actual de tu repositorio en cualquier momento. Su objetivo principal es mostrar que modificaciones se han realizado en el directorio de trabajo y cuáles de esos cambios estan listos para ser guardados definitivamente. Al utilizarlo, git no modifica ningún archivo ni altera el historial; simplemente analiza la carpeta y te entrega un reporte detallado de la situación.

Al leer este reporte, te podés encontrar con distintas categorías de archivos. Primero, los "archivos sin seguimiento" (untracked), que son aquellos documentos nuevos que acabás de crear (por ejemplo, si agregaste un archivo `index.html` a una pagina) y que git todavía no está registrando. Segundo, los "archivos modificados" (modified), que son los archivos que Git ya conocía porque estaban en el historial, pero sufrieron cambios recientes. Por último, los "archivos preparados" o "agregados" (staged), que son las modificaciones ya marcadas para que formen parte del próximo guardado.

### Ejemplo de uso

`bash`
`git status`
