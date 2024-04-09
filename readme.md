# Todo lo que necesitas saber: Preguntas y respuestas sobre JavaScript, la guía completa.

#### Esta es tu guía definitiva para comprender los conceptos fundamentales y avanzados de JavaScript. Desde las nociones básicas hasta los temas más complejos, explorarás una amplia variedad de preguntas y respuestas diseñadas para ayudarte a dominar este poderoso lenguaje de programación. Ya sea que estés comenzando tu viaje en el desarrollo web o buscando ampliar tus conocimientos, esta guía te proporcionará la información necesaria para convertirte en un experto en JavaScript.

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

    let edad = 18;
    if (edad >= 18) {
    console.log("Eres mayor de edad");
    } else {
    console.log("Eres menor de edad");
    }

#### 4. Bucle For

    const array = ['a', 'b', 'c', 'd'];

    for (let i = 0; i < array.length; i++) {
    console.log(array[i]);
    }

#### 5. Bucle for...in

    const objeto = { a: 1, b: 2, c: 3 };

    for (let propiedad in objeto) {
    console.log(propiedad + ': ' + objeto[propiedad]);
    }

#### 6. Bucle while

    let contador = 0;
    while (contador < 5) {
    console.log(contador);
    contador++;
    }

#### 7. Métodos forEach

    let frutas = ["manzana", "banana", "pera"];
    // Recorrer un arreglo
    frutas.forEach(function(fruta) {
    console.log(fruta);
    });

    // Añadir un elemento al arreglo
    frutas.push("naranja");

    // Eliminar el último elemento del arreglo
    frutas.pop();

#### 8. Objetos y Métodos de Objetos

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
    console.log(texto.toUpperCase()); // Imprime: HOLA MUNDO

    // Convertir a minúsculas
    console.log(texto.toLowerCase()); // Imprime: hola mundo

    // Obtener la longitud del texto
    console.log(texto.length); // Imprime: 10

#### 10. Método indexOf()

    let frase = "El perro come comida";
    // Encontrar la posición de una palabra en la frase
    console.log(frase.indexOf("perro")); // Imprime: 3

#### 11. Método slice()

    let frase = "JavaScript es divertido";
    // Extraer una parte de la cadena
    console.log(frase.slice(0, 10));
    // Imprime: JavaScript

#### 12. Método replace()

    let frase = "Aprender es divertido";
    // Reemplazar parte de la cadena
    console.log(frase.replace("divertido", "genial"));
    // Imprime: Aprender es genial

#### 13. Método split()

    let lista = "manzana,naranja,uva";
    // Dividir una cadena en un arreglo
    let frutas = lista.split(",");
    console.log(frutas);
    // Imprime: ["manzana", "naranja", "uva"]

#### 14. Método join()

    let frutas = ["manzana", "naranja", "uva"];
    // Unir elementos de un arreglo en una cadena
    let lista = frutas.join(", ");
    console.log(lista);
    // Imprime: manzana, naranja, uva

#### 15. Método push()

    let numeros = [1, 2, 3];
    // Añadir un elemento al final del arreglo
    numeros.push(4);
    console.log(numeros);
    // Imprime: [1, 2, 3, 4]

#### 16. Método pop()

    let numeros = [1, 2, 3];
    // Eliminar el último elemento del arreglo
    numeros.pop();
    console.log(numeros);
    // Imprime: [1, 2]

#### 17. Método shift()

    let numeros = [1, 2, 3];
    // Eliminar el primer elemento del arreglo
    numeros.shift();
    console.log(numeros);
    // Imprime: [2, 3]

#### 18. Método unshift()

    let numeros = [2, 3];
    // Añadir un elemento al inicio del arreglo
    numeros.unshift(1);
    console.log(numeros);
    // Imprime: [1, 2, 3]

#### 19. Método includes()

    let numeros = [1, 2, 3];
    // Verificar si un elemento está en el arreglo
    console.log(numeros.includes(2)); // Imprime: true
    console.log(numeros.includes(4)); // Imprime: false

#### 20. Método sort()

    let frutas = ["naranja", "manzana", "uva"];
    // Ordenar elementos de un arreglo
    frutas.sort();
    console.log(frutas);
    // Imprime: ["manzana", "naranja", "uva"]

#### 21. Método reverse()

    let numeros = [1, 2, 3];
    // Invertir el orden de los elementos en el arreglo
    numeros.reverse();
    console.log(numeros);
    // Imprime: [3, 2, 1]

#### 22. Método map()

    let numeros = [1, 2, 3];
    // Aplicar una función a cada elemento del arreglo
    let duplicados = numeros.map(numero => numero * 2);
    console.log(duplicados);
    // Imprime: [2, 4, 6]

#### 23. Método filter()

    let numeros = [1, 2, 3, 4, 5];
    // Filtrar elementos de un arreglo
    let impares = numeros.filter(numero => numero % 2 !== 0);
    console.log(impares);
    // Imprime: [1, 3, 5]

#### 24. Método reduce()

    let numeros = [1, 2, 3, 4, 5];
    // Reducir el arreglo a un único valor
    let suma = numeros.reduce((total, numero) => total + numero, 0);
    console.log(suma);
    // Imprime: 15

#### 25. Funciones Flecha

    // Función normal
    function suma(a, b) {
    return a + b;
    }

    // Función flecha
    let suma = (a, b) => a + b;

#### 26. Template String

    let nombre = "Juan";
    let edad = 30;

    // Uso de template strings
    console.log(`Hola, mi nombre es ${nombre} y tengo ${edad} años.`);

#### 27. Spread Operator

    let numeros = [1, 2, 3];
    let otrosNumeros = [4, 5, 6];

    // Combinar arreglos
    let todosLosNumeros = [...numeros, ...otrosNumeros];
    console.log(todosLosNumeros);
    // Imprime: [1, 2, 3, 4, 5, 6]

#### 28. Destructuring

    let persona = { nombre: "Juan", edad: 30 };

    // Destructuring de objeto
    let { nombre, edad } = persona;
    console.log(nombre, edad); // Imprime: Juan 30

#### 29. Parámetros de función predeterminados

        function greet(name = "Urian") {
            return `Hola, ${name}!`;
        }

#### 30. Operador Ternario

    let precio = 100;
    let mensaje = precio > 50 ? "Caro" : "Barato";

    console.log(mensaje); // Imprime: Caro

#### 31. asignación de destructuración

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

    // Array con registros repetidos
    const registros = [1, 2, 3, 1, 2, 4, 5, 3];

    // Eliminar registros repetidos utilizando Set
    const registrosUnicos = [...new Set(registros)];

    // Mostrar los registros únicos
    console.log(registrosUnicos); // Imprime: [1, 2, 3, 4, 5]

#### 35. Eliminar elementos repetidos de un Array usando filter y indexOf

    const registros = [1, 2, 3, 1, 2, 4, 5, 3];
    const registrosUnicos = registros.filter((valor, indice, arreglo) => arreglo.indexOf(valor) === indice);
    console.log(registrosUnicos); // Imprime: [1, 2, 3, 4, 5]

#### 36. Eliminar elementos repetidos de un Array usando filter y includes

    const registros = [1, 2, 3, 1, 2, 4, 5, 3];
    const registrosUnicos = registros.filter((valor, indice, arreglo) => arreglo.includes(valor, indice + 1));
    console.log(registrosUnicos); // Imprime: [1, 2, 3, 4, 5]

#### 37. Eliminar elementos repetidos de un Array usando reduce

    const registros = [1, 2, 3, 1, 2, 4, 5, 3];
    const registrosUnicos = registros.reduce((unicos, valor) => unicos.includes(valor) ? unicos : [...unicos, valor], []);
    console.log(registrosUnicos); // Imprime: [1, 2, 3, 4, 5]

#### 38. Asignación de valores predeterminados

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

    const array = [1, 2, 3, 4, 5];

    // Verificar si el elemento 3 existe en el array
    if (array.includes(3)) {
    console.log('El elemento 3 está presente en el array');
    } else {
    console.log('El elemento 3 no está presente en el array');
    }

#### 40. Verificar si un elemento existe en un array utilizando el método indexOf()

    const array = [1, 2, 3, 4, 5];

    // Verificar si el elemento 3 existe en el array
    if (array.indexOf(3) !== -1) {
    console.log('El elemento 3 está presente en el array');
    } else {
    console.log('El elemento 3 no está presente en el array');
    }

#### 41. Prevención de la modificación de objetos

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

    const numbersArray = [];
    const max = 50;

    for (let i = 0; i <= max; i++) {
        numbersArray.push(i);
    }

    console.log(numbersArray); // Imprime: [0, 1, 2, ..., 50]

#### 49. Generar un conjunto aleatorio de personajes alfanuméricos

    const caracteres = 'ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz0123456789';
    const longitudConjunto = 10; // Longitud del conjunto deseado
    let conjuntoAleatorio = '';

    for (let i = 0; i < longitudConjunto; i++) {
        const indice = Math.floor(Math.random() * caracteres.length);
        conjuntoAleatorio += caracteres.charAt(indice);
    }

    console.log(conjuntoAleatorio); // Imprime el conjunto aleatorio generado

#### 50. Verifique si el valor de una variable es un número

    const argumento = 5; // Cambia esto por el argumento que desees verificar

    if (typeof argumento === 'number') {
    console.log('El argumento es un número.');
    } else {
    console.log('El argumento NO es un número.');
    }

#### 51. Verifique que un argumento dado en una función es un array

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

    const numeros = [5, 2, 8, 10, 3];

    const maximo = Math.max(...numeros);
    const minimo = Math.min(...numeros);

    console.log('Máximo:', maximo); // Imprime: Máximo: 10
    console.log('Mínimo:', minimo); // Imprime: Mínimo: 2

#### 53. Validar si un Array esta vacio

    const miArray = []; // Cambia esto por tu array

    if (miArray.length === 0) {
    console.log('El array está vacío.');
    } else {
    console.log('El array NO está vacío.');
    }

#### 54. setTimeout() se utiliza para ejecutar una función después de que haya transcurrido un tiempo específico (en milisegundos).

    // Función que se ejecutará después de 2 segundos
    function saludar() {
    console.log('¡Hola después de 2 segundos!');
    }

    // Llamar a la función después de 2 segundos
    setTimeout(saludar, 2000);

### 55. setInterval() se utiliza para ejecutar una función repetidamente, cada cierto intervalo de tiempo especificado (en milisegundos)

    // Función que se ejecutará cada segundo
    function mostrarMensaje() {
    console.log('Mensaje repetido cada segundo');
    }

    // Llamar a la función cada segundo
    setInterval(mostrarMensaje, 1000);

#### 56. Eliminar elemento de un Array con el Método splice(), este modifica el contenido de un array eliminando o reemplazando elementos existentes y/o agregando nuevos elementos en su lugar.

    let array = [1, 2, 3, 4, 5];
    const indiceAEliminar = 2; // Índice del elemento a eliminar

    // Eliminar el elemento en el índice especificado
    array.splice(indiceAEliminar, 1);

    console.log(array); // Resultado: [1, 2, 4, 5]

#### 57. Eliminar elemento de un Array con el Método pop(), elimina el último elemento de un array y lo devuelve.

    let array = [1, 2, 3, 4, 5];

    // Eliminar el último elemento del array
    const elementoEliminado = array.pop();

    console.log(array); // Resultado: [1, 2, 3, 4]
    console.log('Elemento eliminado:', elementoEliminado); // Resultado: Elemento eliminado: 5

#### 58. Eliminar elemento de un Array con el Método shift(), este elimina el primer elemento de un array y lo devuelve.

    let array = [1, 2, 3, 4, 5];

    // Eliminar el primer elemento del array
    const elementoEliminado = array.shift();

    console.log(array); // Resultado: [2, 3, 4, 5]
    console.log('Elemento eliminado:', elementoEliminado); // Resultado: Elemento eliminado: 1

#### 59. Agregar un elemento al inicio del Array

    // Declarar un array de frutas
    let frutas = ["manzana", "banana", "naranja"];

    // Agregar un elemento al inicio del array
    frutas.unshift("uva");

#### 60. Agregar un elemento al final del Array

    // Agregar un elemento al final del array
    frutas.push("sandía");

    console.log("Fruta agregada al final del array:", frutas);

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
