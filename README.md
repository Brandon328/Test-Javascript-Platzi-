# Test-Javascript-Platzi-

## Variables y operaciones

### 1️⃣ Responde las siguientes preguntas en la sección de comentarios:

- ¿Qué es una variable y para qué sirve?
    
    Una variables es un espacio en memoria, sirve para almacenar datos.
    
- ¿Cuál es la diferencia entre declarar e inicializar una variable?
    
    Cuando inicializamos una variable le asignamos un dato o un valor y esta es la principal diferencia con declarar una variable, pues en este último solo nombramos a dicha variable.
    
- ¿Cuál es la diferencia entre sumar números y concatenar strings?
    
    Los números se suman como nos enseñaron desde pequeños, y cuando hablamos de concatenar strings nos referimos a poner un carácter después del otro en una sola cadena de texto.
    
- ¿Cuál operador me permite sumar o concatenar?
    
    El operador que nos permite realizar estas dos operaciones es el signo “+”.
    

### 2️⃣ Determina el nombre y tipo de dato para almacenar en variables la siguiente información:

```jsx
// Nombre: String
let name = 'Brandon';

// Apellido: String
let surname = 'Huamán';

// Nombre de usuario en Platzi: String
let username = '@BrandonJJ328';

// Edad: Number
let age = 22;

// Correo electrónico: String
let email = 'tetonic020@gmail.com';

// Mayor de edad: Boolean
let grownup = true;

// Dinero ahorrado: Number
let saved_money = 1000000.00

// Deudas: Number
let debts = 10.00
```

### 4️⃣ Calcula e imprime las siguientes variables a partir de las variables del ejemplo anterior:

```jsx
// Nombre completo (nombre y apellido)
console.log(name+' '+surname);

// Dinero real (dinero ahorrado menos deudas)
console.log(saved_money - debts);
```

## Funciones

### 1️⃣ Responde las siguientes preguntas en la sección de comentarios:

- ¿Qué es una función?
    
    Es una porción de código en javascript.
    
- ¿Cuándo me sirve usar una función en mi código?
    
    Cuándo repites un bloque de código constantemente.
    
- ¿Cuál es la diferencia entre parámetros y argumentos de una función?
    
    Los parámetros son el conjunto de variables que definimos dentro de una función, mientras que los argumentos son los valores que asignamos a los parámetros de una función cuando esta es invocada.
    

### 2️⃣ Convierte el siguiente código en una función, pero, cambiando cuando sea necesario las variables constantes por parámetros y argumentos en una función:

```jsx
function greet(name, lastname, nickname){
	console.log(`Mi nombre es ${name} ${lastname}, pero prefiero que me digas ${nickname}.`);
}
```

## Condicionales

### 1️⃣ Responde las siguientes preguntas en la sección de comentarios:

- ¿Qué es un condicional?
    
    Es una porción de código que se ejecuta si se cumple una condición determinada.
    
- ¿Qué tipos de condicionales existen en JavaScript y cuáles son sus diferencias?
    
    En javascript existen las sigueintes condicionales: if else, switch. El primero evalúa solo dos condiciones y el segundo evalúa mas de dos.
    
- ¿Puedo combinar funciones y condicionales?
    
    Si.
    

### 2️⃣ Replica el comportamiento del siguiente código que usa la sentencia switch utilizando if, else y else if:

```jsx
const tipoDeSuscripcion = "Basic";

if (tipoDeSuscripcion == "Free") console.log("Solo puedes tomar los cursos gratis");
if (tipoDeSuscripcion == "Basic") console.log("Puedes tomar casi todos los cursos de Platzi durante un mes");
if (tipoDeSuscripcion == "Expert") console.log("Puedes tomar casi todos los cursos de Platzi durante un año");
if (tipoDeSuscripcion == "ExpertPlus") console.log("Tú y alguien más pueden tomar TODOS los cursos de Platzi durante un año");
```

### 3️⃣ Replica el comportamiento de tu condicional anterior con if, else y else if, pero ahora solo con if (sin else ni else if).

```jsx
const tipoDeSuscripcion = "Basic";

const suscripciones = {
	"Free": "Solo puedes tomar los cursos gratis",	
	"Basic": "Solo puedes tomar los cursos gratis",
	"Expert": "Puedes tomar casi todos los cursos de Platzi durante un año",
	"ExpertPlus": "Tú y alguien más pueden tomar TODOS los cursos de Platzi durante un año"
}

console.log(suscripciones[tipoDeSuscripción]);
```

## Ciclos

### 1️⃣ Responde las siguientes preguntas en la sección de comentarios:

- ¿Qué es un ciclo?
    
    Es una porción de código que se repite siempre y cuando se cumpla una condición.
    
- ¿Qué tipos de ciclos existen en JavaScript?
    
    Los ciclos son: for, while, etc.
    
- ¿Qué es un ciclo infinito y por qué es un problema?
    
    Son ciclos con una condicional que siempre se cumple. Es un problema porque sobrecarga la memoria del computador volviéndolo más lenta.
    
- ¿Puedo mezclar ciclos y condicionales?
    
    Si.
    

### 2️⃣ Replica el comportamiento de los siguientes ciclos for utilizando ciclos while:

```jsx
let i = 0;
while(i<5){
	console.log("El valor de i es: " + i);
	i++;
}

let i = 10;
while(i>=2){
	console.log("El valor de i es: " + i);
	i--;
}
```

### 3️⃣ Escribe un código en JavaScript que le pregunte a los usuarios cuánto es `2 + 2`. Si responden bien, mostramos un mensaje de felicitaciones, pero si responden mal, volvemos a empezar.

```jsx
let answer;
while (answer != 4){
	answer = prompt('¿Cuánto es 2+2?');
}
alert('¡Felicitaciones!');

```

## Listas

### 1️⃣ Responde las siguientes preguntas en la sección de comentarios:

- ¿Qué es un array?
    
    También conocido como vector, es una estructura o conjunto de datos organizados en fila, en donde cada elemento posee un número de orden llamado índice.
    
- ¿Qué es un objeto?
    
    Es un conjunto de pares clave-valor. A diferencia de los arrays estos no llevan un orden.
    
- ¿Cuándo es mejor usar objetos o arrays?
    
    Depende mucho de lo que quieras hacer.
    
- ¿Puedo mezclar arrays con objetos o incluso objetos con arrays?
    
    Si.
    

### 2️⃣ Crea una función que pueda recibir cualquier array como parámetro e imprima su primer elemento.

```jsx
function spit(arr){
	return arr[0];
}
```

### 3️⃣ Crea una función que pueda recibir cualquier array como parámetro e imprima todos sus elementos uno por uno (no se vale imprimir el array completo).

```jsx
function spit_each(arr){
	arr.forEach(e=>console.log(e));
}
```

### 4️⃣ Crea una función que pueda recibir cualquier objeto como parámetro e imprima todos sus elementos uno por uno (no se vale imprimir el objeto completo).

```jsx
function spit_obj(obj){
	for(const [key, value] of Object.entries(obj)){
	  console.log(`${key}: ${value}`);
	}
}
```
