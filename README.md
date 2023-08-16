# Proyecto Práctica DOM con JavaScript

Este proyecto tiene como objetivo principal practicar las operaciones básicas del DOM (Document Object Model) usando JavaScript. A través del código presentado, se crea una galería de imágenes de Pokémon, aprovechando las imágenes disponibles en la API de Pokémon.

## Descripción

Usando un bucle `for`, se crea una serie de elementos `div` que contienen una imagen de un Pokémon y una etiqueta que indica el número de ese Pokémon en la Pokedex. Luego, cada `div` se añade a un contenedor principal llamado `container`.

El proyecto utiliza la base de sprites de la PokeAPI para recuperar las imágenes.

### Estructura del código:

1. **Selección del contenedor principal**:
    ```javascript
    const container = document.querySelector('#container');
    ```

2. **Definición de la URL base**:
    La URL base es donde se alojan las imágenes de los Pokémon.
    ```javascript
    const baseURL =  'https://raw.githubusercontent.com/PokeAPI/sprites/master/sprites/pokemon/';
    ```

3. **Bucle para generar elementos**:
    Se crea un bucle que itera 299 veces (para obtener imágenes de 299 Pokémon diferentes).
    Dentro de este bucle, se hace lo siguiente para cada iteración:
    - Crear un `div` para el Pokémon.
    - Agregar una clase de estilo al `div`.
    - Crear una etiqueta `span` para mostrar el número del Pokémon.
    - Crear un elemento de imagen `img` y asignarle la URL correspondiente.
    - Agregar la imagen y la etiqueta al `div`.
    - Finalmente, añadir el `div` al contenedor principal.
    ```javascript
    for( let i = 1; i < 300; i++ ){
        const pokemon = document.createElement('div');
        // ... (resto del código)
    }
    ```

## Cómo utilizar:

1. Asegúrese de tener un contenedor en su archivo HTML con el ID `container`.
2. Incorpore este script en su proyecto.
3. Ejecute su página web y debería ver una galería de imágenes de Pokémon con etiquetas numéricas.

## Conclusión:

Este proyecto sirve como una excelente práctica para aquellos que buscan entender y practicar las operaciones del DOM con JavaScript, así como también la integración y utilización de recursos externos a través de URLs.