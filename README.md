# GPUL School landing page

Landing page para el proyecto GPUL School

## Añadir una charla

Se puede crear el evento con Hugo
```bash
hugo new content content/charlas/<YYYY>/<nombre-charla>/index.md
```

O copiando un evento y modificándolo. La ruta de una charla es `content/charlas/<YYYY>/<permalink>/index.md. En el mismo directorio se pueden subir los recursos relacionados con la charla, como diapositivas o el cartel, y se enlaza desde el archivo con rutas relativas (así que directamente con el nombre del archivo).

Los detalles de la charla se especifican en front-matter, y los campos son:
```
+++
title = '<Título de la charla>'
date = 2024-10-07T14:32:00+02:00    # Fecha en la que será la charla
poster = '<ruta del cartel>'
summary = 'Breve resumen de la charla'
location = 'Aula x.x - Facultade de Informática'
time = '18:30 a 20:30'
author = ''
author_link = ''
meetup = ''
+++
```

Solo son obligatorios el título, la fecha y el cartel. Si no quieres que un campo aparezca, puedes dejarlo en blanco o eliminar su línea. Es posible añadir el nombre del ponente y no un enlace, pero si hay varios ponentes no se pueden añadir varios enlaces, ya que todos los autores tienen que ir dentro de una sola etiqueta.

Como las fechas de muchas charlas serán en el futuro, si quieres previsualizar el sitio, con `hugo server` no aparecerán, hay que añadir la opción `--buildFuture

### Licencia
[Licencia Creative Commons Atribución-CompartirIgual 4.0 Internacional](http://creativecommons.org/licenses/by-sa/4.0/)
