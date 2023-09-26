# Comandos de Git para ser un Pro

1. **git init**: Inicializa un repositorio de Git en un directorio existente.
2. **git clone**: Clona un repositorio remoto en su computadora local.
3. **git add**: Agrega archivos al área de preparación (staging area) para que puedan ser incluidos en el próximo commit.
4. **git commit**: Crea un punto de control en el historial del repositorio con los cambios actuales en el área de preparación.
5. **git status**: Muestra el estado actual de los archivos en el repositorio, incluyendo los cambios que no han sido incluidos en el área de preparación.
6. **git log**: Muestra el historial de commits del repositorio.
7. **git diff**: Muestra las diferencias entre los archivos en el repositorio y los cambios no confirmados.
8. **git branch**: Muestra una lista de ramas en el repositorio y la rama actual.
9. **git merge**: Combina otra rama en la rama actual.
10. **git pull**: Trae los cambios de un repositorio remoto y combina con la rama actual.
11. **git push**: Envía los cambios locales a un repositorio remoto.

**Recuerde siempre hacer un git pull antes de empezar a trabajar en una rama y hacer git push y git pull request una vez terminado de trabajar en ella.**


1. Clonar un repositorio remoto:
   git clone <URL-del-repositorio>

2. Actualizar tu repositorio local:
   git pull

3. Crear una nueva rama:
   git checkout -b nombre-de-rama

4. Cambiar de rama:
   git checkout nombre-de-rama

5. Ver el estado de los cambios locales:
   git status

6. Agregar archivos al área de preparación (staging):
   git add nombre-de-archivo

7. Hacer una confirmación (commit):
   git commit -m "Mensaje de confirmación"
   git commit -m "feat(authentication): add user login functionality"

8. Subir cambios al repositorio remoto:
   git push

9. Ver el historial de confirmaciones:
   git log

10. Ver diferencias entre confirmaciones:
    git diff commit1 commit2

11. Eliminar una rama local:
    git branch -d nombre-de-rama

12. Eliminar una rama remota:
    git push origin --delete nombre-de-rama

13. Recuperar cambios eliminados:
    git checkout -- nombre-de-archivo

14. Resolver conflictos de fusión:
    # Después de resolver conflictos, agrega y confirma los cambios.
    git add nombre-de-archivo
    git commit -m "Resuelto conflicto de fusión"

15. Etiquetar confirmaciones:
    git tag nombre-de-etiqueta


# Paso 1: Clonar el Repositorio
1. Clona el repositorio desde el repositorio remoto a tu máquina local:
   git clone <URL-del-repositorio>

# Paso 2: Crear una Nueva Rama
2. Cambia a la rama principal (main o master):
   git checkout main

3. Asegúrate de que tu rama principal esté actualizada:
   git pull

4. Crea una nueva rama para tu trabajo:
   git checkout -b nombre-de-tu-rama

# Paso 3: Trabajar en la Rama
5. Realiza tus cambios en la rama y realiza confirmaciones (commits) frecuentes:
   git add .
   git commit -m "Mensaje descriptivo de la confirmación"

# Paso 4: Subir Cambios al Repositorio Remoto
6. Sube tus cambios a la rama remota correspondiente:
   git push origin nombre-de-tu-rama

# Paso 5: Eliminar la Rama (Opcional)
7. Si la rama ya no es necesaria, puedes eliminarla localmente:
   git branch -d nombre-de-tu-rama

8. También puedes eliminar la rama remota después de hacer merge:
   git push origin --delete nombre-de-tu-rama

# Paso 6: Hacer el Merge
9. Una vez que tus cambios están listos y revisados, realiza el merge a la rama principal:
   git checkout main
   git merge nombre-de-tu-rama

# Paso 7: Repetir el Ciclo (Opcional)
10. Si tienes más tareas, crea una nueva rama y repite los pasos 3-6.

# Nota: Asegúrate de utilizar nombres descriptivos para tus ramas y confirmaciones.
