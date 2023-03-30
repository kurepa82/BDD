# BDD
## Gherkin 
Es un lenguaje de especificación utilizado en BDD (Behavior Driven Development), que permite describir el comportamiento de un sistema de software en un formato fácil de entender para todas las partes interesadas, incluyendo desarrolladores, testers, analistas y usuarios finales.

Las palabras clave se utilizan para describir los diferentes pasos que se llevan a cabo en un escenario, 
- Given (Dado)
- When (Cuando) 
- Then (Entonces)

Los argumentos se utilizan para proporcionar información específica sobre un paso, como el nombre de usuario o contraseña en un escenario de login. Los comentarios se utilizan para proporcionar información adicional o para hacer notas sobre el escenario en sí.

## Ejemplo

Supongamos que queremos implementar la funcionalidad de login de una página web. Un escenario BDD para esta funcionalidad podría ser el siguiente:

- **Dado** que estoy en la página de login
- **Cuando** introduzco mi nombre de usuario y contraseña válidos
- **Entonces** debo ser redirigido a la página de inicio de sesión

A partir de este escenario, se podrían escribir pruebas automatizadas utilizando un framework BDD para comprobar que la funcionalidad de login se comporta de acuerdo con los requisitos establecidos. Un ejemplo de código en Gherkin, un lenguaje de especificación utilizado en BDD, podría ser el siguiente:
```
Feature: Login
  Como usuario de la página web
  Quiero poder iniciar sesión en mi cuenta
  Para acceder a mi contenido personal

  Scenario: Iniciar sesión con éxito
    Given que estoy en la página de login
    When introduzco mi nombre de usuario y contraseña válidos
    Then debo ser redirigido a la página de inicio de sesión

  Scenario: Iniciar sesión con nombre de usuario incorrecto
    Given que estoy en la página de login
    When introduzco un nombre de usuario incorrecto y una contraseña válida
    Then debo ver un mensaje de error indicando que el nombre de usuario es incorrecto

  Scenario: Iniciar sesión con contraseña incorrecta
    Given que estoy en la página de login
    When introduzco un nombre de usuario válido y una contraseña incorrecta
    Then debo ver un mensaje de error indicando que la contraseña es incorrecta
 ```

En estas pruebas se utilizarían herramientas de automatización de pruebas web para simular la interacción del usuario con la página web y verificar que el resultado coincide con el esperado en cada uno de los escenarios definidos.

Existen varias herramientas web para hacer BDD (Behavior Driven Development), a continuación se mencionan algunas de ellas:

- Cucumber: es una herramienta muy popular para la automatización de pruebas en BDD. Es compatible con varios lenguajes de programación, como Java, Ruby, JavaScript, entre otros.

- Behave: es una herramienta para Python que permite escribir pruebas BDD de manera sencilla y clara. Se integra con varias librerías de Python para la ejecución de pruebas.

- SpecFlow: es una herramienta para .NET que permite escribir pruebas BDD en lenguaje natural y las convierte en código para su ejecución. Es compatible con varios lenguajes .NET, como C# y Visual Basic.

- JBehave: es una herramienta para Java que permite escribir pruebas BDD en lenguaje natural. Se integra con varias herramientas de construcción, como Maven y Gradle.

- Gauge: es una herramienta de código abierto para la automatización de pruebas BDD. Es compatible con varios lenguajes de programación, como Java, Ruby, C#, entre otros.

- Robot Framework: es una herramienta de automatización de pruebas que soporta BDD. Es compatible con varios lenguajes de programación y es muy flexible en cuanto a la definición de las pruebas.

