tarea
=====

Un unit test es un método que prueba una unidad de código. Al hablar de una unidad de código nos referimos a un requerimiento. Muchos desarrolladores tienen su propio concepto de lo que es una prueba unitaria; sin embargo, la gran mayoría coincide en que una prueba unitaria tiene las siguientes características: Prueba solamente pequeñas cantidades de código: Solamente prueba el código del requerimiento específico. Se aísla de otro código y de otros desarrolladores: El unit test prueba exclusivamente el código relacionado con el requerimiento y no interfiere con el trabajo hecho por otros desarrolladores. Solamente se prueban los endpoints públicos: Esto principalmente porque los disparadores de los métodos privados son métodos públicos por lo tanto se abarca el código de los métodos privados dentro de las pruebas. Los resultados son automatizados: Cuando ejecutamos las pruebas lo podemos hacer de forma individual o de forma grupal. Estas pruebas las hace el motor de prueba y los resultados de los mismos deben de ser precisos con respecto a cada prueba unitaria desarrollada Repetible y predecible: No importa el orden y las veces que se repita la prueba, el resultado siempre debe de ser el mismo. Son rápidos de desarrollar: Contrariamente a lo que piensan los desarrolladores –> que el desarrollo de pruebas unitarias quita tiempo – los unit test por lo general deben de ser simples y rápidos de desarrollar. Difícilmente una prueba unitaria deba de tomar más de cinco minutos en su desarrollo.
sus herramientas son 
JUnit: Entorno de pruebas para Java creado por Erich Gamma y Kent Beck. Se encuentra basado en SUnit creado originalmente para realizar pruebas unitarias para el lenguaje Smalltalk.
TestNG: Creado para suplir algunas deficiencias en JUnit.
JTiger: Basado en anotaciones, como TestNG.
SimpleTest: Entorno de pruebas para aplicaciones realizadas en PHP.
PHPUnit: Sistema para la realización pruebas unitarias en PHP.
CPPUnit: Versión del framework para lenguajes C/C++.
NUnit: Versión del framework para la plataforma.NET.
FoxUnit: Entorno OpenSource de pruebas unitarias para Microsoft Visual FoxPro
MOQ: Entorno para la creación dinámica de objetos simuladores (mocks). «MOQ».
QUnit: Librería para pruebas unitarias en Javascript. Creada por la fundación jQuery, ha sido reescrita para ser independiente de la librería jQuery.
libunittest: Librería portable para pruebas unitarias en C++ que usa el nuevo estándar C++11.

herencias en c++
La 'herencia' es una de las piedras angulares de la POO ya que ésta permite la creación de clasificaciones jerárquicas. Con la herencia, es posible crear una clase general que defina tratos comunes a una serie de elementos relacionados. Esta clase podría luego ser heredada por otras clases más específicas, cada una agregando solo aquellas cosas que son únicas para la clase 'heredera'.
En terminología estándar C++, una clase que es heredada es referida como la clase 'base'. La clase que efectúa la herencia es llamada la clase 'derivada'. Además, una clase derivada puede ser usada como una clase base por otra clase derivada. De esta manera, una jerarquía multicapa de clases puede ser lograda.
conceptos de herencias
 Pertenencia (TIENE-UN) -> Relaciones todo-parte
 Variedad (ES-UN) -> Herencia
ejemplos de herencias
class Figura2D {
 public:
 ...
 void setColor(Color c);
 Color getColor() const;
 private:
 Color colorRelleno;
... }; 
class Circulo : Figura2D {
...
 public:
 void vaciarCirculo() {
 colorRelleno=NINGUNO; 
 // ¡ERROR! colorRelleno es privado
 setColor(NINGUNO); // OK
 }
}

