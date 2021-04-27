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