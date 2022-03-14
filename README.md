
# Readme

<!-- badges: start -->
<!-- badges: end -->

Este es un proyecto de prueba para como usar git en R y conectarlo a GitHub.
En primer lugar hemos usado esta página donde se detalla a la perfección:

(Link a la página)![http://destio.us.es/calvo/asignaturas/ge_esco/tutorialusargitgithubrstudio/UsarGitGithubconRStudio.html]

En primer lugar este repo se ha hecho en R y luego se ha subido. Tambien se podría hacer el reves como viene detallada en la página

1. En primer lugar, se ha seteado la configuración del usuario. Para ello hemos usado la librería `library(usethis)` de la cual hemos usado 

``` bash
usethis::edit_git_config()
# Modificar en el fichero ".gitconfig" los apartados: "name" y "email" 
# y guardar el fichero
```

2. UNa vez seteados estos parámetros, hemos creado un proyecto como siempre y marcado la casilla de git. Sino lo podemos dejar sin marcar y seguir los pasos:

``` bash
library(usethis)
usethis::use_git()
# Elegir siempre la opción: 1
# Y ante la ventana, seleccionar: "Save"
```


3. En el relojito de la pestaña de Git podemos hacer los commits y demas, es muy facil.
4.Por último, para conectar Git y R tenemos que generar un tokken (PAT), Hemos seguido los pasos de esta página (Fallo)![https://community.rstudio.com/t/error-no-github-auth-token-is-available/75975]

En el seteamos que el protocolo sea hhtps y luego nos lleva a la página de generar el token de github. Este lo debemos de copiar en el path del fichero `usethis::edit_r_environ()` dejando la linea de abajo vacia.

5. Usamos la función:

``` bash

library(usethis)
usethis::use_github()

```

Si no funciona hacer un restar de R.

6. Estos cambios los estamos haciendo despues de crear el repo en GitHub ahora lo que tenemos que hacer es darle a la flecha verde para el push.


