# Javascript-Test
This is the test I took for the course Javascript in Platzi
Variables y operaciones

1️⃣ Responde las siguientes preguntas en la sección de comentarios:
¿Qué es una variable y para qué sirve?
Es un espacio reservado en memoria que nos permite almacenar información.
¿Cuál es la diferencia entre declarar e inicializar una variable?
Una variable se declara para indicarle al programa a partir de qué lugar empieza a existir, qué nombre tendrá y qué tipo de datos almacenará. La asignación de un valor inicial se llama inicialización
¿Cuál es la diferencia entre sumar números y concatenar strings?
Sumar numeros es la operación matematica de sumar, es decir, la adición matematica de una cantidad a otra. En cambio, concatenar strings es añadir texto adicional a un texto.
¿Cuál operador me permite sumar o concatenar?
Para ambos casos es el signo +

2️⃣ Determina el nombre y tipo de dato para almacenar en variables la siguiente información:
Nombre
var name = string
Apellido
var lastname = string
Nombre de usuario en Platzi
var user = string
Edad
var age = number
Correo electrónico
var email = string
Mayor de edad
var aged = boolean
Dinero ahorrado
var money = number
Deudas
var debts = number

3️⃣ Traduce a código JavaScript las variables del ejemplo anterior y deja tu código en los comentarios.

var name = "Alex"
var lastname = "Angulo"
var user = "alex.angulo"
var age = 27
var email = "ing.alex.angulo@gmail.com"
var aged = true
var money = 10000
var debts = 0

4️⃣ Calcula e imprime las siguientes variables a partir de las variables del ejemplo anterior:
Nombre completo (nombre y apellido)
Dinero real (dinero ahorrado menos deudas)

var fullname = name + " " + lastname
console.log(fullname)

var fullmoney = money - debts
console.log(fullmoney)

1️⃣ Responde las siguientes preguntas en la sección de comentarios:
¿Qué es una función?
Una función es un bloque de código que realiza alguna operación
¿Cuándo me sirve usar una función en mi código?
Para realizar una funcionalidad en especifico
¿Cuál es la diferencia entre parámetros y argumentos de una función?
Cada argumento corresponde al parámetro que se encuentra en la misma posición en la lista. A diferencia de la definición de parámetro, los argumentos no tienen nombres. Cada argumento es una expresión que puede contener cero o más variables, constantes y literales.
¿Cuál es la diferencia entre parámetros y argumentos de una función?
2️⃣ Convierte el siguiente código en una función, pero, cambiando cuando sea necesario las variables constantes por parámetros y argumentos en una función:
const name = "Juan David";
const lastname = "Castro Gallego";
const completeName = name + lastname;
const nickname = "juandc";

console.log("Mi nombre es " + completeName + ", pero prefiero que me digas " + nickname + ".");

var userinformation = [{name: "juan David",
                        lastname: "Castro Gallego",
                        nickname: "juandc"}]
 function myFunction(userinformation){
 var completeName = userinformation.name + userinformation.lastname
 console.log("Mi nombre es " + completeName + ", pero prefiero que me digas " + userinformation.nickname + ".");}
 
 1️⃣ Responde las siguientes preguntas en la sección de comentarios:
¿Qué es un condicional?
Las «instrucciones condicionales» se usan para realizar las diferentes acciones según una condición.

En JavaScript podemos encontrar las siguientes declaraciones condicionales:

if: se usa para ejecutar un bloque código si la condición es verdadera.
if…else: se usa para ejecutar un bloque de código si la condición es verdadera u otro bloque de código si la condición es falsa.
if…else if…else: se usa para seleccionar uno de los muchos bloques de código a ejecutar.
switch: se usa para seleccionar uno de los varios bloques de código a ejecutar (igual ).
¿Qué tipos de condicionales existen en JavaScript y cuáles son sus diferencias?
if: se usa para ejecutar un bloque código si la condición es verdadera.
if…else: se usa para ejecutar un bloque de código si la condición es verdadera u otro bloque de código si la condición es falsa.
if…else if…else: se usa para seleccionar uno de los muchos bloques de código a ejecutar.
switch: se usa para seleccionar uno de los varios bloques de código a ejecutar (igual ).
¿Puedo combinar funciones y condicionales?
Podemos encadenar una respusta desde un condional a otro pero no podemos combinarlo dentro de una misma expresión. Si podemos ocuparlos de forma separada y luego encadenar una acción dependiendo del resultado.


2️⃣ Replica el comportamiento del siguiente código que usa la sentencia switch utilizando if, else y else if:
const tipoDeSuscripcion = "Basic";

switch (tipoDeSuscripcion) {
   case "Free":
       console.log("Solo puedes tomar los cursos gratis");
       break;
   case "Basic":
       console.log("Puedes tomar casi todos los cursos de Platzi durante un mes");
       break;
   case "Expert":
       console.log("Puedes tomar casi todos los cursos de Platzi durante un año");
       break;
   case "ExpertPlus":
       console.log("Tú y alguien más pueden tomar TODOS los cursos de Platzi durante un año");
       break;
}

Solution

if(tipoDeSuscripcion == "Free"){
console.log("Solo puedes tomar los cursos gratis");
}else if (tipoDeSuscripcion == "Basic"){
 console.log("Puedes tomar casi todos los cursos de Platzi durante un mes");
 }else if (tipoDeSuscripcion == "Expert"){ 
  console.log("Puedes tomar casi todos los cursos de Platzi durante un año");
 }else if (tipoDeSuscripcion == "ExpertPlus"){ 
console.log("Tú y alguien más pueden tomar TODOS los cursos de Platzi durante un año");
}

3️⃣ Replica el comportamiento de tu condicional anterior con if, else y else if, pero ahora solo con if (sin else ni else if).
let typeSuscripción = [
"Free",
"Basic", 
"Expert", 
"ExpertPlus"
];
let infoSuscripción = [
"solo puedes tomar los cursos gratis", 
"puedes tomar casi todos los cursos de Platzi durante un mes", 
"puedes tomar casi todos los cursos de Platzi durante un año", 
"tú y alguien más pueden tomar TODOS los cursos de Platzi durante un año"];
let userSuscription = "Expert";
for (let i=0; i < typeSuscripción.length; i++) {
  if (userSuscription == typeSuscripción[i]) {
  	console.log(`Si estas suscrito al plan ${typeSuscripción[i]} en el cual ${infoSuscripción[i]}`)
  }
}








