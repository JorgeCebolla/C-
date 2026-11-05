Carlos Candela, Jorge Cebolla
Bucle en C#

## 1. Declaración de Variables

En Python las variables no llevan tipo explícito (tipado dinámico):
```python
# Python
edad = 25
nombre = "Carlos"
precio = 9.99
activo = True
```

En C#, por regla general, **debes indicar el tipo de dato** antes del nombre de la variable y terminar con punto y coma (`;`):
```csharp
// C#
int edad = 25;               // Números enteros
string nombre = "Carlos";    // Texto (comillas dobles obligatorias)
double precio = 9.99;        // Decimales
bool activo = true;          // Booleano (en minúsculas: true/false)
```

---

## 2. Delimitación de Bloques de Código

* **Python:** Delimita el código mediante **sangría / indentación** (espacios o tabuladores) y dos puntos (`:`).
* **C#:** Delimita el código mediante **llaves (`{ }`)** y finaliza cada instrucción con **punto y coma (`;`)**.

### Comparativa:

**En Python:**
```python
if edad >= 18:
    print("Mayor de edad")
    print("Bienvenido")
```

**En C#:**
```csharp
if (edad >= 18)
{
    Console.WriteLine("Mayor de edad");
    Console.WriteLine("Bienvenido");
}
```

---

## 3. ¿Qué cambia en la sintaxis respecto a Python?

| Aspecto | Python | C# |
|---|---|---|
| **Fin de instrucción** | Salto de línea | Punto y coma (`;`) obligatorio |
| **Bloques** | Indentación | Llaves (`{ }`) |
| **Condiciones** | `if edad > 10:` | Paréntesis obligatorios: `if (edad > 10)` |
| **Imprimir en pantalla** | `print("hola")` | `Console.WriteLine("hola");` |
| **Comentarios** | `# comentario` | `// línea` o `/* bloque */` |
| **Booleanos** | `True`, `False`, `None` | `true`, `false`, `null` |
| **Operadores lógicos** | `and`, `or`, `not` | `&&`, `\|\|`, `!` |

---

## 4. ¿Qué parte de la lógica se mantiene igual?

La forma de pensar y resolver problemas es exactamente la misma:
1. **Flujo de control:** La lógica de `if`, `else if` (en Python `elif`) y `else` funciona idéntica.
2. **Operadores de comparación:** `==`, `!=`, `<`, `>`, `<=`, `>=` funcionan exactamente igual.
3. **Conceptos de bucles:** La idea de iterar un número determinado de veces o mientras se cumpla una condición es la misma (`while`, `for`).
4. **Funciones y retorno:** Ambas manejan parámetros de entrada, ejecución interna y retorno de valores (`return`).

---

## 5. Ejemplo de bucle: Contar del 1 al 5

### En Python:
```python
for i in range(1, 6):
    print(i)
```

### En C#:
```csharp
for (int i = 1; i <= 5; i++)
{
    Console.WriteLine(i);
}
```
* `int i = 1;` $\rightarrow$ Valor inicial.
* `i <= 5;` $\rightarrow$ Condición para continuar.
* `i++` $\rightarrow$ Incremento en 1 en cada paso (equivalente a `i += 1`).
