

> **Tip importante:** Para resolver este challenge no estás obligado a usar un único tipo de dato.

Puedes decidir si quieres que los atributos internos de tu clase sean:

- **Números (`int`)**, trabajando siempre como enteros.
- **Texto (`String`)**, manejando signos y formatos más manualmente.
- **Una mezcla**, si te resulta más claro.

---
> Estos son algunos metodos propios de Java que te pueden servir para solucionar el ejercicio
###  Métodos útiles

| Método | ¿Qué hace? | Ejemplo |
| --- | --- | --- |
| `startsWith(String prefix)` | Verifica si un texto comienza con un prefijo dado. | `"−5".startsWith("-")` → `true` |
| `substring(int beginIndex)` | Extrae parte del texto a partir de una posición. | `"−5".substring(1)` → `"5"` |
| `String.valueOf(int n)` | Convierte un número a `String`. | `String.valueOf(5)` → `"5"` |
| `equals(String other)` | Compara si dos textos son exactamente iguales.**Cuidado:** no uses `==` para comparar textos.  | `"0".equals("0")` → `true` |
| `Math.abs(int n)` | Devuelve el valor absoluto de un número. | `Math.abs(-7)` → `7` |

---
A continuación se te sugieren algunas ideas de como puedes plantear la clase Fraccion (**esto solo es una guia**) y estas en total libertad de añadir o quitar metodos y atributos, todo depende de tu logica de porgramación.

### Plantilla guia si quieres tratar los atributos como enteros `int`

**Ventajas:**
- Cálculos directos y eficientes.
- Código más corto y claro para operaciones numéricas.
- No necesitas convertir constantemente entre tipos (`String` ↔️ `int`)

---

```java
public class Fraccion {
    // Atributos
    private int numerador;
    private int denominador;

    // Constructor
    public Fraccion(int numerador, int denominador) {
        
    }

    // Método para verificar si la fracción es válida (denominador diferente de cero)
    private boolean esValida() {
        // Implementa la validacion
        return true;
    }

    // Método para mostrar la fracción en su forma  propia o impropia, piensa en los posibles casos
    //que pueden existir, ej (numerado igual a cero)
    public String neutral() {
        return ""; // Completa la lógica
    }

    // Método para mostrar la fracción como número mixto, de nuevo, piensa en todos los posibles casos
    // que pueden existir.
    public String aMixto() {
        return ""; // Completa la lógica
    }
}
```
### Plantilla guia si quieres tratar los atributos como cadenas de texto

**Ventajas:**
- Más control sobre cómo mostrar el resultado.
- Facilita manejar el signo al imprimir.

**Desventajas:**
- Se necesita convertir entre `String` e `int` para hacer calculos matematicos.
- El codigo se extiend unas lineas de mas
  
```java
public class Fraccion {
    // Atributos
    private String num;
    private String denom;
    private String entero; // Podrías necesitarlo para representar parte entera
    private String sign = "";

    // Constructor
    public Fraccion(int nume, int denomi) {
    }

    // Método para asignar el signo de la fracción
    private void setSign(int n, int d) {
        // Si el producto de n*d es negativo, el signo es "-"
        // De lo contrario, el signo es vacío ""
    }

    // Método para verificar si la fracción es válida (denominador distinto de "0")
    private boolean valida() {
        // Implementa la validacion
        return true; // Cambia por la condición correcta
    }

    // Método para mostrar la fracción en su forma propia o impropia (pienas en todos los posibles casos)
    public String neutral() {
        return ""; // Completa la lógica
    }

    // Método para mostrar la fracción como número mixto, de nuevo piensa en todos los posibles casos
    public String toMixt() {
        return ""; // Completa la lógica
    }
}
```

---
