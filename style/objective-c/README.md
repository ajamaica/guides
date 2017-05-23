Objective-C
===========

[Sample](sample.m)

* Colocar los `#import` en el prefijo del header (`ProjectName-Prefix.pch`) solo si se usa en _muchos_ archivos.
* Colocar los archivos `.xib` en `Resources/Nibs` y sus archivos de asociaciones  en `Classes/Views`.
* Ordenar las declaraciones del `#import` alfabéticamente.
* Ordenar directivos de `@class` alfabéticamente.
* Ordenar los modificadores de `@property`: manejo de memoria, atomicidad, capacidad de escritura.
* Dejar afuera los modificadores `@property` a menos que sean necesarios, `nonatomic` es la única manera en la mayoría de los casos.
* Se prefiren fuertes referencias a IBOutlet.
* Prefer `@class` to `#import` when referring to external classes in a public
  `@interface`.
* Prefer `@property` to declaring instance variables.
* Utilizar un prefijo de 2 a 3 letras para los acrónimos de los nombres de las clases.
* Utilizar prefijos de strings constantes como llaves con 'k'.
* Quitar declaraciones `#import` para `Foundation` y `UIKit` en plantillas de nuevos proyectos.
* Separar métodos y funciones como `#pragma mark - <Section Name>`.
* Separar secciones en subsecciones como `#pragma mark <Subsection Name>`.
* Usar literales `@[arrayObject]`, `@{@"key" : value}`, `@(YES or NO)`, y `@5.0`.
* Use `@interface ClassName ()` to declare private properties.
* Usar `lowerCamelCase` para los nombres de los métodos.
* Usar `NSAssert` en métodos que requieren la presencia de ciertos argumentos.
* Ecribir métodos usando el camino feliz. Indentar en casos excepcionales. El caso óptimo debe estar en la columna más izquierda.
* Preferir `enumerateObjectsUsingBlock:` cuando se recorren arreglos.
* Siempre usar llaves en bloques de control y de ciclos a menos que se pueda comodar en una sola línea.
* Poner una llave abierta para los bloques de control y de ciclos de una sola línea.
* Preferir `NSInteger`, `CGFloat`, y similares macros cobre `int`, `float`, y
  otros tipos base.
* Preferir *Auto Layout* para view layouts y constraints.
