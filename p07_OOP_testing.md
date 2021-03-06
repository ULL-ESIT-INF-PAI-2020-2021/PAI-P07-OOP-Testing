# Práctica 7. Programación Orientada a Objetos en JavaScript. Unit Testing
### Factor de ponderación: 7

### Objetivos
Los objetivos de esta práctica son:
 
* Poner en práctica metodologías y conceptos de Programación Orientada a Objetos en JavaScript.
* Practicar el diseño y desarrollo de pruebas de software (testing) utilizando Mocha y Chai.

### Rúbrica de evaluacion del ejercicio
Se señalan a continuación los aspectos más relevantes (la lista no es exhaustiva)
que se tendrán en cuenta a la hora de evaluar esta práctica:

* El comportamiento del programa debe ajustarse a lo solicitado en este enunciado.
* Deben usarse estructuras de datos adecuadas para representar los diferentes elementos que intervienen en el problema.
* Capacidad del programador(a) de introducir cambios en el programa desarrollado.
* Se comprobará que el código que el alumnado escribe se adhiere a las reglas de la Guía de Estilo.
* El código ha de estar documentado con [JSDoc](https://jsdoc.app/). 
  Haga que la documentación del programa generada con JSDoc esté disponible a través de una web alojada en su máquina IaaS de la asignatura.
* El alumnado ha de acreditar su capacidad para configurar y ejecutar ESLint en sus programas.
* El alumnado ha de acreditar que sabe depurar sus programas usando Visual Studio Code.
* Se comprobarán los tests unitarios que el alumnado ha desarrollado para todos sus códigos usando Mocha y Chai.
* El alumnado ha de acreditar su capacidad para ejecutar los tests unitarios desde la interfaz de Visual
  Studio Code.

### Indicaciones de caracter general
Configure un fichero `package.json` diferente para cada uno de sus "proyectos" (ejercicios)
de modo que ejecutando `npm install` queden instaladas todas las dependencias del proyecto.

Algunos de los programas correspondientes a los ejercicios 1-5 de esta práctica ya han sido realizados en
sesiones de prácticas anteriores, de modo que los tests unitarios que se propone desarrollar serían 
desarrollados *a posteriori*. 
Esta no es la práctica habitual al seguir la metodología TDD sino que los tests (al igual que la
documentación) han de comenzar a desarrollarse **antes** de desarrollar el código.
Ello no es óbice para que tanto los tests como la documentación se revisen convenientemente conforme se
refactoriza el código.
Si no hubiera realizado Ud. anteriormente cualquiera de esos ejercicios, desarrolle sus correspondientes
tests usando Mocha y Chai antes de proceder a desarrollar los programas.

En cualquier caso diseñe e implemente sus propios tests en Mocha y Chai y verifique que sus programas pasan
estos tests **antes** de revisar los tests (usando Jest) que Exercism proporciona.

Independientemente de cómo se implemente una función, el desarrollador conoce de antemano los resultados que
esa función debe entregar como correctos.
Recuerde asimismo que los tests de código son en sí mismo programas y como tales han de estar correctamente
documentados.
El *hook* *describe* es posiblemente la mejor herramienta para la documentación de sus tests, pero no ha de
ser la única.
Incluya comentarios de cabecera también en los ficheros `*.spec.js` de pruebas de código.

En esta práctica y las siguientes se promoverá el uso del paradigma orientado a objetos.
Así pues los programas estarán organizados en torno a clases que se han de implementar usando la sintaxis para
clases de JavaScript y poniendo en práctica los principios de abstracción y encapsulamiento característicos 
de la Programación Orientada a Objetos.
Vigile siempre el tipo de visibilidad que elige para los atributos (properties) de sus clases
y tenga en cuenta tanto las reglas de 
[estilo](https://google.github.io/styleguide/jsguide.html#features-classes)
como las 
[etiquetas JSDoc](https://stackoverflow.com/questions/41715994/how-to-document-ecma6-classes-with-jsdoc)
relacionadas con el constructo 'class'.

### 1.- Tests uniarios para *Prime Factors*
Cree un nuevo proyecto tomando como punto de partida el programa `prime-factors.js` que resuelve el problema
[*Prime Factors*](https://exercism.io/my/solutions/fce10654772240b3b22955cd5aeb855a)
del *track* de JavaScript de 
[Exercism](https://exercism.io/my/tracks/javascript).
Configure su proyecto para realizar tests usando Mocha y Chai.
A continuación diseñe y desarrolle tests unitarios para acreditar la corrección del programa
`prime-factors.js`.
Se propone que diseñe e implemente sus tests sin revisar los tests que Exercism suministra para este ejercicio.
Compruebe que el programa pasa todos los tests que desarrolle.
Compare finalmente los tests que Ud. ha desarrollado con los que la plataforma Exercism propone para ese mismo
problema.

### 2.- Tests uniarios para *Strain*
Repita el ejercicio anterior, pero en este caso para el programa `strain.js` correspondiente al problema
[*Strain*](https://exercism.io/my/solutions/03d029e7331642fd8a15501eb1ae64bf)
de Exercism.

### 3.- Tests uniarios para *Sieve*
Repita el ejercicio 1 para el programa `sieve.js` correspondiente al problema
[*Sieve*](https://exercism.io/my/solutions/6b48d3e059014849952c2886ac3ba9bd)
de Exercism.

### 4.- Tests uniarios para *Sum of Multiples*
Repita el ejercicio 1 para el programa `sum-of-multiples.js` correspondiente al problema
[*Sum of Multiples*](https://exercism.io/my/solutions/f51f679400aa4d93a1b278c4bd73d5b8)
de Exercism.

### 5.- Tests uniarios para *Roman Numerals*
Repita el ejercicio 1 para el programa `roman-numerals.js` correspondiente al problema
[*Roman Numerals*](https://exercism.io/my/solutions/5bd5622efab448d9b12233e779696a41)
de Exercism.

### 6.- La clase *Clock*
En este ejercicio se propone desarrollar un módulo ES6 que implemente una clase `Clock` 
para representar un reloj digital con horas y minutos. No es necesario contemplar segundos.

La clase no ha de usar en modo alguno objetos 
[Date](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Date)
de JavaScript y se desarrollará usando la sintaxis para clases de JavaScript y poniendo en práctica los principios de
abstracción y encapsulamiento característicos de la Programación Orientada a Objetos.

La clase ha de contener un método *toString()* que permita imprimir en pantalla un objeto *Clock* en el
formato `hh:mm`.
La clase ha de contemplar métodos que permitan sumar y restar minutos a un objeto *Clock*.
Análogamente, dos objetos que representen la misma hora deben ser iguales entre sí.
Incluya discrecionalmente cualesquiera otras operaciones que considere adecuadas como métodos en la clase `Clock`.

Previo a la implementación de la clase, diseñe y desarrolle un conjunto de tests para probar el correcto
funcionamiento de todos los métodos de la clase.

Encapsule la clase en un módulo que exporte la misma hacia otros programas clientes que pudieran utilizarla.

Desarrolle un programa *cliente* que utilice la clase *Clock* e instancie objetos de esa clase:
```javascript
const horaActual = new Clock(11, 59);
console.log(horaActual.toString());   // 11:59h
```

### 7.- La clase *Complejo*
Un
[número complejo](https://es.wikipedia.org/wiki/N%C3%BAmero_complejo)
puede representarse como la suma de un número real y un número imaginario, de la forma `a + bi` donde el
término `a` es la parte real, `b` la parte imaginaria e `i` la
[unidad imaginaria](https://es.wikipedia.org/wiki/Unidad_imaginaria).

En este ejercicio se propone desarrollar un módulo ES6 que implemente una clase `Complejo` que permita operar con números complejos.
La clase se desarrollará usando la sintaxis para clases de JavaScript y poniendo en práctica los principios de
abstracción y encapsulamiento característicos de la Programación Orientada a Objetos.

La clase ha de contener al menos métodos que permitan las siguientes operaciones con números complejos:

* `print` Imprimir un número complejo 
* `add` Sumar 
* `sub` Restar
* `mul` Multiplicar
* `div` Dividir
* `abs` Calcular el valor absoluto
* `conj` Calcular el conjugado de un número complejo

Incluya discrecionalmente cualesquiera otras operaciones que considere adecuadas como métodos en la clase `Complejo`.

Previo a la implementación de la clase, diseñe y desarrolle un conjunto de tests para probar el correcto
funcionamiento de todos los métodos de la clase.

Desarrolle un programa cliente `complejos.js` que permita operar con números complejos y haga uso de la clase `Complejo` que diseñe.
El programa cliente definirá un par de números complejos `-1-5i` y `1+i` y realice todas las operaciones
anteriores utilizando ambos números como operandos.
