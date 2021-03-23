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
A la hora de resolver los problemas que se le proponen, trate de usar exclusivamente las características de
JavaScript que ha estudiado en clase o bien en el material que se le ha pedido que estudie.

Descarte soluciones avanzadas y nunca utilice código que no sea Ud. capaz de comprender y explicar a otra
persona.

Puesto que en la práctica anterior ya se ha trabajado con módulos CommonJS se propone aquí que
la aplicación que desarrolle se organice utilizando
[módulos ES6](https://blog.logrocket.com/es-modules-in-node-today/)

Configure un fichero `package.json` en el directorio raíz de su repositorio de modo que ejecutando 
`npm install` queden instaladas todas las dependencias de su proyecto.

### Tests uniarios para *Prime Factors*
Cree un nuevo proyecto tomando como punto de partida el programa `prime-factors.js` que resuelve el problema
[*Prime Factors*](https://exercism.io/my/solutions/fce10654772240b3b22955cd5aeb855a)
del *track* de JavaScript de 
[Exercism](https://exercism.io/my/tracks/javascript).
Configure su proyecto para realizar tests usando Mocha y Chai.
A continuación diseñe y desarrolle tests unitarios para acreditar la corrección del programa
`prime-factors.js`.
Se propone que diseñe sus tests sin revisar los tests que Exercism suministra para este ejercicio.
Compruebe que el programa pasa todos los tests que desarrolle.
Compare finalmente los tests que Ud. ha desarrollado con los que la plataforma Exercism propone para ese mismo
problema.

### Tests uniarios para *Strain*
Repita el ejercicio anterior, pero en este caso para el programa `strain.js` correspondiente al problema
[*Strain*](https://exercism.io/my/solutions/03d029e7331642fd8a15501eb1ae64bf)
de Exercism.

### Tests uniarios para *Sieve*
Repita el ejercicio anterior, pero en este caso para el programa `sieve.js` correspondiente al problema
[*Sieve*](https://exercism.io/my/solutions/6b48d3e059014849952c2886ac3ba9bd)
de Exercism.

### Tests uniarios para *Sum of Multiples*
Repita el ejercicio anterior, pero en este caso para el programa `sieve.js` correspondiente al problema
[*Sieve*](https://exercism.io/my/solutions/6b48d3e059014849952c2886ac3ba9bd)
de Exercism.

### Tests uniarios para *Roman Numerals*
Repita el ejercicio anterior, pero en este caso para el programa `roman-numerals.js` correspondiente al problema
[*Roman Numerals*](https://exercism.io/my/solutions/5bd5622efab448d9b12233e779696a41)
de Exercism.

