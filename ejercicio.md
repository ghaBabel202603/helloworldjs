# Ejercicio: fork, GitHub Actions y despliegue en GitHub Pages

## Objetivo

Practicar un flujo real de CI/CD con GitHub Actions a partir de este repositorio:

1. Hacer un fork del repositorio en tu cuenta `owner`.
2. Adaptar la configuración necesaria para que el fork pueda desplegar correctamente.
3. Lanzar el workflow con un `push` a la rama adecuada.
4. Verificar en GitHub Actions que la pipeline termina en verde.
5. Verificar en GitHub Pages que la aplicación queda publicada y accesible.

## Contexto del repositorio

Este proyecto contiene una aplicación React y un workflow en [`.github/workflows/workflow.yml`](.github/workflows/workflow.yml) que:

- se ejecuta con `push` sobre `main` y `develop`
- construye la aplicación
- despliega el resultado a GitHub Pages

Hay una pista importante en [`package.json`](helloworldjs/package.json): la propiedad `homepage` apunta al repositorio del owner original, no al fork.

## Enunciado

Realiza las siguientes tareas sobre tu fork:

1. Haz un fork de este repositorio en tu cuenta de GitHub.
2. Clona tu fork en local.
3. Crea una rama de trabajo.
4. Revisa el workflow existente para entender cuándo se ejecuta y qué hace.
5. Corrige la configuración necesaria para que el despliegue en GitHub Pages funcione desde tu fork.
6. Haz un commit con el cambio.
7. Sube la rama y crea un `push` a `main` o `develop` para disparar el workflow.
8. Comprueba en la pestaña `Actions` que el job termina correctamente.
9. Comprueba en la configuración del repositorio que GitHub Pages está sirviendo el contenido publicado.
10. Accede a la URL pública y valida que la aplicación se ve correctamente.

