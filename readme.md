# Todo lo que necesitas saber sobre JavaScript, La Guía completa de JavaScript desde Cero.🥇

#### Esta es tu guía definitiva para comprender los conceptos fundamentales y avanzados de JavaScript. Desde las nociones básicas hasta los temas más complejos, explorarás una amplia variedad de preguntas y respuestas diseñadas para ayudarte a dominar este poderoso lenguaje de programación. Ya sea que estés comenzando tu viaje en el desarrollo web o buscando ampliar tus conocimientos, esta guía te proporcionará la información necesaria para convertirte en un experto en JavaScript.

![Guia completa de JavaScript](https://raw.githubusercontent.com/urian121/imagenes-proyectos-github/master/guia-completa-de-javascript-desde-cero.png)width=100px height=100px



#### 1. Variables y Tipos de Datos

    // Declaración de variables
    let nombre = "Juan";
    const PI = 3.14;

    // Tipos de datos
    let numero = 10; // Número entero
    let decimal = 3.14; // Número decimal
    let texto = "Hola Mundo"; // Cadena de texto
    let esVerdadero = true; // Booleano
    let arreglo = [1, 2, 3, 4]; // Arreglo
    let objeto = { nombre: "Juan", edad: 30 }; // Objeto

#### 2. Funciones

##### La función saludar toma un parámetro nombre y muestra un saludo personalizado en la consola cuando se llama con un nombre específico

    // Definición de una función
    function saludar(nombre) {
    console.log("¡Hola, " + nombre + "!");
    }

    // Llamada a la función
    saludar("Juan"); // Imprime: ¡Hola, Juan!

#### 3. Condicionales

##### Utilizando la estructura condicional if...else para verificar si una variable edad es mayor o igual a 18. Dependiendo del resultado de la condición, se imprime un mensaje apropiado en la consola.

    let edad = 18;
    if (edad >= 18) {
        console.log("Eres mayor de edad");
    } else {
        console.log("Eres menor de edad");
    }

#### 4. Bucle For

##### cómo usar un bucle for en JavaScript para iterar sobre un array. El bucle recorre cada elemento del array e imprime su valor en la consola.

    const array = ['a', 'b', 'c', 'd'];

    for (let i = 0; i < array.length; i++) {
        console.log(array[i]);
    }

#### 5. Bucle for...in

##### Ilustrando el uso del bucle for...in en JavaScript para iterar sobre las propiedades de un objeto. En cada iteración, se accede a una propiedad del objeto y se imprime su nombre y valor correspondiente en la consola.

    const objeto = { a: 1, b: 2, c: 3 };

    for (let propiedad in objeto) {
        console.log(propiedad + ': ' + objeto[propiedad]);
    }

#### 6. Bucle while

##### Usando el bucle while para imprimir los números del 0 al 4 en la consola. El bucle se ejecuta mientras el contador sea menor que 5, incrementando el contador en cada iteración.

    let contador = 0;
    while (contador < 5) {
        console.log(contador);
        contador++;
    }

#### 7. Métodos forEach

##### Cómo usar el método forEach() en un array en JavaScript para recorrer cada elemento del array y realizar una acción específica, en este caso, imprimir cada fruta en la consola.

    let frutas = ["manzana", "banana", "pera"];
    frutas.forEach(function(fruta) {
        console.log(fruta);
    });

    // Añadir un elemento al arreglo
    frutas.push("naranja");

    // Eliminar el último elemento del arreglo
    frutas.pop();

#### 8. Objetos y Métodos de Objetos

##### la creación de un objeto persona en JavaScript con propiedades como nombre y edad, así como un método saludar() que imprime un saludo personalizado utilizando las propiedades del objeto.

    let persona = {
        nombre: "Juan",
        edad: 30,
        saludar: function() {
            console.log("Hola, soy " + this.nombre + " y tengo " + this.edad + " años.");
        }
    };

    // Acceder a las propiedades y métodos del objeto
    console.log(persona.nombre); // Imprime: Juan
    persona.saludar(); // Imprime: Hola, soy Juan y tengo 30 años.

#### 9. Métodos de Cadena de Texto

    let texto = "Hola Mundo";

    // Convertir a mayúsculas
    console.log(texto.toUpperCase());
    // Imprime: HOLA MUNDO

    // Convertir a minúsculas
    console.log(texto.toLowerCase());
    // Imprime: hola mundo

    // Obtener la longitud del texto
    console.log(texto.length);
    // Imprime: 10

#### 10. Método indexOf()

##### cómo utilizar el método indexOf() en JavaScript para encontrar la posición de una palabra específica dentro de una cadena de texto. En este caso, se busca la palabra "perro" dentro de la frase "El perro come comida", y se imprime la posición de la palabra encontrada, que es 3.

    let frase = "El perro come comida";
    // Encontrar la posición de una palabra en la frase
    console.log(frase.indexOf("perro"));
    // Imprime: 3

#### 11. Método slice()

##### El método slice() en JavaScript para extraer una parte específica de una cadena de texto. Se especifica el índice inicial (0) y el índice final (10) de la porción que se desea extraer de la cadena "JavaScript es divertido", lo que resulta en la impresión de "JavaScript".

    let frase = "JavaScript es divertido";
    // Extraer una parte de la cadena
    console.log(frase.slice(0, 10));
    // Imprime: JavaScript

#### 12. Método replace()

##### El método replace() en JavaScript para reemplazar una parte específica de una cadena de texto. Se busca la palabra "divertido" en la frase "Aprender es divertido" y se reemplaza por "genial", lo que resulta en la impresión de "Aprender es genial".

    let frase = "Aprender es divertido";
    // Reemplazar parte de la cadena
    console.log(frase.replace("divertido", "genial"));
    // Imprime: Aprender es genial

#### 13. Método split()

##### El método split() en JavaScript para dividir una cadena de texto en un array. La cadena original "manzana,naranja,uva" se divide en tres elementos del array ["manzana", "naranja", "uva"] utilizando la coma como separador.

    let lista = "manzana,naranja,uva";
    // Dividir una cadena en un arreglo
    let frutas = lista.split(",");
    console.log(frutas);
    // Imprime: ["manzana", "naranja", "uva"]

#### 14. Método join()

##### El método join() en JavaScript para combinar los elementos de un array en una cadena de texto. Los elementos del array frutas se unen utilizando ", " como separador, lo que resulta en la impresión de la cadena "manzana, naranja, uva".

    let frutas = ["manzana", "naranja", "uva"];
    // Unir elementos de un arreglo en una cadena
    let lista = frutas.join(", ");
    console.log(lista);
    // Imprime: manzana, naranja, uva

#### 15. Método push()

##### El método push() en JavaScript para añadir un elemento al final de un array. Se agrega el número 4 al array numeros, lo que resulta en la impresión del nuevo array [1, 2, 3, 4].

    let numeros = [1, 2, 3];
    // Añadir un elemento al final del arreglo
    numeros.push(4);
    console.log(numeros);
    // Imprime: [1, 2, 3, 4]

#### 16. Método pop()

##### El método pop() en JavaScript para eliminar el último elemento de un array. Se elimina el número 3 del array numeros, resultando en la impresión del nuevo array [1, 2].

    let numeros = [1, 2, 3];
    // Eliminar el último elemento del arreglo
    numeros.pop();
    console.log(numeros);
    // Imprime: [1, 2]

#### 17. Método shift()

##### El método shift() en JavaScript para eliminar el primer elemento de un array. Se elimina el número 1 del array numeros, lo que resulta en la impresión del nuevo array [2, 3].

    let numeros = [1, 2, 3];
    // Eliminar el primer elemento del arreglo
    numeros.shift();
    console.log(numeros);
    // Imprime: [2, 3]

#### 18. Método unshift()

##### El método unshift() en JavaScript para añadir un elemento al inicio de un array. Se agrega el número 1 al array numeros, resultando en la impresión del nuevo array [1, 2, 3].

    let numeros = [2, 3];
    // Añadir un elemento al inicio del arreglo
    numeros.unshift(1);
    console.log(numeros);
    // Imprime: [1, 2, 3]

#### 19. Método includes()

##### El método includes() en JavaScript para verificar si un elemento está presente en un array. Se verifica si el número 2 está presente en el array numeros, lo que imprime true, y se verifica si el número 4 está presente, lo que imprime false.

    let numeros = [1, 2, 3];
    // Verificar si un elemento está en el arreglo
    console.log(numeros.includes(2)); // Imprime: true
    console.log(numeros.includes(4)); // Imprime: false

#### 20. Método sort()

##### El método sort() en JavaScript para ordenar los elementos de un array alfabéticamente. Se ordenan las frutas en el array frutas, resultando en la impresión del nuevo array ["manzana", "naranja", "uva"].

    let frutas = ["naranja", "manzana", "uva"];
    // Ordenar elementos de un arreglo
    frutas.sort();
    console.log(frutas);
    // Imprime: ["manzana", "naranja", "uva"]

#### 21. Método reverse()

##### El método reverse() en JavaScript para invertir el orden de los elementos en un array. Los números en el array numeros se invierten, resultando en la impresión del nuevo array [3, 2, 1].

    let numeros = [1, 2, 3];
    // Invertir el orden de los elementos en el arreglo
    numeros.reverse();
    console.log(numeros);
    // Imprime: [3, 2, 1]

#### 22. Método map()

##### El método map() en JavaScript para aplicar una función a cada elemento del array numeros. Se duplica cada número del array original, resultando en la impresión del nuevo array [2, 4, 6].

    let numeros = [1, 2, 3];
    // Aplicar una función a cada elemento del arreglo
    let duplicados = numeros.map(numero => numero * 2);
    console.log(duplicados);
    // Imprime: [2, 4, 6]

#### 23. Método filter()

##### El método filter() en JavaScript para filtrar los elementos de un array numeros. Se filtran los números impares del array original, resultando en la impresión del nuevo array [1, 3, 5].

    let numeros = [1, 2, 3, 4, 5];
    // Filtrar elementos de un arreglo
    let impares = numeros.filter(numero => numero % 2 !== 0);
    console.log(impares);
    // Imprime: [1, 3, 5]

#### 24. Método reduce()

##### El método reduce() en JavaScript para reducir un array numeros a un único valor. Se suma todos los números del array utilizando la función de reducción, comenzando con un valor inicial de 0, lo que resulta en la impresión del valor total de 15.

    let numeros = [1, 2, 3, 4, 5];
    // Reducir el arreglo a un único valor
    let suma = numeros.reduce((total, numero) => total + numero, 0);
    console.log(suma);
    // Imprime: 15

#### 25. Funciones Flecha

##### Sintaxis de las funciones flecha en JavaScript, que proporcionan una forma más concisa de escribir funciones. Se compara una función normal suma() con una función flecha equivalente, ambas realizando la misma operación de suma de dos números a y b.

    // Función normal
    function suma(a, b) {
        return a + b;
    }

    // Función flecha
    let suma = (a, b) => a + b;

#### 26. Template String

##### El uso de template strings en JavaScript, que permiten incrustar variables y expresiones dentro de una cadena de texto utilizando ${}. Se imprime un saludo personalizado con el nombre y la edad de la persona, utilizando las variables nombre y edad.

    let nombre = "Juan";
    let edad = 30;

    // Uso de template strings
    console.log(`Hola, mi nombre es ${nombre} y tengo ${edad} años.`);

#### 27. Spread Operator

##### El uso del operador de propagación (spread operator) en JavaScript, que permite combinar múltiples arrays en uno solo de manera más concisa. Se combinan los arrays numeros y otrosNumeros en un nuevo array todosLosNumeros, lo que resulta en la impresión del array combinado [1, 2, 3, 4, 5, 6].

    let numeros = [1, 2, 3];
    let otrosNumeros = [4, 5, 6];

    // Combinar arreglos
    let todosLosNumeros = [...numeros, ...otrosNumeros];
    console.log(todosLosNumeros);
    // Imprime: [1, 2, 3, 4, 5, 6]

#### 28. Destructuring

##### El uso de la destructuración (destructuring) en JavaScript para extraer propiedades de un objeto de forma más concisa. Se extraen las propiedades nombre y edad del objeto persona, lo que permite acceder a estos valores de manera directa, resultando en la impresión de "Juan 30".

    let persona = { nombre: "Juan", edad: 30 };

    // Destructuring de objeto
    let { nombre, edad } = persona;
    console.log(nombre, edad);
    // Imprime: Juan 30

#### 29. Parámetros de función predeterminados

##### El uso de parámetros de función predeterminados en JavaScript. La función greet() tiene un parámetro name que tiene un valor predeterminado de "Urian". Si no se proporciona ningún argumento al llamar a la función, se utilizará el valor predeterminado "Urian".

        function greet(name = "Urian") {
            return `Hola, ${name}!`;
        }

#### 30. Operador Ternario

##### El operador ternario en JavaScript para asignar un valor a la variable mensaje basado en una condición. Si el precio es mayor que 50, el mensaje será "Caro", de lo contrario, será "Barato". En este caso, como el precio es 100, el mensaje impreso es "Caro".

    let precio = 100;
    let mensaje = precio > 50 ? "Caro" : "Barato";

    console.log(mensaje); // Imprime: Caro

#### 31. asignación de destructuración

##### Cómo realizar la asignación de destructuración en JavaScript para extraer propiedades específicas de un objeto. Se extraen las propiedades nombre, edad y ciudad del objeto persona, lo que permite acceder a estos valores de manera directa y utilizarlos en otras partes del código.

    // Objeto con información de una persona
    const persona = {
        nombre: 'Juan',
        edad: 30,
        ciudad: 'Madrid'
    };

    // Asignación de destructuración para extraer propiedades del objeto
    const { nombre, edad, ciudad } = persona;

    // Mostrar los valores extraídos
    console.log(nombre); // Imprime: Juan
    console.log(edad); // Imprime: 30
    console.log(ciudad); // Imprime: Madrid

#### 32. Operador de propagación para la clonación de objetos

##### Cómo clonar un objeto en JavaScript utilizando el operador de propagación (...). Se crea una copia del objeto personaOriginal llamada personaClon, lo que permite tener dos objetos independientes con las mismas propiedades y valores. Esto es útil para evitar mutaciones no deseadas en el objeto original.

    // Objeto original
    const personaOriginal = {
        nombre: 'Juan',
        edad: 30,
        ciudad: 'Madrid'
    };

    // Clonar el objeto utilizando el operador de propagación
    const personaClon = { ...personaOriginal };

    // Modificar una propiedad del objeto clonado
    personaClon.edad = 35;

    // Mostrar los objetos originales y clonados
    console.log('Objeto original:', personaOriginal);
    console.log('Objeto clonado:', personaClon);

#### 33. operador de encadenamiento opcional (?)

##### El uso del operador de encadenamiento opcional (?.) en JavaScript para acceder a una propiedad anidada de forma segura. Se intenta acceder al código postal (codigoPostal) dentro del objeto direccion del objeto usuario. Si direccion no está definido o es null o undefined, la expresión devolverá undefined en lugar de lanzar un error.

    // Objeto que puede contener propiedades anidadas
    const usuario = {
        nombre: 'Juan',
        direccion: {
            ciudad: 'Madrid',
            codigoPostal: 28001
        }
    };

    // Acceder a una propiedad anidada de forma segura utilizando el operador de encadenamiento opcional
    const codigoPostal = usuario.direccion?.codigoPostal;

    // Mostrar el código postal si está presente, de lo contrario, mostrar un mensaje predeterminado
    console.log('Código Postal:', codigoPostal ?? 'No disponible');

#### 34. Eliminar Elementos repetidos de un array utilizando new Set

##### El constructor Set. Se crea un nuevo Set a partir del array registros, que automáticamente elimina los elementos duplicados. Luego, se convierte el Set de nuevo en un array utilizando el operador de propagación (...) para obtener un array con registros únicos en registrosUnicos.

    // Array con registros repetidos
    const registros = [1, 2, 3, 1, 2, 4, 5, 3];

    // Eliminar registros repetidos utilizando Set
    const registrosUnicos = [...new Set(registros)];

    // Mostrar los registros únicos
    console.log(registrosUnicos); // Imprime: [1, 2, 3, 4, 5]

#### 35. Eliminar elementos repetidos de un Array usando filter y indexOf

##### Se filtran los elementos del array registros, conservando solo aquellos cuyo índice es igual a la primera aparición del elemento en el array, lo que resulta en un array con registros únicos en registrosUnicos.

    const registros = [1, 2, 3, 1, 2, 4, 5, 3];
    const registrosUnicos = registros.filter((valor, indice, arreglo) => arreglo.indexOf(valor) === indice);
    console.log(registrosUnicos); // Imprime: [1, 2, 3, 4, 5]

#### 36. Eliminar elementos repetidos de un Array usando filter y includes

##### Se filtran los elementos del array registros, conservando solo aquellos que no están repetidos en el array, lo que resulta en un array con registros únicos en registrosUnicos.

    const registros = [1, 2, 3, 1, 2, 4, 5, 3];
    const registrosUnicos = registros.filter((valor, indice, arreglo) => arreglo.includes(valor, indice + 1));
    console.log(registrosUnicos); // Imprime: [1, 2, 3, 4, 5]

#### 37. Eliminar elementos repetidos de un Array usando reduce

##### Se recorre el array registros, y para cada valor se verifica si ya está presente en el array de valores únicos (unicos). Si no está presente, se añade al array de valores únicos, de lo contrario se conserva el array actual. Esto resulta en un array con registros únicos en registrosUnicos.

    const registros = [1, 2, 3, 1, 2, 4, 5, 3];
    const registrosUnicos = registros.reduce((unicos, valor) => unicos.includes(valor) ? unicos : [...unicos, valor], []);
    console.log(registrosUnicos); // Imprime: [1, 2, 3, 4, 5]

#### 38. Asignación de valores predeterminados

##### Cómo asignar valores predeterminados a los parámetros de una función en JavaScript utilizando el operador de fusión nula (??). Si el argumento pasado a la función es null o undefined, se asigna el valor predeterminado 'Invitado'. Esto permite que la función se comporte correctamente incluso si no se proporcionan argumentos al llamarla.

    // Función que toma un nombre como argumento y lo imprime
    function saludar(nombre) {
        // Asignación de valor predeterminado usando el operador de fusión nula (??)
        nombre = nombre ?? 'Invitado';
        console.log(`Hola, ${nombre}!`);
    }

    // Llamada a la función sin argumento
    saludar(); // Imprime: Hola, Invitado!

    // Llamada a la función con un argumento
    saludar('Juan'); // Imprime: Hola, Juan!

#### 39. Verificar si un elemento existe en un array utilizando el método includes()

##### El método includes() en JavaScript para verificar si un elemento específico está presente en un array. Se verifica si el elemento 3 está presente en el array array, y se imprime un mensaje apropiado en la consola dependiendo del resultado. Si el elemento está presente, se imprime 'El elemento 3 está presente en el array', de lo contrario se imprime 'El elemento 3 no está presente en el array'

    const array = [1, 2, 3, 4, 5];

    // Verificar si el elemento 3 existe en el array
    if (array.includes(3)) {
        console.log('El elemento 3 está presente en el array');
    } else {
        console.log('El elemento 3 no está presente en el array');
    }

#### 40. Verificar si un elemento existe en un array utilizando el método indexOf()

##### El método indexOf() en JavaScript para verificar si un elemento específico está presente en un array. Se verifica si el elemento 3 está presente en el array array, y se imprime un mensaje apropiado en la consola dependiendo del resultado. Si el elemento está presente, se imprime 'El elemento 3 está presente en el array', de lo contrario se imprime 'El elemento 3 no está presente en el array'.

    const array = [1, 2, 3, 4, 5];

    // Verificar si el elemento 3 existe en el array
    if (array.indexOf(3) !== -1) {
        console.log('El elemento 3 está presente en el array');
    } else {
        console.log('El elemento 3 no está presente en el array');
    }

#### 41. Prevención de la modificación de objetos

##### Cómo prevenir la modificación de un objeto en JavaScript utilizando el método Object.freeze(). Al llamar a este método con el objeto persona como argumento, se congela el objeto, lo que significa que no se pueden agregar, eliminar o modificar propiedades existentes en el objeto. Esto ayuda a proteger el objeto persona de modificaciones no deseadas.

    // Objeto que queremos proteger de modificaciones
    const persona = {
        nombre: 'Juan',
        edad: 30
    };

    // Prevenir la modificación del objeto
    Object.freeze(persona);

    // Intentar modificar una propiedad del objeto
    persona.nombre = 'Pedro'; // No se producirá ningún cambio

    // Intentar añadir una nueva propiedad al objeto
    persona.ciudad = 'Madrid'; // No se añadirá la propiedad

    // Mostrar el objeto
    console.log(persona); // Imprimirá el objeto original sin cambios

#### 42. Callback, en JavaScript es una función que se pasa como argumento a otra función y que se ejecuta después de que alguna operación asincrónica o de larga duración haya finalizado.

##### La función hacerAlgoAsincrono() simula una operación asincrónica utilizando setTimeout(). Después de una demora de 2 segundos, ejecuta la función de callback manejarResultado() pasada como argumento. Esta función de callback maneja el resultado de la operación asincrónica, en este caso, simplemente imprime el mensaje "Resultado: Datos cargados" en la consola.

    // Función que simula una operación asincrónica
    function hacerAlgoAsincrono(callback) {
    // Simular una demora de 2 segundos (por ejemplo, cargar datos del servidor)
    setTimeout(function() {
        // Después de la demora, ejecutar la función de callback
        callback('Datos cargados');
    }, 2000);
    }

    // Función de callback que maneja el resultado
    function manejarResultado(resultado) {
        console.log('Resultado:', resultado);
    }

    // Llamar a la función asincrónica con el callback
    hacerAlgoAsincrono(manejarResultado);

#### 43. Método fetch

##### Cómo realizar una solicitud HTTP utilizando el método fetch() en JavaScript. Se realiza una solicitud a la URL especificada y se encadenan promesas para manejar la respuesta. En el primer then(), se verifica si la respuesta es exitosa y se parsea la respuesta como JSON. En el segundo then(), se manipulan los datos obtenidos. En el catch(), se manejan los errores que puedan ocurrir durante la solicitud.

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

#### 44. Método fetch usando async/await y try/catch

##### Se utiliza async/await y try/catch para realizar una solicitud HTTP utilizando el método fetch() en JavaScript. La función obtenerDatos() se declara como asíncrona (async), lo que permite utilizar await dentro de ella. Dentro del bloque try, se realiza la solicitud a la API y se manejan los errores utilizando throw y catch. Si la solicitud es exitosa, se convierte la respuesta a formato JSON y se imprimen los datos obtenidos. Si hay algún error durante la ejecución, se captura en el bloque catch y se imprime el mensaje de error correspondiente. Esto proporciona una forma más concisa y legible de trabajar con solicitudes HTTP asincrónicas en JavaScript.

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

#### 45. Usando Axios para hacer una solicitud HTTP de tipo (GET)

##### Se utiliza la biblioteca Axios para realizar una solicitud HTTP de tipo GET en JavaScript. Se declara una función asincrónica obtenerDatos() que utiliza async/await y try/catch para manejar la solicitud y cualquier error que pueda ocurrir. Dentro del bloque try, se utiliza axios.get() para hacer la solicitud a la URL especificada. Si la solicitud es exitosa, se imprime la respuesta en la consola. Si hay algún error durante la ejecución, se captura en el bloque catch y se imprime el mensaje de error correspondiente. Axios es una biblioteca popular para realizar solicitudes HTTP en JavaScript debido a su facilidad de uso y soporte para promesas y async/await.

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

#### 46. Diferencia entre los operadores de igualdad == y ===

    console.log(0 == false);          // true
    console.log(0 === false);         // false
    console.log(1 == "1");            // true
    console.log(1 === "1");           // false
    console.log(null == undefined);   // true
    console.log(null === undefined);  // false
    console.log('0' == false);        // true
    console.log('0' === false);       // false
    console.log([] == []);            // false, hacen referencia a objetos diferentes en memoria
    console.log([] === []);           // false, hacen referencia a objetos diferentes en memoria
    console.log({} == {});            // false, hacen referencia a objetos diferentes en memoria
    console.log({} === {});           // false, hacen referencia a objetos diferentes en memoria

#### 47. Funciones constructoras son funciones que se utilizan para crear objetos en JavaScript

##### Cómo utilizar funciones constructoras en JavaScript para crear objetos. La función constructora Persona se define con parámetros nombre y edad, que se utilizan para inicializar las propiedades del objeto. Se crean objetos persona1 y persona2 utilizando el operador new, pasando los valores deseados para nombre y edad. Después de crear los objetos, se puede acceder a sus propiedades utilizando la notación de punto (persona1.nombre, persona1.edad, etc.). Esto ilustra cómo las funciones constructoras pueden ser utilizadas como una forma conveniente de crear múltiples objetos con la misma estructura y comportamiento en JavaScript.

    // Definir una función constructora para crear objetos de tipo Persona
    function Persona(nombre, edad) {
        this.nombre = nombre;
        this.edad = edad;
    }

    // Crear objetos utilizando la función constructora
    const persona1 = new Persona('Juan', 30);
    const persona2 = new Persona('María', 25);

    // Acceder a las propiedades de los objetos creados
    console.log(persona1.nombre); // Imprime: Juan
    console.log(persona1.edad);   // Imprime: 30

    console.log(persona2.nombre); // Imprime: María
    console.log(persona2.edad);   // Imprime: 25

#### 48. Generar una matriz (Array) de números con números desde el 0 hasta el 50

##### Cómo generar una matriz (array) de números del 0 al 50 en JavaScript utilizando un bucle for. Se inicializa un array vacío numbersArray y se define una variable max con el valor 50. Luego, se utiliza un bucle for para iterar desde 0 hasta max, y en cada iteración se agrega el valor actual de i al array numbersArray utilizando el método push(). Finalmente, se imprime el array resultante en la consola.

    const numbersArray = [];
    const max = 50;

    for (let i = 0; i <= max; i++) {
        numbersArray.push(i);
    }

    console.log(numbersArray); // Imprime: [0, 1, 2, ..., 50]

#### 49. Generar un conjunto aleatorio de personajes alfanuméricos

##### Se define una cadena caracteres que contiene todos los caracteres alfabéticos en mayúsculas y minúsculas, así como los dígitos del 0 al 9. Luego, se especifica la longitud del conjunto deseado en la variable longitudConjunto. Se inicializa una cadena vacía conjuntoAleatorio que se utilizará para almacenar el conjunto aleatorio generado.

#### A continuación, se utiliza un bucle for para iterar longitudConjunto veces. En cada iteración, se genera un índice aleatorio entre 0 y la longitud de la cadena de caracteres utilizando Math.random(). Luego, se utiliza charAt(indice) para obtener el carácter correspondiente al índice generado y se concatena a la cadena conjuntoAleatorio.

    const caracteres = 'ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz0123456789';
    const longitudConjunto = 10; // Longitud del conjunto deseado
    let conjuntoAleatorio = '';

    for (let i = 0; i < longitudConjunto; i++) {
        const indice = Math.floor(Math.random() * caracteres.length);
        conjuntoAleatorio += caracteres.charAt(indice);
    }

    console.log(conjuntoAleatorio); // Imprime el conjunto aleatorio generado

#### 50. Verifique si el valor de una variable es un número

##### Se define una variable argumento que contiene el valor que se desea verificar. Luego, se utiliza un condicional if para comprobar si el tipo de datos de argumento es igual a 'number' utilizando el operador typeof. Si el resultado de esta comprobación es verdadero, se imprime en la consola el mensaje 'El argumento es un número.', de lo contrario se imprime 'El argumento NO es un número.'

    const argumento = 5; // Cambia esto por el argumento que desees verificar

    if (typeof argumento === 'number') {
        console.log('El argumento es un número.');
    } else {
        console.log('El argumento NO es un número.');
    }

#### 51. Verifique que un argumento dado en una función es un array

##### Se define una función llamada verificarArray que toma un argumento argumento. Dentro de la función, se utiliza el método estático Array.isArray() para comprobar si argumento es un array. Si Array.isArray(argumento) devuelve true, se imprime en la consola el mensaje 'El argumento es un array.', de lo contrario se imprime 'El argumento NO es un array.'.

#### Finalmente, se llama a la función verificarArray con un ejemplo de array miArray como argumento.

    function verificarArray(argumento) {
        if (Array.isArray(argumento)) {
            console.log('El argumento es un array.');
        } else {
            console.log('El argumento NO es un array.');
        }
    }

    const miArray = [1, 2, 3]; // Cambia esto por el argumento que desees verificar
    verificarArray(miArray);

#### 52. Extraer el máximo y el mínimo de una serie de números en un array utilizando los métodos Math.max() y Math.min() junto con el operador de propagación (...)

##### Cómo extraer el máximo y el mínimo de una serie de números almacenados en un array utilizando los métodos Math.max() y Math.min() junto con el operador de propagación (...).

    const numeros = [5, 2, 8, 10, 3];

    const maximo = Math.max(...numeros);
    const minimo = Math.min(...numeros);

    console.log('Máximo:', maximo); // Imprime: Máximo: 10
    console.log('Mínimo:', minimo); // Imprime: Mínimo: 2

#### 53. Validar si un Array esta vacio

##### Se define un array llamado miArray, y luego se utiliza una estructura condicional if para verificar si la propiedad length del array es igual a cero. Si miArray.length es igual a cero, significa que el array está vacío y se imprime en la consola el mensaje 'El array está vacío.'. De lo contrario, si miArray.length no es igual a cero, significa que el array no está vacío y se imprime en la consola el mensaje 'El array NO está vacío.'.

    const miArray = []; // Cambia esto por tu array

    if (miArray.length === 0) {
        console.log('El array está vacío.');
    } else {
        console.log('El array NO está vacío.');
    }

#### 54. setTimeout() se utiliza para ejecutar una función después de que haya transcurrido un tiempo específico (en milisegundos).

##### Se define una función llamada saludar() que simplemente imprime en la consola el mensaje '¡Hola después de 2 segundos!'. Luego, se llama a la función setTimeout() con dos argumentos: la función saludar que se ejecutará después de que haya transcurrido el tiempo especificado, y el tiempo en milisegundos (en este caso, 2000 milisegundos, es decir, 2 segundos).

    // Función que se ejecutará después de 2 segundos
    function saludar() {
        console.log('¡Hola después de 2 segundos!');
    }

    // Llamar a la función después de 2 segundos
    setTimeout(saludar, 2000);

#### 55. setInterval() se utiliza para ejecutar una función repetidamente, cada cierto intervalo de tiempo especificado (en milisegundos)

    // Función que se ejecutará cada segundo
    function mostrarMensaje() {
        console.log('Mensaje repetido cada segundo');
    }

    // Llamar a la función cada segundo
    setInterval(mostrarMensaje, 1000);

#### 56. Eliminar elemento de un Array con el Método splice(), este modifica el contenido de un array eliminando o reemplazando elementos existentes y/o agregando nuevos elementos en su lugar.

##### Esto ilustra cómo se puede configurar una tarea para que se repita a intervalos regulares utilizando setInterval() en JavaScript.

    let array = [1, 2, 3, 4, 5];
    const indiceAEliminar = 2; // Índice del elemento a eliminar

    // Eliminar el elemento en el índice especificado
    array.splice(indiceAEliminar, 1);

    console.log(array); // Resultado: [1, 2, 4, 5]

#### 57. Eliminar elemento de un Array con el Método pop(), elimina el último elemento de un array y lo devuelve.

##### Al llamar al método pop() sobre el array, se elimina el último elemento, que es el número 5, y se almacena en la variable elementoEliminado,después de ejecutar pop(), el array queda modificado y ahora contiene los números del 1 al 4.

    let array = [1, 2, 3, 4, 5];

    // Eliminar el último elemento del array
    const elementoEliminado = array.pop();

    console.log(array); // Resultado: [1, 2, 3, 4]
    console.log('Elemento eliminado:', elementoEliminado);
    // Resultado: Elemento eliminado: 5

#### 58. Eliminar elemento de un Array con el Método shift(), este elimina el primer elemento de un array y lo devuelve.

##### Al llamar al método shift() sobre el array, se elimina el primer elemento, que es el número 1, y se almacena en la variable elementoEliminado, después de ejecutar shift(), el array queda modificado y ahora contiene los números del 2 al 5.

    let array = [1, 2, 3, 4, 5];

    // Eliminar el primer elemento del array
    const elementoEliminado = array.shift();

    console.log(array); // Resultado: [2, 3, 4, 5]
    console.log('Elemento eliminado:', elementoEliminado);
    // Resultado: Elemento eliminado: 1

#### 59. Agregar un elemento al inicio del Array

##### Al llamar al método unshift() con el argumento "uva", se agrega esta fruta al principio del array, después de ejecutar unshift(), el array se modifica y ahora contiene las frutas "uva", "manzana", "banana" y "naranja".

    // Declarar un array de frutas
    let frutas = ["manzana", "banana", "naranja"];

    // Agregar un elemento al inicio del array
    frutas.unshift("uva");

#### 60. Agregar un elemento al final del Array

##### Al llamar al método push() con el argumento "sandía", se agrega esta fruta al final del array, después de ejecutar push(), el array se modifica y ahora contiene las frutas "uva", "manzana", "banana", "naranja" y "sandía".

    // Agregar un elemento al final del array
    frutas.push("sandía");

    console.log("Fruta agregada al final del array:", frutas);

# Preguntas y Respuestas 😱

#### ¿Cuál es la salida de este código?

    let miArray = [1, , 3];
    console.log(miArray.length);
    //Salida: 3

#### ¿Cuál es la salida de este código?

    console.log(2 + '2');
    //Salida: 22

#### ¿Cuál es la salida de este código?

    console.log(0.1 + 0.2 === 0.3);
    //Salida: false

#### ¿Cuál es la salida de este código?

    let x = 5;
    console.log(++x);
    //Salida: 6

#### ¿Cuál es la salida de este código?

    console.log(1 < 2 < 3);
    //Salida: true

#### ¿Cuál es la salida de este código?

    console.log(3 < 2 < 1);
    //Salida: true

#### ¿Cuál es la salida de este código?

    console.log(false == "0");
    //Salida: true

#### ¿Cuál es la salida de este código?

    console.log(false === "0");
    //Salida: false

#### ¿Cuál es la salida de este código?

    console.log([] == []);
    //Salida: false

#### ¿Cuál es la salida de este código?

    console.log(1 + "1");
    //Salida: 11

#### ¿Cuál es la salida de este código?

    console.log(1 - "1");
    //Salida: 0

#### ¿Cuál es la salida de este código?

    console.log("20" > "3");
    //Salida: false

#### ¿Cuál es la salida de este código?

    console.log(1 + "2", +3 + 4);
    //Salida: "12" 7

#### ¿Cuál es la salida de este código?

    let miArrayNumeros = [1, 2, 3];
    //Salida: [1, 1, 1]
    //Nota: Recordar ue el método fill() cambia todos los elementos en una matriz por un valor estático y devuelve la matriz modificada. En el primer caso, fill(1) rellena todos los elementos con el valor 1, y en el segundo caso, fill(0) rellena todos los elementos con el valor 0

#### ¿Cuál es la salida de este código?

    console.log(miArrayNumeros.fill(0));
    //Salida: [1, 1, 1]
