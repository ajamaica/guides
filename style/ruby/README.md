Ruby
====

[Muestra](sample.rb)

* Evitar modificadores de condicionales (líneas que terminan con condicionales).
* Evitar múltiples asociaciones por línea (`one, two = 1, 2`).
* Evitar comentarios de organización (`# Validations`).
* Evitar operadores ternarios (`boolean ? true : false`). Usar multilínea `if`
  para resaltar ramas de código.
* Evitar declaraciones explícitas de retorno.
* Evitar usar puntos y comas.
* Evitar nombres de métodos bang (!). Se prefieren nombres descriptivos.
* No usar explícitamente `self` en cualquier lugar excepto en las clases del método (`def self.method`)
  y en asignaciones (`self.attribute =`).
* Preferir clases anidadas y definiciones de módulos sobre versiones cortas.
  [Ejemplo][class definition example]
* Preferir `detect` sobre `find`.
* Preferir `select` sobre `find_all`.
* Preferir `map` sobre `collect`.
* Preferir `reduce` sobre `inject`.
* Preferir comillas dobles para los strings.
* Preferir `&&` y `||` sobre `and` y `or`.
* Preferir `!` sobre `not`.
* Preferir `&:method_name` a `{ |item| item.method_name }` para llamadas a métodos simples.
* Preferir `if` sobre `unless`.
* Usar `_` para bloques de parámetros que no han sido usados.
* Usar guion bajo (`_`) para variables que no han sido utilizadas así como parámetros de funaciones.
* Usar un guion para definir variables de instancia para memorización.
* Usar `%{}` para strings de una sola línea que necesitan interpolación y comillas dobles.
* Usar `{...}` para bloques de una sola línea. Usar `do..end` para bloques de múltiples líneas.
* Usar `?` para fufijos de métodos de predicado.
* Usar `CamelCase` para clases y módulos, `snake_case` para variables y métodos, `SCREAMING_SNAKE_CASE` para constantes.
* Usar `def self.method` en vez de `def Class.method` o `class << self`.
* Usar `def` con paréntesis cuando hay argumentos.
* No usar espacios después de argumentos requeridos. [Example][required kwargs]
* Usar `each` en vez de `for` para iteración.
* Utilice una coma de arrastre después de cada elemento en una lista de varias líneas, incluido el último elemento. [Example][trailing comma example]
* Usar heredocs para stings de múltiples líneas.
* Preferir `private` sobre `protected` para `attr_reader`,
  `attr_writer`, y `attr_accessor` de manera pública.
* Ordenar los métodos de la clase sobre las instancias de los métodos.
* Preferir invocación de métodos sobre instanciación de métodos.

[trailing comma example]: /style/ruby/sample.rb#L53
[required kwargs]: /style/ruby/sample.rb#L16
[class definition example]: /style/ruby/sample.rb#L103
