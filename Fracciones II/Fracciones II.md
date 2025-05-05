###  Sugerencia:

Cuando se trabaja con fracciones en programación, es importante mantenerlas simplificadas para que los resultados sean correctos y consistentes.

Una buena práctica en programación orientada a objetos es **automatizar procesos que deberían ocurrir siempre**, como simplificar una fracción cuando se crea.

####  Tip:

Considera **llamar al método `simplificar()` desde el constructor** de tu clase `Fraccion`, así te aseguras de que toda fracción se cree ya en su forma más simple.

####  Ejemplo:

```java
Fraccion f1 = new Fraccion(4, 6); // si llamas simplificar() en el constructor, se convierte en 2/3
Fraccion f2 = new Fraccion(1, 3);

Fraccion resultado = f1.sumar(f2); // suma 2/3 + 1/3 = 3/3 → se simplifica a 1/1 automáticamente

System.out.println(resultado.mostrar()); // Debería imprimir: 1/1
