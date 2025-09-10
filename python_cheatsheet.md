# Python Cheat Sheet

A quick reference guide for common Python functions, operations, and concepts.

---

## 1. Printing & Comments
| Concept       | Description | Example |
|---------------|------------|---------|
| `print()`     | Shows output on the screen | `print("Hello World")` → Hello World |
| `# Comment`   | Notes for yourself, ignored by Python | `# This is a comment` |


---
## 2. Variables

| Concept   | Description | Example |
|-----------|------------|---------|
| Variable  | Stores data | `x = 5`<br>`name = "Alice"` |
| Rules     | Letters, numbers, `_` (no spaces, can’t start with number) | `my_var = 10` |

---

## 3. Data Types

| Type   | Description | Example |
|--------|------------|---------|
| int    | Whole numbers | `5, -3` |
| float  | Decimal numbers | `3.14, -0.5` |
| str    | Text | `"Hello"` |
| bool   | True or False | `True, False` |

---
## 4. Basic Math

| Operator | Description | Example |
|----------|------------|---------|
| `+`      | Addition | `2 + 3 → 5` |
| `-`      | Subtraction | `5 - 2 → 3` |
| `*`      | Multiplication | `2 * 3 → 6` |
| `/`      | Division | `5 / 2 → 2.5` |
| `//`     | Floor division | `5 // 2 → 2` |
| `%`      | Modulus (remainder) | `5 % 2 → 1` |
| `**`     | Power | `2 ** 3 → 8` |

---

## 5. Lists

| Concept | Description | Example |
|---------|------------|---------|
| List    | Store multiple values | `numbers = [1, 2, 3]` |
| `len()` | Count items | `len(numbers) → 3` |
| `sum()` | Add numbers | `sum(numbers) → 6` |
| `append()` | Add item to list | `numbers.append(4)` |
| `pop()` | Remove last item | `numbers.pop()` |

---

## 6. Conditionals

| Statement | Description | Example |
|-----------|------------|---------|
| `if`      | Run code if condition is True | `if x > 5:` |
| `elif`    | Run if previous `if`/`elif` False | `elif x == 5:` |
| `else`    | Run if all previous conditions False | `else:` |
| `==`      | Equal to | `if x == 5:` |
| `!=`      | Not equal | `if x != 5:` |

---

| Concept               | Description | Example |
|-----------------------|------------|---------|
| `def`                 | Define a function | `def greet(name):` |
| Parameters / Arguments| Input values a function uses | `def greet(name): return "Hello " + name`<br>`greet("Alice")` |
| Default Parameters    | Provide a default if no argument is given | `def greet(name="Guest"): return "Hello " + name`<br>`greet() → "Hello Guest"` |
| Multiple Parameters   | Functions can take more than one parameter | `def add(a, b): return a + b`<br>`add(2, 3) → 5` |
| Keyword Arguments     | Pass arguments by name | `greet(last_name="Smith", first_name="John") → "Hello John Smith"` |
| `return`              | Sends a value back from the function | `def add(a, b): return a + b` |
| `print()`             | Shows output on the screen, does not return a value | `def add_and_print(a, b): print(a + b)` |

### Parameter vs Argument

| Term       | Definition                                   | Example |
|-----------|----------------------------------------------|---------|
| Parameter | Variable in the function definition, a placeholder | `def greet(name):` → `name` is the parameter |
| Argument  | Actual value passed to the function when calling it | `greet("Alice")` → `"Alice"` is the argument |
| Usage     | Can be used inside the function to perform operations | `"Hello " + name` → concatenates "Hello " with the parameter value |
