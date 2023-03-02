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

## Reto 5
1. Añadir PropTypes a los componentes creados (se deben instalar: https://reactjs.org/docs/typechecking-with-proptypes.html)
2. 
    
    
Muchos éxitos :)
