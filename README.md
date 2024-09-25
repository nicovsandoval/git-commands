
# Comandos útiles de Git

A continuación, se presenta una lista de comandos esenciales de Git, junto con una breve explicación de cada uno.

### 1. `git init`
Inicializa un nuevo repositorio de Git en el directorio actual. Este comando crea un subdirectorio oculto `.git`, donde se almacenarán los datos del repositorio.

### 2. `git add .`
Agrega todos los cambios (nuevos archivos, modificaciones, y eliminaciones) al área de "staging" para preparar un commit.

### 3. `git reset .`
Quita los cambios del área de "staging" (también conocido como "index"), pero los deja sin modificar en tu directorio de trabajo.

### 4. `git commit -m "mensaje"`
Crea un nuevo commit con los cambios del área de staging, añadiendo un mensaje que describe dichos cambios.

### 5. `git checkout -- .`
Restaura todos los archivos del proyecto al estado del último commit. Este comando es útil si deseas deshacer cambios locales en los archivos.

### 6. `git log`
Muestra el historial de commits realizados en el repositorio, incluyendo detalles como autor, fecha y mensajes del commit.

### 7. `git commit --amend`
Permite modificar el último commit. Usualmente se utiliza para corregir el mensaje del commit o agregar cambios que olvidaste añadir al commit anterior.
   1. Presiona la tecla `i` para entrar en el modo de edición.
   2. Luego, presiona `Escape` para salir del modo de edición.
   3. Escribe `:wq!` para guardar los cambios y salir.

### 8. `git checkout -b development`
Crea una nueva rama llamada `development` a partir de la rama actual y te cambia a esa rama automáticamente.

### 9. `git checkout main`
Te cambia de vuelta a la rama principal (usualmente llamada `main`).

### 10. `git merge development`
Fusiona la rama `development` en la rama actual. Después de ejecutar este comando, deberás agregar un mensaje de commit para completar la fusión.

### 11. `git branch -d development`
Elimina la rama `development` si ya no la necesitas. **Nota**: La rama debe estar fusionada o se mostrará un error.

### 12. `git remote add origin https://github.com/nicovsandoval/your-repository`
Agrega un repositorio remoto con el nombre `origin`, apuntando a la URL especificada. Esto te permitirá subir tus cambios a plataformas como GitHub, GitLab o Bitbucket.

### 13. `git branch -M main`
Renombra la rama actual (generalmente `master`) a `main`. Es útil cuando se sigue la convención moderna de utilizar `main` como la rama principal.

### 14. `git push -u origin main`
Envía los cambios (commits) locales a la rama `main` del repositorio remoto. La opción `-u` configura `origin/main` como la rama predeterminada para futuros `git push`.

### 15. `git commit -am "mensaje"`
Combina los comandos `git add` y `git commit` en uno solo. Esto agrega automáticamente todos los archivos modificados y crea el commit con el mensaje especificado.

### 16. `git status`
Muestra el estado actual del repositorio. Esto incluye archivos modificados, nuevos archivos sin trackear y archivos listos para commit.

---

### Notas adicionales:
- Usa `git status` en cualquier momento para verificar el estado actual de tu repositorio y ver qué archivos han sido modificados, agregados o están listos para el commit.
- Es importante elegir nombres descriptivos para los mensajes de commit y ramas para que sea más fácil rastrear los cambios en el proyecto.
