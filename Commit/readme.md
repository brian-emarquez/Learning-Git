### Recomendaciones para generar un buen commit

_github bestpractices_

Durante el desarrollo de un proyecto es muy recomendable contar con una guía de buenas prácticas la cual nos facilite redactar commits que sean claros y puedan ayudar a cualquier miembro del equipo, esto para evitar que a medida que un proyecto se prolonga, los mensajes de los commits de mi git se vuelven cada vez menos informativos y podemos encontrar mensajes como **ya funciona x parte* los cuales en ocasiones no son ni descriptivos y peor aún en ocasiones ni el *responsable** recuerda o sabe lo que generó😒.

Por lo que para poder llevar de la mejor forma un proyecto es recomendable que todos los miembros del equipo adopten un estándar que les permite la redacción de commits, con base a mi experiencia comparto las siguientes recomendaciones.

## Estructura
El mensaje de un commit se divide en 3 partes diferentes el **título, **el cuerpo* y pie* como se muestra en el siguiente ejemplo.

```git
[Titulo ] => Type : Subject

[Body]

[Pie]
```

Como se puede apreciar en la imagen anterior el título se conforma de dos partes las cuales son el tipo y del asunto del mensaje.


### Tipo

*➕ADD *: Se genera una nueva funcionalidad.
*🛠 FIX *: Se soluciona un bug.
♻️ REFACTOR : Refactorización y mejoras.
☠️ DELETE : Se eliminan funciones o archivos.
📚 DOCS : Se generar cambios en la documentación.

Es importante notar que el Type se escribe en mayúsculas y se puede utilizar emoji el cual es opcional en mi caso los utilizo ya que me facilita de primera vista saber el tipo de commit.

### Subject/Asunto

El asunto no debe contener más de 50 caracteres, debe iniciar con una letra mayúscula y no terminar con un punto. Debemos ser imperativos al momento de redactar nuestro commit, es decir, hay que ser objetivos y muy importante tenemos que acostumbrarnos a escribirlos en Inglés esto es una de las mejores prácticas que podemos tener.


### Body/Cuerpo

Se utiliza para explicar el ¿Qué? y ¿Por qué? del commit y no el ¿Cómo?, Al escribir el cuerpo, requerimos de una línea en blanco entre el título y el cuerpo, además debemos limitar la longitud de cada línea a no más de 72 caracteres.

### Footer/Pie

Esta parte es muy importante ya que es donde se coloca el seguimiento de los **issues *o** tickets ***relacionados con los cambios generados.

### Ejemplo

Tomando en cuenta las recomendaciones mencionadas la estructura de nuestro commit se vería de la siguiente manera.

```bash
DOCS: Redaccion de reglas para commits
Een la seleccion Wiki se redactaron las buenas practicas para los commits

Issue: #1
```




[https://dev.to/konami12/recomendaciones-para-generar-un-buen-commit-544i#:~:text=%F0%9F%9A%A7%20Estructura,y%20del%20asunto%20del%20mensaje.]

---

### Otra Manera

_Type/Tipo_

El tipo es contenido en el titulo y puede ser de alguno de los siguientes casos:

`eat`: Una nueva caracteristica.

`fix`: Se soluciono un bug.

`docs`: Se realizaron cambios en la documentacion.

`style`: Se aplico formato, comas y puntos faltantes, etc; Sin cambios en el codigo.

`refactor`: Refactorizacion del codigo en produccion.

`test`: Se añadieron pruebas, refactorizacion de pruebas; Sin cambios en el codigo.

`chore`: Actualizacion de tareas de build, configuracion del admin. de paquetes; Sin cambios en el codigo.


### Ejemplo

```bash
feat: Summarize changes in around 50 characters or less

More detailed explanatory text, if necessary. Wrap it to about 72 
characters or so. In some contexts, the first line is treated as the 
subject of the commit and the rest of the text as the body. 

The blank line separating the summary from the body is 
critical (unless you omit the body entirely); 
various tools like `log`, `shortlog` and `rebase` can get 
confused if you run the two together. 

Explain the problem that this commit is solving. 
Focus on why you are making this change as oppose
to how (the code explains that). 

Are there side effects or other unintuitive consequenses of this change?
Here's the place to explain them.
Further paragraphs come after blank lines.

- Bullet points are okay, too 
- Typically a hyphen or asterisk is used for the bullet, preceded by a 
single space, with blank lines in between, but conventions vary here

If you use an issue tracker, put references to them at the bottom, like this:

Resolves: #123 
See also: #456, #789
```

[https://codigofacilito.com/articulos/buenas-practicas-en-commits-de-git]

---

_PLatilla_

```bash

Resumen de los cambios en 50 caracteres o menos

Texto explicativo más detallado, solo si es necesario. La línea en blanco que separa el título del resto del texto es crucial (a no ser que omitas el cuerpo y el mensaje solo tenga título); algunas herramientas pueden mostrar información alterada si omites la línea en blanco de separación.

También se pueden añadir más párrafos, separados igualmente por una línea en blanco.

- Se pueden añadir listas

- Para las listas se usan guiones o asteriscos (como en Markdown)

En el pie, se pueden poner referencias a los IDs de los issue trackers, por ejemplo:

Resuelve: #193
Afecta a: #270, #286
```