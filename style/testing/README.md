Testing
=======

* Evita la palabra `private` en specs.
* Evita verificar la igualdad booleana directamente. En su lugar, escriba métodos predicados y
Utilice los matchers apropiados. [Example][predicate-example].
* Preferir `eq` a `==` en RSpec.
* Separar las fases de configuración, ejercicios, verificación y demolición.
* Usar RSpec's [`expect` syntax].
* Usar RSpec's [`allow` syntax] para métodos stubs.
* Usar `not_to` en vez de `to_not` en RSpec expectations.
* Preferir `have_css` a `have_selector`en afirmaciones Capybara.

[`expect` syntax]: http://myronmars.to/n/dev-blog/2012/06/rspecs-new-expectation-syntax
[`allow` syntax]: https://github.com/rspec/rspec-mocks#method-stubs
[predicate-example]: predicate_tests_spec.rb

Pruebas de Aceptación
----------------

[Sample](acceptance_test_spec.rb)

* Evitar títulos de escenarios que no dan información esencial.
* Evitar títulos de escenarios que repitan el título de la característica.
* Coloca los métodos de ayuda para los specs direncatamente en el nivel más alto del módulo `Features`.
* Usar Capybara's `feature/scenario` DSL.
* Usar nombres `ROLE_ACTION_spec.rb`, como
  `user_changes_password_spec.rb`, para los specs del archivo.
* Usar solo un bloque `feature` para cada futuro spec en el archivo.
* Usar títulos del escenario que describa el éxito o falla de los caminos.
* Usar directorio de spec/features para guardar los futuros specs.
* Usar el directorio spec/support/features para soporte de código relacionado a futuros specs.

Factories
---------

* Ordenar los contenidos de `factories.rb`: secuencias, traits, definiciones de factories.
* Ordenar los atributos: atributos implícitos, atributos explícitos,
  definiciones de hijos de factories. Los atributos de cada sección deben de estar en orden alfabético.
* Ordenar alfabéticamente las definiciones por el nombre de la factory.
* Usar un archivo factories.rb por cada proyecto.

Pruebas Unit
----------

[Sample](unit_test_spec.rb)

* No usar el prefijo `it` bloquear descripciones con `should`. Usar [modo imperativo]
* Usar bloque `subject` para definir objetos para uso de una línea de los specs.
  [Ejemplo][subject for one-liners example].
* Poner specs de una línea al principio del bloque de `describe`.
* Usar `.method` para describir los métodos de la clase y `#method` para describir la instancia de los métodos.
* Usar `context` para describir las precondiciones de las pruebas.
* Usar `describe '#method_name'` para agrupar puebas método-bajo-prueba..
* Usar un solo bloque de alto nivel `describe ClassName`.
* Ordenar validación, asociación, pruebas de métodos en el mismo orden en que aparecen el las clases.

[modo imperativo]: http://en.wikipedia.org/wiki/Imperative_mood
[subject for one-liners example]: unit_test_spec.rb#6
