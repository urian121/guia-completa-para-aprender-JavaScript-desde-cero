# Lista de Métodos más usados en JavaScript 🥇

#### Esta es tu guía definitiva para comprender todos los **Métodos de JavaScript** más usados. Desde las nociones básicas hasta los temas más complejos, explorarás una amplia variedad de ejemplos y respuestas diseñadas para ayudarte a dominar este poderoso lenguaje de programación. Ya sea que estés comenzando tu viaje en el desarrollo web o buscando ampliar tus conocimientos, esta guía te proporcionará la información necesaria para convertirte en un experto en JavaScript.


![Guia completa de JavaScript](https://raw.githubusercontent.com/urian121/imagenes-proyectos-github/master/guia-completa-para-dominar-javascript.png)


## Los métodos en JavaScript
**Los métodos en JavaScript** son funciones integradas que nos permiten realizar acciones específicas en distintos tipos de datos, **como cadenas, arrays, objetos, etc.** Son fundamentales para manipular y transformar información de manera eficiente. Entender y dominar los métodos más comunes es clave para trabajar de manera productiva en JavaScript, ya que simplifican tareas complejas y optimizan el desarrollo.

## ¿Qué es un método en JavaScript? 
En el mundo de la programación, un método es una función que pertenece a una clase específica. Cuando se trata de JavaScript, un método es una función puesta en un objeto o una serie de instrucciones para completar una tarea única.

## Introducción a Bucles y Estructuras de Control

#### 1. Bucle `for`
El bucle for permite iterar sobre un array. Aquí recorremos el array letras e imprimimos cada elemento.

```javascript
    const letras = ['a', 'b', 'c', 'd'];

    for (let i = 0; i < letras.length; i++) {
        console.log(letras[i]); 
        // Imprime cada letra del array
    }
```

#### 2. Bucle `for...in`

El bucle `for...in` permite iterar sobre las propiedades enumerables de un objeto. En cada iteración, accede a una propiedad del objeto y muestra su nombre y valor correspondiente en la consola.

```javascript
    // Definición de un objeto
    const objeto = { a: 1, b: 2, c: 3 };

    // Iteración sobre las propiedades del objeto
    for (let propiedad in objeto) {
        console.log(propiedad + ': ' + objeto[propiedad]); 
        // Imprime el nombre y valor de cada propiedad
    }
```


#### 3. Bucle `while`

Usando el bucle `while` para imprimir los números del 0 al 4 en la consola. El bucle se ejecuta mientras el contador sea menor que 5, incrementando el contador en cada iteración.

```javascript
    let contador = 0;
    while (contador < 5) {
        console.log(contador);
        contador++;
    }
```

## Manipulación de Arrays

#### 1. Métodos `forEach`

Cómo usar el método `forEach()` en un array en JavaScript para recorrer cada elemento del array y realizar una acción específica, en este caso, imprimir cada fruta en la consola.

```javascript
    let frutas = ["manzana", "banana", "pera"];

    // Recorrer cada elemento del array e imprimirlo
    frutas.forEach(function(fruta) {
        console.log(fruta);
    });

    // Añadir un elemento al arreglo
    frutas.push("naranja");

    // Eliminar el último elemento del arreglo
    frutas.pop();
```

#### 2. Método `map()`

El método `map()` en JavaScript se utiliza para aplicar una función a cada elemento del array `numeros`. Se duplica cada número del array original, resultando en la impresión del nuevo array `[2, 4, 6]`.

```javascript
    let numeros = [1, 2, 3];
    // Aplicar una función a cada elemento del arreglo
    let duplicados = numeros.map(numero => numero * 2);
    console.log(duplicados);
    // Imprime: [2, 4, 6]
```

#### 3. Método `filter()`

El método `filter()` en JavaScript se utiliza para filtrar los elementos de un array según una condición. 

1. Filtrar los números impares del array `numeros`, resultando en la impresión del nuevo array `[1, 3, 5]`.

```javascript
    let numeros = [1, 2, 3, 4, 5];
    // Filtrar elementos de un arreglo
    let impares = numeros.filter(numero => numero % 2 !== 0);
    console.log(impares);
    // Imprime: [1, 3, 5]
```

2. Retornar solo el elemento "manzana" que existe en el array frutas

```javascript
    const frutas = ["manzana", "banana", "pera", "uva"];
    // Filtrar las ocurrencias de "manzana" en el array de frutas
    const manzanas = frutas.filter(fruta => fruta === "manzana");
    console.log(manzanas);
    // Resultado: ["manzana"]
```

3. Retornar todos los elementos del array excepto "pera".

```javascript
    // Filtrar todas las frutas excepto "pera"
    const frutasExceptoPera = frutas.filter(fruta => fruta !== "pera");
    console.log(frutasExceptoPera);
    // Resultado: ["manzana", "banana", "uva"]
```

#### 4. Método `reduce()`

El método `reduce()` en JavaScript se utiliza para reducir un array a un único valor. En este caso, se suman todos los números del array `numeros` utilizando la función de reducción, comenzando con un valor inicial de 0, resultando en la impresión del valor total de 15.

```javascript
    let numeros = [1, 2, 3, 4, 5];
    // Reducir el arreglo a un único valor
    let suma = numeros.reduce((total, numero) => total + numero, 0);
    console.log(suma);
    // Imprime: 15
```

#### 5. Método `some()`

El método `some()` se utiliza en JavaScript para verificar si al menos un elemento de un array cumple con cierta condición especificada en una función de retorno. Itera sobre cada elemento del array y devuelve `true` si al menos un elemento cumple con la condición, y `false` si ningún elemento la cumple. Este método es útil cuando se desea verificar si al menos un elemento de un array satisface ciertos criterios sin necesidad de iterar manualmente.

```javascript
    const numeros = [1, 2, 3, 4, 5];

    // Verificar si al menos un número es mayor que 3
    const resultado = numeros.some(numero => numero > 3);

    console.log(resultado);
    // Resultado: true, ya que 4 y 5 son mayores que 3
```

#### 6. Método `every()`

El método `every()` se utiliza en JavaScript para verificar si todos los elementos de un array cumplen con cierta condición especificada en una función de retorno. Itera sobre cada elemento del array y devuelve `true` si todos los elementos cumplen con la condición, o `false` en caso contrario. Este método es útil cuando se desea verificar si todos los elementos de un array satisfacen ciertos criterios.

```javascript
    const numeros = [1, 2, 3, 4, 5];

    // Verificar si todos los números son mayores que 0
    const todosMayoresQueCero = numeros.every(numero => numero > 0);

    console.log(todosMayoresQueCero); 
    // Resultado: true, ya que todos los números son mayores que 0
```

#### 7. Método `find()`

El método `find()` se utiliza en JavaScript para encontrar el primer elemento en un array que cumple con cierta condición especificada en una función de retorno. Itera sobre cada elemento del array y devuelve el primer elemento que cumple con la condición, o `undefined` si ningún elemento la cumple. Este método es útil cuando se desea encontrar un elemento específico en un array basado en ciertos criterios.

```javascript
    const numeros = [1, 2, 3, 4, 5];

    // Encontrar el primer número mayor que 3
    const encontrado = numeros.find(numero => numero > 3);

    console.log(encontrado); 
    // Resultado: 4, ya que es el primer número mayor que 3
```


#### 8. Método `findIndex()`

El método findIndex() en JavaScript se usa para encontrar el índice del primer elemento en un array que cumple con una condición específica. El método devuelve -1 si no se encuentra ningún elemento que cumpla con la condición.

```javascript
    const numeros = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10];

    // Encontrar el índice del primer número par
    const indice = numeros.findIndex(numero => numero % 2 === 0);

    console.log(indice);
    // Salida: 1

    // Otro ejemplo del Método findIndex()
    const indice2 = numeros.findIndex(numero => numero > 5);

    console.log(indice2);
    // Salida: 5
```

#### 9. Método `indexOf()`

Cómo utilizar el método `indexOf()` en JavaScript para encontrar la posición de una palabra específica dentro de una cadena de texto. En este caso, se busca la palabra `"perro"` dentro de la frase `"El perro come comida"`, y se imprime la posición de la palabra encontrada.

```javascript
    let frase = "El perro come comida";
    // Encontrar la posición de una palabra en la frase
    console.log(frase.indexOf("perro")); 
    // Imprime: 3
```

#### 10. Método `slice()`

El método `slice()` en JavaScript permite extraer una parte específica de una cadena de texto. Se especifica el índice inicial (0) y el índice final (10) de la porción que se desea extraer de la cadena `"JavaScript es divertido"`, lo que resulta en la impresión de `"JavaScript"`.

```javascript
    let frase = "JavaScript es divertido";
    // Extraer una parte de la cadena
    console.log(frase.slice(0, 10));
    // Imprime: JavaScript
```

#### 11. Método `concat()`

El método `concat()` se utiliza para concatenar dos o más arrays en uno nuevo.

```javascript
    const array1 = [1, 2, 3];
    const array2 = [4, 5, 6];
    const array3 = [7, 8, 9];

    // Concatenar los tres arrays en uno nuevo
    const newArray = array1.concat(array2, array3);

    console.log(newArray);
    // Resultado: [1, 2, 3, 4, 5, 6, 7, 8, 9]
```

#### 12. El método `push()`

El método `push()` agrega uno o más elementos al final de un array y devuelve la nueva longitud del array. Modifica el array original.

```javascript
    // Declarar un array de frutas
    let frutas = ["uva", "manzana", "banana", "naranja"];

    // Agregar un elemento al final del array
    frutas.push("sandía");

    console.log("Fruta agregada al final del array:", frutas); 
    // Resultado: ["uva", "manzana", "banana", "naranja", "sandía"]
```

#### 14. Método `pop()`

El método `pop()` en JavaScript se utiliza para eliminar el último elemento de un array. En este caso, se elimina el número `3` del array `numeros`, resultando en la impresión del nuevo array `[1, 2]`.

```javascript
    let numeros = [1, 2, 3];
    // Eliminar el último elemento del arreglo
    numeros.pop();
    console.log(numeros);
    // Imprime: [1, 2]
```


#### 15. Método `shift()`

El método `shift()` en JavaScript se utiliza para eliminar el primer elemento de un array. En este caso, se elimina el número `1` del array `numeros`, resultando en la impresión del nuevo array `[2, 3]`.

```javascript
    let numeros = [1, 2, 3];
    // Eliminar el primer elemento del arreglo
    numeros.shift();
    console.log(numeros);
    // Imprime: [2, 3]
```


#### 16. Método `unshift()`

El método `unshift()` en JavaScript se utiliza para añadir un elemento al inicio de un array. En este caso, se agrega el número `1` al array `numeros`, resultando en la impresión del nuevo array `[1, 2, 3]`.

```javascript
    let numeros = [2, 3];
    // Añadir un elemento al inicio del arreglo
    numeros.unshift(1);
    console.log(numeros);
    // Imprime: [1, 2, 3]
```

#### 17. Método `splice()`

El método `splice()` modifica el contenido de un array eliminando o reemplazando elementos existentes y/o agregando nuevos elementos en su lugar. En este caso, se utiliza `splice()` para eliminar un elemento específico del array.

```javascript
    let array = [1, 2, 3, 4, 5];
    const indiceAEliminar = 2; 
    // Índice del elemento a eliminar

    // Eliminar el elemento en el índice especificado
    array.splice(indiceAEliminar, 1);

    console.log(array); 
    // Resultado: [1, 2, 4, 5]
```

#### 18. Método `reverse()`

El método `reverse()` en JavaScript se utiliza para invertir el orden de los elementos en un array. Los números en el array `numeros` se invierten, resultando en la impresión del nuevo array `[3, 2, 1]`.

```javascript
    let numeros = [1, 2, 3];
    // Invertir el orden de los elementos en el arreglo
    numeros.reverse();
    console.log(numeros);
    // Imprime: [3, 2, 1]
```

#### 17. Método `sort()`

El método `sort()` en JavaScript se utiliza para ordenar los elementos de un array alfabéticamente. En este caso, se ordenan las frutas en el array `frutas`, resultando en la impresión del nuevo array `["manzana", "naranja", "uva"]`.

```javascript
    let frutas = ["naranja", "manzana", "uva"];
    // Ordenar elementos de un arreglo
    frutas.sort();
    console.log(frutas);
    // Imprime: ["manzana", "naranja", "uva"]
```

#### 18. Método `includes()`

El método `includes()` en JavaScript se utiliza para verificar si un elemento está presente en un array. En este caso, se verifica si el número `2` está presente en el array `numeros`, lo que imprime `true`, y se verifica si el número `4` está presente, lo que imprime `false`.

```javascript
    let numeros = [1, 2, 3];
    // Verificar si un elemento está en el arreglo
    console.log(numeros.includes(2)); // Imprime: true
    console.log(numeros.includes(4)); // Imprime: false
```

#### 19. Método `join()`

El método `join()` en JavaScript permite combinar los elementos de un array en una cadena de texto. Los elementos del array `frutas` se unen utilizando `", "` como separador, lo que resulta en la impresión de la cadena `"manzana, naranja, uva"`.

```javascript
    let frutas = ["manzana", "naranja", "uva"];
    // Unir elementos de un arreglo en una cadena
    let lista = frutas.join(", ");
    console.log(lista);
    // Imprime: manzana, naranja, uva
```

## Manipulación de Cadenas (Strings)

#### 20. Método `replace()`

El método `replace()` en JavaScript permite reemplazar una parte específica de una cadena de texto. Se busca la palabra `"divertido"` en la frase `"Aprender es divertido"` y se reemplaza por `"genial"`, lo que resulta en la impresión de `"Aprender es genial"`.

```javascript
    let frase = "Aprender es divertido";
    // Reemplazar parte de la cadena
    console.log(frase.replace("divertido", "genial"));
    // Imprime: Aprender es genial
```

#### 21. Método `split()`

El método `split()` en JavaScript permite dividir una cadena de texto en un array. La cadena original `"manzana,naranja,uva"` se divide en tres elementos del array `["manzana", "naranja", "uva"]` utilizando la coma como separador.

```javascript
    let lista = "manzana,naranja,uva";
    // Dividir una cadena en un arreglo
    let frutas = lista.split(",");
    console.log(frutas);
    // Imprime: ["manzana", "naranja", "uva"]
```

## Objetos y Métodos de Objetos

#### 22. El método `toString()`

El método `toString()` devuelve una cadena de caracteres representando el array especificado y sus elementos.

```javascript
    const array1 = [1, 2, 'a', 'HTML'];

    console.log(array1.toString());
    // Resultado: "1,2,a,HTML"
```

#### 23. Anular el método `toString()`

Es posible anular el método toString() en un objeto para proporcionar una representación de cadena personalizada.

```javascript
    let persona = {
        nombre: "Juan",
        edad: 25,
        toString: function() {
            return this.nombre + " (" + this.edad + " años)";
        }
    };

    let cadena = persona.toString();

    console.log(cadena);
    // Salida: "Juan (25 años)"
```

#### 24. Método `values()`

El método values() en JavaScript se usa para obtener un array con los valores de las propiedades enumerables de un objeto. El orden de los valores en el array es el mismo que el orden de las propiedades en el objeto.

```javascript
    const persona = {
        nombre: "Juan",
        edad: 25,
        ciudad: "Bogotá"
    };

    const valores = Object.values(persona);

    console.log(valores);
    // Salida: ["Juan", 25, "Bogotá"]
```

#### 25. Objetos

La creación de un objeto `persona` en JavaScript con propiedades como `nombre` y `edad`, así como un método `saludar()` que imprime un saludo personalizado utilizando las propiedades del objeto.

```javascript
    let persona = {
        nombre: "Juan",
        edad: 30,
        saludar: function() {
            console.log("Hola, soy " + this.nombre + " y tengo " + this.edad + " años.");
        }
    };

    // Acceder a las propiedades y métodos del objeto
    console.log(persona.nombre); // Imprime: Juan
    persona.saludar(); 
    // Imprime: Hola, soy Juan y tengo 30 años.
```

## Temporizadores y Métodos de Tiempo

#### 26. setTimeout()

Se utiliza para ejecutar una función después de que haya transcurrido un tiempo específico (en milisegundos).

Se define una función llamada `saludar()` que simplemente imprime en la consola el mensaje '¡Hola después de 2 segundos!'. Luego, se llama a la función `setTimeout()` con dos argumentos: la función `saludar` que se ejecutará después de que haya transcurrido el tiempo especificado, y el tiempo en milisegundos (en este caso, 2000 milisegundos, es decir, 2 segundos).

```javascript
    // Función que se ejecutará después de 2 segundos
    function saludar() {
        console.log('¡Hola después de 2 segundos!');
    }

    // Llamar a la función después de 2 segundos
    setTimeout(saludar, 2000);
```

#### 27. setInterval()

se utiliza para ejecutar una función repetidamente, cada cierto intervalo de tiempo especificado (en milisegundos)

Se define una función llamada `mostrarMensaje()` que imprime en la consola el mensaje 'Mensaje repetido cada segundo'. Luego, se llama a la función `setInterval()` con dos argumentos: la función `mostrarMensaje` que se ejecutará repetidamente, y el intervalo de tiempo en milisegundos (en este caso, 1000 milisegundos, es decir, 1 segundo).

```javascript
    // Función que se ejecutará cada segundo
    function mostrarMensaje() {
        console.log('Mensaje repetido cada segundo');
    }

    // Llamar a la función cada segundo
    setInterval(mostrarMensaje, 1000);
```

## Solicitudes HTTP y Promesas

#### 28. Método `fetch`

Cómo realizar una solicitud HTTP utilizando el método `fetch()` en JavaScript. Se realiza una solicitud a la URL especificada y se encadenan promesas para manejar la respuesta. En el primer `then()`, se verifica si la respuesta es exitosa y se parsea la respuesta como JSON. En el segundo `then()`, se manipulan los datos obtenidos. En el `catch()`, se manejan los errores que puedan ocurrir durante la solicitud.

```javascript
    // URL a la que haremos la solicitud
    const url = 'https://jsonplaceholder.typicode.com/posts/1';

    // Realizar la solicitud utilizando fetch
    fetch(url)
        .then(response => {
            // Verificar si la respuesta es exitosa
            if (!response.ok) {
                throw new Error('No se pudo obtener la respuesta');
            }
            // Parsear la respuesta como JSON
            return response.json();
        })
        .then(data => {
            // Manipular los datos obtenidos
            console.log(data);
        })
        .catch(error => {
            // Manejar errores
            console.error('Error:', error);
        });
```

#### 29. Método fetch usando `async/await` y `try/catch`

Se utiliza `async/await` y `try/catch` para realizar una solicitud HTTP utilizando el método `fetch()` en JavaScript. La función `obtenerDatos()` se declara como asíncrona (`async`), lo que permite utilizar `await` dentro de ella. Dentro del bloque `try`, se realiza la solicitud a la API y se manejan los errores utilizando `throw` y `catch`. Si la solicitud es exitosa, se convierte la respuesta a formato JSON y se imprimen los datos obtenidos. Si hay algún error durante la ejecución, se captura en el bloque `catch` y se imprime el mensaje de error correspondiente. Esto proporciona una forma más concisa y legible de trabajar con solicitudes HTTP asincrónicas en JavaScript.

```javascript
    async function obtenerDatos() {
        try {
            // Hacer la solicitud a la API usando fetch
            const respuesta = await fetch('https://jsonplaceholder.typicode.com/posts/1');

            // Verificar si la respuesta es exitosa
            if (!respuesta.ok) {
                throw new Error('No se pudo obtener la respuesta');
            }

            // Convertir la respuesta a formato JSON
            const datos = await respuesta.json();

            // Imprimir los datos obtenidos
            console.log('Datos:', datos);
        } catch (error) {
            // Manejar errores
            console.error('Error:', error.message);
        }
    }

    // Llamar a la función para obtener los datos
    obtenerDatos();
```

#### 30. Usando `Axios` para hacer una solicitud HTTP de tipo (GET)

Se utiliza la biblioteca Axios para realizar una solicitud HTTP de tipo GET en JavaScript. Se declara una función asincrónica `obtenerDatos()` que utiliza `async/await` y `try/catch` para manejar la solicitud y cualquier error que pueda ocurrir. Dentro del bloque `try`, se utiliza `axios.get()` para hacer la solicitud a la URL especificada. Si la solicitud es exitosa, se imprime la respuesta en la consola. Si hay algún error durante la ejecución, se captura en el bloque `catch` y se imprime el mensaje de error correspondiente. Axios es una biblioteca popular para realizar solicitudes HTTP en JavaScript debido a su facilidad de uso y soporte para promesas y async/await.

```javascript
    // Asegúrate de haber importado Axios antes de usarlo
    // import axios from 'axios';

    async function obtenerDatos() {
        try {
            // Hacer la solicitud a la API usando Axios
            const respuesta = await axios.get('https://jsonplaceholder.typicode.com/posts/1');

            // Imprimir los datos obtenidos
            console.log('Datos:', respuesta.data);
        } catch (error) {
            // Manejar errores
            console.error('Error:', error.message);
        }
    }

    // Llamar a la función para obtener los datos
    obtenerDatos();
```


### Expresiones de Gratitud 🎁

    Comenta a otros sobre este proyecto 📢
    Invita una cerveza 🍺 o un café ☕
    Paypal iamdeveloper86@gmail.com
    Da las gracias públicamente 🤓.

## No olvides SUSCRIBIRTE 👍
