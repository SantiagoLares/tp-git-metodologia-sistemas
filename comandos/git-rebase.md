## GIT REBASE:

# El comando "git rebase" permite mover o reaplicar commits sobre otra base de trabajo.
# Se utiliza para actualizar alguna rama con los cambios mas recientes y poder mantener un historial mas limpio.
# La diferencia con merge es que merge crea un commit de union de ramas, rebase reorganiza el historial reaplicando commits.

# EJEMPLO:

# bash
# git checkout feature/nombre-rama
# git rebase main   

# EXPLICACION: Los cambios de la rama actual se vuelven a aplicar sobre la version mas reciente de main.