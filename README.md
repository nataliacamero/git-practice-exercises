# Práctica del curso de git, github y Sourcetree

## Ejercicio 1

### Respuestas:

- ¿Qué comandos utilizaste en el paso 11? ¿Por qué?.

  - El comando que utilicé fue `git reset --hard HEAD~1`, ya que este comando es la suma de `git reset HEAD~1` (el cual afecta mi repo y deshace el último commit) y el comando `git restore <file>` (que afecta los cambios realizados en mi working copy).

- ¿Qué comando o comandos utilizaste en el paso 12? ¿Por qué?.

  - Primero use `git reflog` para tomar el id del commit y luego el comando que utilicé fue `git reset —hard c61c242`, ya que este comando mueve la rama al commit que le indicamos, o mejor dicho hace que la referencia apunte al commit que indicamos. Asi que que volvi a ubicarme en el commit que habia realizado anteriormente, gracias a que el historial de commits en Git nunca se pierde, esto gracias a que Git está diseñado para mantener un registro completo de todos los commits realizados en el repositorio.

- El merge del paso 13, ¿Causó algún conflicto? ¿Por qué?.

  - El merge del paso 13 fue Fast Foward, ya que en la rama main no habia cambios sin registrar por git, los cambios del commit actual, producto del merge solo eran de la rama styled.

- El merge del paso 19, ¿Causó algún conflicto? ¿Por qué?.

  - EL merge del paso 19 fue un not fast-foward, ya que tanto la rama styled como la rama htmlify, tenian commits a los que no se les habian dado acceso respecto de los cambios realizados en el mismo archivo y mismas lineas.

- El merge del paso 21, ¿Causó algún conflicto? ¿Por qué?.

  - Este merge no causo conflicto, por que en el paso 13 con el HEAD en la rama styled hice un merge con main, por lo tanto, tenia acceso al los cambios que se hicieron en styled. Y al hacer el merge con styled desde la rama main, ya no había conflictos por que ya main tenia los cambios. Fue un merge fast foward.

- ¿Qué comando o comandos utilizaste en el paso 25?.

  - Dibuje el diagrama con el comando `git log —graph`.

- El merge del paso 26, ¿Podría ser fast foward? ¿Por qué?.

  - Podria ser fast foward por que no hubo conflictos, agrege una linea entera nueva.

- ¿Qué comando o comandos utilizaste en el paso 27?.

  - El comando que utilicé fue `git reset HEAD~1`, ya que asumí este cambio, como deshacer el último commit, sin afectar el working copy.

- ¿Qué comando o comandos utilizaste en el paso 28?.

  - EL comando que utilice fue `git restore git-nuestro.md`.

- ¿Qué comando o comandos utilizaste en el paso 29?.

  - En este caso utilice `git branch -D title`, ya que dejaba un commit inaccesible.

- ¿Qué comando o comandos utilizaste en el paso 30?.

  - En este paso `git reflog` y `git reset —hard ca40d82`.

- ¿Qué comando o comandos utilizaste en el paso 32?.

  - En este paso `git reflog` y `git reset —hard d78fda1`.

- ¿Qué comando o comandos utilizaste en el paso 33?.

  - En este paso `git reflog` y `git reset —hard ca40d82`.
