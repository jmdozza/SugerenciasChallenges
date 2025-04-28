
> **Tip importante:** No estás obligado a usar un único tipo de datos.

Puedes decidir si quieres que los atributos internos de tu clase sean:

- **Números (`int`)**, trabajando siempre como enteros.
- **Texto (`String`)**, manejando signos y formatos más manualmente.
- **Una mezcla**, si te resulta más claro.

---

###  Métodos de `String` útiles

| Método | ¿Para qué sirve? | Ejemplo |
| --- | --- | --- |
| `startsWith("-")` | Saber si un texto empieza con signo negativo. | `"−5".startsWith("-")` → `true` |
| `substring(int)` | Obtener una parte de un texto desde cierta posición. | `"−5".substring(1)` → `"5"` |
| `valueOf(int)` | Convertir un número a `String`. | `String.valueOf(5)` → `"5"` |
| `equals(String)` | Comparar si dos textos son iguales. **Cuidado:** no uses `==` para comparar textos. | `"0".equals("0")` → `true` |


---
A continuación se le sugiere al programador algunas ideas de como puede plantear la clase Fraccion, **esto solo es una guia** y el programador esta en total libertad de diseñarla segun sus necesidades
### Plantilla sugerida si usas `int`

```java
public class Fraccion {
    private int numerador;
    private int denominador;
    
    public Fraccion(int numerador, int denominador) {
        // Validar y normalizar signos
    }
    
    public String neutral() {
        // Implementar
        return "";
    }
    
    public String aMixto() {
        // Implementar
        return "";
    }
}
```

---

### Plantilla sugerida si usas `String`

```java
public class Fraccion {
    private String numerador;
    private String denominador;
    private String signo = "";
    
    public Fraccion(int num, int den) {
        // Convertir y preparar los strings
    }
    
    private boolean valida() {
        // Implementar validación
        return false;
    }
    
    public String neutral() {
        // Implementar
        return "";
    }
    
    public String aMixto() {
        // Implementar
        return "";
    }
}
```

---
