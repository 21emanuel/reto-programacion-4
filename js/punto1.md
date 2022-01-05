## ¿Qué es una variable y para qué sirve?

Es una forma de almacenar un valor en la memoria RAM, ppara poder reutilizarlas, calculadoras, ect.

## ¿Cuál es la diferencia entre declarar e inicializar una variable?

- Declarar es dar un nombre a la variable ej: `let numero`
- Inicializar es **asignar** un valor a la variable ej: `numero = 1`

## ¿Cuál es la diferencia entre sumar números y concatenar strings?

- La suma se realiza unicamente con variables de tipo **number**
- La concatenacion se realiza uniendo **string** con otros valores

## ¿Qué operador me permite sumar o concatenar?

- El operador suma: `+`

## Determina el nombre y tipo de dato para almacenar en variables la siguiente información:

- Nombre `const nombre = 'Esteban'`
- Apellido `const apellido = 'Mamani'`
- Nombre de usuario `const username = ecrmamani`
- Edad `let edad = 18`
- Correo electrónico `let email = 'estebandamian@gmail.com'`
- Mayor de edad `let mayorEdad = true`
- Dinero ahorrado `let ahorro = 20000.50`
- Deudas `let deudas = 0`

## Traduce a código JavaScript las variables del ejemplo anterior y deja tu código en un archivo nuevo.

`const persona = { nombre: 'cristian', apellido: 'chaime', username: 'ectam', edad: 18, email: 'ectam484@gmail.com' }`

## Calcula e imprime las siguientes variables a partir de las variables del ejemplo anterior:

- Nombre completo (nombre y apellido)
  `const nombreCompleto = persona.nombre + ' ' + persona.apellido`
- Dinero real (dinero ahorrado menos deudas)
  `const patrimonio = persona.ahorro - persona.deudas`

## Responde las siguientes preguntas en un nuevo archivo:

## ¿Qué es una función?

- Es un conjunto de instrucciones agrupados en un bloque de codigo

## ¿Cuándo me sirve usar una función en mi código?

- Me sirve para dividir mis tareas en diferentes funciones que realizan un unica tarea

## ¿Cuál es la diferencia entre parámetros y argumentos de una función?

- Parametros son cuanndo inicializamos la funcion
- Argumentos son cuando llamamos la funcion

## Convierte el siguiente código en una función, pero, cambiando cuando sea necesario las variables constantes por parámetros y argumentos en una función:

`const name = "Juan David";
const lastname = "Castro Gallego";
const completeName = name + lastname;
const nickname = "juandc";

console.log("Mi nombre es " + completeName + ", pero prefiero que me digas " + nickname + ".");`

`funcion presentacion (completeName, nikName) { const frase = `Mi nombre es ${completeName}, pero prefiero que me digas ${nikName}`} const res = presentacion(completeName, nikName); console.log(res)`

## Responde las siguientes preguntas en un nuevo archivo:

- ¿Qué es una condicional?
  - Los condicionales es una forma de controlar el flujo de ejecucion de mi codigo. Por el lado verdadero y el falso.
- ¿Qué tipos de condicionales existen en JavaScript y cuáles son sus diferencias?
  - Existen 4 tipos: if else, else if, switch y if ternario. Cuando tenemos varios else if anidados nos conviene usar switch.
- ¿Puedo combinar funciones y condicionales?
  - SI

## Replica el comportamiento del siguiente código que usa la sentencia switch utilizando if, else y else if:

`const tipoDeSuscripcion = "Basic";

switch (tipoDeSuscripcion) {
case "Free":
console.log("Solo puedes tomar los cursos gratis");
break;
case "Basic":
console.log("Puedes tomar casi todos los cursos durante un mes");
break;
case "Expert":
console.log("Puedes tomar casi todos los cursos durante un año");
break;
case "ExpertPlus":
console.log("Tú y alguien más pueden tomar TODOS los cursos durante un año");
break;
}`

`if ( tipoDeSuscripcion === 'free') { console.log("Solo puedes tomar los cursos gratis"); } else if (tipoDeSuscripcion === 'Basic') { console.log("Puedes tomar casi todos los cursos durante un mes"); } else if (tipoDeSuscripcion === 'Expert') { console.log("Puedes tomar casi todos los cursos durante un año"); } else if (tipoDeSuscripcion === 'ExpertPlus') { console.log("Tú y alguien más pueden tomar TODOS los cursos durante un año"); }`

## Replica el comportamiento de tu condicional anterior con if, else y else if, pero ahora solo con if (sin else ni else if).

`if (tipoDeSuscripcion === 'free') console.log("Solo puedes tomar los cursos gratis");`
`if (tipoDeSuscripcion === 'Basic') console.log("Puedes tomar casi todos los cursos durante un mes");`
`if (tipoDeSuscripcion === 'Expert') console.log("Puedes tomar casi todos los cursos durante un año");`
`if (tipoDeSuscripcion === 'ExpertPlus') console.log("Tú y alguien más pueden tomar TODOS los cursos durante un año");`

## Bonus: si ya eres una experta o experto en el lenguaje, te desafío a comentar cómo replicar este comportamiento con arrays y un solo condicional. 😏

`const subs = ['free', 'Basic', 'Expert', 'ExpertPlus']`
`const mensaje = ['mens1', 'm2', 'm3', 'm4']`
`const pos = sub.`

## Responde las siguientes preguntas en un nuevo archivo:

- ¿Qué es un ciclo?
  - Los bucles o ciclos son sentencia sque se utilizan para ejecutar una o varias instrucciones de forma repetitiva cuando sea necesario
- ¿Qué tipos de ciclos existen en JavaScript?
  - Existen tres tipos de bucles principales pero dentro de estos también existen sus propias ramas como veremos a continuación: for(for in, for of, for-each), while, do while.
- ¿Qué es un ciclo infinito y por qué es un problema?
  - existen 3 ciclos el while, el for ,y el do while
- ¿Puedo mezclar ciclos y condicionales?
  - Si se puede mmezclar

## Replica el comportamiento de los siguientes ciclos for utilizando ciclos while:

`for (let i = 0; i < 5; i++) { console.log("El valor de i es: " + i); } for (let i = 10; i >= 2; i--) { console.log("El valor de i es: " + i); }`

## Escribe un código en JavaScript que le pregunte a los usuarios cuánto es 2 + 2. Si responden bien, mostramos un mensaje de felicitaciones, pero si responden mal, volvemos a empezar.

`let incorrecto = true;

while (incorrecto) {
const respuesta = prompt('¿cuanto es 2 + 2?');
if(respuesta == 4){
incorrecto = false;
console.log('felicidades la respuesta es correcta')
}
}`

## Responde las siguientes preguntas en un nuevo archivo:

- ¿Que es una array?

  - Un array es un tipo de dato que tiene como funcionalidad almacenar, del mismo tipo o relacionados, los elementos que están dentros de un array pueden ser de tipos simples o compuestos

- ¿Que es un objeto?

  - Los objetos son colecciones de datos que constan de variables y funciones, a estos dos se los llaman propiedades y métodos cuando están dentro del objeto

- ¿Cuándo es mejor usar objetos o arrays?

  - Se puede usar tanto arrays que contengas objetos como asi también objectos que contengan array usualmente son cases en que las tareas requieren de 2 o mas tipos de inforacion

- ¿Puedo mezclar arrays con objetos o incluso objetos con arrays?

  - si se puede

## Crea una función que pueda recibir cualquier array como parámetro e imprima su primer elemento.

const componentePc = ['cpu', 'motherboard','ram','ssd'];

const firstElement = () => {
const primerElemento = componentePc[0];
console.log(primerElemento)
}

firstElement();

## Crea una función que pueda recibir cualquier array como parámetro e imprima todos sus elementos uno por uno (no se vale imprimir el array completo).

`let cosas = ['pelota', 'casa','piso','departamento'];

const cosasName = () => {
nombreCosas.forEach( nombresCosas => {
console.log(`hola ${nombresCosas}`)
});
}
cosasName()`

## Crea una función que pueda recibir cualquier objeto como parámetro e imprima todos sus elementos uno por uno (no se vale imprimir el objeto completo).

`const personas1 ={
nombre: 'critian',
apellido: 'chaime',
nombreUsuario: 'ectam21',
};

const infoPersona = () =>{
for(const recorrido in personas1) {
console.log(`inforacion personas1: ${recorrido} => ${personas1[recorrido]}`);
};
};

infoPersona();`
