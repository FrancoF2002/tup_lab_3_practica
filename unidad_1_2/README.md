# Unidad 1.2 - Lógica de componentes - Práctica


## Pre-requisitos



* Tener instalados node y create-react-app localmente
* Un editor de código (VSCode recomendado)
* Inicializar el código de la actividad con el siguiente comando:


```
npx create-react-app unidad1.2-apellido_nombre_alumno
```


Considerando el siguiente objeto de JavaScript:


```
const site = {
  pageTitle: 'Unidad 1.2 - Práctica',
  pageBody: 'Implementación de árbol de componentes y propiedades en React.'
}
```



### Tarea 1



* Crear la carpeta `components` dentro de `src` 
* Crear el componente `Title` que reciba como parámetro la propiedad `pageTitle` y la renderice dentro de una etiqueta de encabezado (`h1`).
* Crear el componente `Body` que reciba como parámetro la propiedad `pageBody` y la renderice dentro de una etiqueta `div`
* Importar los componentes `Title` y `Body` desde `App.js` y renderizarlos pasándose como propiedades sus respectivos valores de la constante `site`. 
* Bonus: utilizar `object destructuring` para leer las propiedades pasadas a los componentes como argumentos


### Tarea 2: 



* Crear el componente `Header` que importará el componente `Title` y recibirá como propiedad `pageTitle`
* Crear el componente `Main` que importará el componente `Body` y recibirá como propiedad `pageBody` y además renderizar una lista de menú (`navbar` y `ul`) con enlaces a 2 sitios web externos.
* Refactorizar App para utilizar los componente `Main` y `Header`
* Bonus: Enviar los enlaces a sitio web externos como `props` enviadas a `Main`


### Tarea 3

* Crear un componente `Page` de forma que acepte hijos (children) y los renderice de esa forma a los componente `Main` y `Header`
* Refactorizar `App` para que importe y renderice `Page`, recordar enviarle que la constante site debe estar definida en `App` y enviarla a los distintos componentes via `props`.
* En el componente `Main` modificar el contenido de la página agregando una frase a elección del alumno.


<<<<<<< HEAD
* Crear un componente `Page` de forma que acepte hijos (children) y los renderice de esa forma a `Main` y `Header`
* Refactorizar `App` para que importe y renderice `Page`, recordar enviarle que la constante site debe estar definida en `App` y enviarla a los distintos componentes via `props`.
* En el componente `Main` modificar el contenido de la página agregando una frase a elección del alumno.

=======
>>>>>>> e2457ec3db1d408f5849700ef82927c5d42de70b
### Tarea 4 - Reutilización de componentes

* Refactorizar las propiedades `pageTitle` y `pageBody` de `Title` y `Body` respectivamente para que llamen `title` y `body`
* Crear un componente `BlogPost` que renderice los componentes `Title` y `Body` pasando como paramétros `title` y `body` los datos de una noticia del diario seleccionada a la azar. Colocar `BlogPost` dentro de `Main` a continuación del `Body` 
* Realizar lo necesario para que el título de la página situado en `Header` se vea en mayúsculas mientras que el título del `BlogPost` se vea normal.
* Realizar lo necesario para que el body de la página situado en `Main` se vea en mayúsculas en italics  mientras que el body del `BlogPost` se vea normal.
BONUS: Utilizar CSS para agregar alguna diferenciación extra