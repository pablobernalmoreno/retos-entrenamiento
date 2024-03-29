# retos-entrenamiento

Para cada reto crear una rama distinta a la rama "main" que siga la siguiente nomenclatura: feature/x donde x será UX_Name (para cambios únicamente visuales) o L_Name (para cambios de funcionalidades o lógica)

## Reto #1
1. Crear un repositorio usando el comando de "create-react-app" (https://create-react-app.dev/docs/getting-started) 
2. Crear los siguientes componentes: Titulo, Barra de busqueda y Botón submit, para que estén posicionados y estilizados de esta forma: ![image](https://user-images.githubusercontent.com/26677733/218548015-1f9cc937-72b6-4930-a1df-5f4e7ed6de39.png)

Para los componentes se pueden crear usando HTML vanilla o frameworks de componentes como material-ui (https://v4.mui.com/), bootstrap (https://getbootstrap.com/) o el que más disfruten!

## Reto #2
1. Para el estilizado de la app podemos implementar varias alternativas, como opciones se proponen las siguientes 
    1. styled-components (https://styled-components.com/) 
    2. Styled de material ui (https://mui.com/system/styled/) la elección es libre
3. Crear una barra de navegación, la cual debe cumplir el siguiente esquema:
    1. Botón drawer (para abrir opciones extras)
    2. Botón perfil
    3. Botón para cambiar el tema (light/dark)
    4. La barra de busqueda y el botón de busqueda del reto anterior deben estar en esta barra de navegación
    5. La barra de navegación debe tener de estilo position: sticky (https://developer.mozilla.org/en-US/docs/Web/CSS/position)
4. Elegir BaaS para implementar. Puede ser el que más les guste, como opciones se proponen las siguientes:
    1. SupaBase (https://supabase.com/)
    2. PocketBase (https://pocketbase.io/)
    
## Reto #3
1. Crear las cartas donde se muestren los juegos (objetos) en venta, el estilizado es libre pero deben tener los siguientes campos (Nombre juego, precio, cantidad en stock, imagen, descripción)
2. Llenar la base de datos con algunos elementos para que estos se muestren en la página
3. Implementar react-redux https://es.redux.js.org/ con todos sus componentes (store, reducer, actions y types)
4. El primer reducer a implementar y usar es el reducer para manejar el estado global de la aplicación para el tema (claro/oscuro)

## Reto #4
1. Añadir a la barra de navegación un carrito de compra
2. Añadir a las cartas de juegos un botón para añadirlo al carrito
3. Añadir una badge al icono del carrito de compras para que se pueda saber cuántos articulos hay en este carrito
4. Añadir un modal (puede ser usando react portals:https://reactjs.org/docs/portals.html o usando el dialog de material ui:https://mui.com/material-ui/react-dialog/) al carrito de compras en el cual se puedan ver los articulos del carrito (en una versión más pequeña donde solo haya nombre y depronto imagen)
5. Añadir también dos botones, "view details" y un botón para eliminar el elemento, la funcionalidad de view details entrará en otro reto, pero si implementar la funcionalidad de borrar elementos

## Reto #5
1. Añadir PropTypes a los componentes creados (se deben instalar: https://reactjs.org/docs/typechecking-with-proptypes.html)
2. Añadir JSDoc https://www.inkoop.io/blog/a-guide-to-js-docs-for-react-js/
    
## Reto #6 
Vamos a implementar react router(https://reactrouter.com/en/main), para eso haremos lo siguiente:
1. Crear el router donde pondremos nuestras rutas, este router irá en App.js (puede estar directamente en App.js o exportarlo de otra parte)
2. Nuestra pantalla main va a ser la ruta default '/'
3. Crearemos otra ruta que se llame 'game/:gameId' donde se mostraran datos de cada juego, siendo gameId el id del juego dentro de nuestra DB

## Reto #7
Vamos a implementar custom hooks para la llamada de las apis: https://es.reactjs.org/docs/hooks-custom.html

## Reto #8
En este reto vamos a estilizar la página de cada juego que creamos en el reto #6, en este reto vamos a tener libertad creativa pero si quiero que muestre las siguientes cosas:
1. Imagen del juego grande
2. Nombre del juego
3. Descripción de cada juego
4. Cantidad en stock
5. Precio
6. Tags (añadir tags a cada juego)
7. Comentarios de los usuarios (por ahora populados manualmente)

## Reto #9
Para este reto vamos a crear otra ruta para los tags, entonces cada tag va a tener su propia ruta "/tags/:tag", acá mostraremos todos los juegos que contengan dicho tag. También hay que tener cuidado con las rutas anidadas ya que de la página "tags/:tag" podemos ir a la página de cada juego "games/:game" y no es lo mismo "home/game/:game" que "home/tags/:tag/game/:game"

## Reto 10
En este reto crearemos por fin la funcionalidad de "búsqueda de juego" en este haremos que al darle submit al botón de búsqueda con el nombre de algún juego, nos lleve a la página de este, por lo que tendremos que buscar el id del juego solo con el nombre de este y al hacer match, llevarlo a la página que es, si el nombre está mal o no se encuentra, llevarlo a la página de error.
Como bonus del reto, podemos implementar un "te refieres a" o algo por el estilo para que en caso de que el nombre buscado no exista o esté mal escrito, recomendarle al usuario algún juego similar (o algunos)

## Reto 11
En este reto vamos a implementar private routing, para esto crearemos primero una página de login para ir a esta página será dandole click al botón de "perfil" que tenemos en nuestra navbar, al estar ya logeados, vamos a usar el sistema de auth de pocketbase (en caso de usar otro CMS, buscar su sistema de auth) https://pocketbase.io/docs/authentication. Al tener todo esto, crearemos nuestra primer ruta privada, esta será para registrar un nuevo juego, entonces al estar registrados se cargara la página sin problema, en caso de no estar registrado, se debe redirigir al usuario a otra página (ya queda a criterio nuestro si es una página error o lo llevamos nuevamente al main page). En la página de registro de juego, crearemos un simple formulario donde llenaremos los campos básicos del juego que crearemos y así podemos hacer el POST

## Reto 12
Tristemente, create-react-app ha muerto, por lo que la documentación nos pide que utilicemos un framework, entonces antes de seguir con cualquier cosa, debemos migrar a un framework para evitar errores en el fúturo. Existen varios, pero los mayores a día de hoy son NextJs(https://nextjs.org/) y Gatsby(https://www.gatsbyjs.com/)

Muchos éxitos :)
