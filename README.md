# clases-yamil
Playwright 

crear rama
git checkout -b

elimina un branch en github
git push origin --delete NOMBRE_DE_LA_RAMA

elimina un branch en git
git branch -d NOMBRE_DE_LA_RAMA

Modificar nombre de la rama
git branch -m nuevo-nombre

### Selectores

Priorizar en este orden:
1. getByRole - Para elementos con roles ARIA, ya que son accesibles y semánticos.
2. getByLabel - Para campos de formulario, ya que están asociados con etiquetas y son fáciles de entender.
3. getByTestId - Para elementos específicos de testing, ya que son robustos y no cambian con frecuencia.
4. getByText - Para texto visible, útil cuando el texto es único y no cambia.
5. locator - Para selectores CSS o XPath, cuando los anteriores no son aplicables.
5. getByPlaceholder - Para campos de entrada con texto de placeholder.
5. getByAltText - Para imágenes con texto alternativo.


Paso a Paso Git:

-Crear la nueva rama: git checkout -b "nombre-de-mi-rama"
-Agregar algo a la rama (Directamente en el archivo, no terminal)
-Git add . (Esto lo agrega a un stage)
-Hacer el commit: git commit -m "Aqui va el cambio generado"
-Acá hacemos el push, subir los cambios a GitHub: git push origin "Nombre de mi rama con cambios"
-GITHUB: Generar el Pull Request seleccionar mi rama y colocar en la descripción el cambio que hice (en un ambiente real debo esperar la aprobación del líder)
-Una vez aprobado, eliminar la rama creada en GH y luego en Git: git branch -d NOMBRE_DE_LA_RAMA
-Siempre hacerle pull al main, mantenerlo actualizado: git pull


# Tipo de commit (elige uno):
# feat     → nueva funcionalidad
# fix      → corrección de bug
# test     → cambios en pruebas (agregar, reactivar, modificar)
# chore    → mantenimiento, configs, dependencias
# refactor → cambios en código sin alterar funcionalidad
# docs     → documentación
# style    → formato, lint, espacios, etc.

# Ejemplos

# feat(auth): agregar login con Google
# fix(inbox): corregir error al abrir conversación archivada
# test(chatbot): reactivar casos skippeados en suite smoke
# chore(ci): actualizar configuración de pipeline
# refactor(forms): simplificar validaciones de inputs
# docs(readme): agregar instrucciones de instalación
# style(lint): aplicar formato con prettier



| Tipo          | Propósito                                                            | Ejemplo                           |
| ------------- | -------------------------------------------------------------------- | --------------------------------- |
| **feature/**  | Nueva funcionalidad o historia de usuario                            | feature/add-user-authentication |
| **bugfix/**   | Corrección de errores detectados en QA o producción                  | bugfix/fix-login-timeout        |
| **hotfix/**   | Solución urgente en main o producción                                | hotfix/allure-report-crash      |
| **test/**     | Nuevas pruebas automatizadas o mejoras en las existentes             | test/create-smoke-suite         |
| **chore/**    | Mantenimiento, configuración o tareas no funcionales                 | chore/update-node-version       |
| **docs/**     | Cambios en documentación o README                                    | docs/playwright-guidelines      |
| **refactor/** | Reestructuración de código sin cambio funcional                      | refactor/pom-structure          |
| **ci/**       | Cambios en pipelines o integraciones (GitHub Actions, Jenkins, etc.) | ci/improve-allure-upload        |