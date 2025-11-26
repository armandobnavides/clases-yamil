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