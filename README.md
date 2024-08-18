# What is C:
C is a **powerful, general-purpose** programming language that allows you to write **efficient programs**. It provides **low-level access** to memory and system resources, making it ideal for system programming like operating systems. C's syntax and structure are foundational, influencing many modern programming languages like C++ and Java.
# Starting:
This is **a simple c starting** code:
```c
#include <stdio.h>

int main(void) {
  printf("Ahmed notes\n");
  return 0;
}
```
note: "void" in:
```c
int main(void)
```
is optional, which means the code can be written as:
```c
#include <stdio.h>

int main() {
  printf("Ahmed notes\n");
  return 0;
}
```

**Note:** you don't need to worry about the "starting code". In fact, you can just copy it and you'll get used to it. 

## Comments:

A comment in C is a way to include notes or explanations in your code that the compiler ignores, helping to make the code more understandable. There are two types of comments in C:
1. **Single-line comment:** Begins with `//` and extends to the end of the line.
```c
#include <stdio.h>
// This is a comment
// This is another comment
int main() {
  printf("Ahmed notes\n");
  return 0;
}
```
2. **Multi-line comment:** Begins with `/*` and ends with `*/`, and can span multiple lines.
```c
#include <stdio.h>
/* This is a
multi-line 
comment */
int main() {
  printf("Ahmed notes\n");
  return 0;
}
```

## Escape sequences:
Escape sequences in C are special sequences of characters used to represent certain special characters within strings or character literals. They start with a backslash (`\`) followed by one or more characters. Here are some common escape sequences in C:

- `\n` : Newline (moves the cursor to the next line)
- `\t` : Horizontal tab (adds a tab space)
- `\\` : Backslash (inserts a `\` character)
- `\"` : Double quote (inserts a `"` character)
- `\'` : Single quote (inserts a `'` character)
**Example:**
using `\n`
```c
#include <stdio.h>
int main() {
  printf("Ahmed notes\n");
  return 0;
}
```
Now lets try to write every word in a new line:
```c
#include <stdio.h>
int main() {
  printf("Ahmed\nnotes\nare\ndecent");
  return 0;
}
```
the output would be:
```
Ahmed
notes
are
decent
```

# Variables:
In C, a variable is a named storage location in memory used to hold a value that can be changed during program execution. 
Variables are defined by specifying a data type (like `int`, `float`, `char`) followed by the variable name.
 1. **`int` (Integer)**
- Used to store whole numbers.
- Example:
```c
int age = 25;
```

2. **`float` (Floating Point)**
- Used to store single-precision decimal numbers.
- Example:
```c
float temperature = 36.5;
```

3. **`double` (Double Precision Floating Point)**
- Used to store double-precision decimal numbers (more accurate than `float`).
- Example:
```c
double pi = 3.14159;
```

4. **`char` (Character)**
- Used to store a single character.
- Example:
```c
char grade = 'A';
```

5. **`_Bool` (Boolean)**
- Used to store a boolean value (true or false). Available in C99 and later.
- Example:
```c
_Bool isTrue = 1; // 1 represents true, 0 represents false
```

**Full version:**
```c
int age = 25;
float temperature = 36.5;
double pi = 3.14159;
char grade = 'A';
_Bool isTrue = 1; // 1 represents true, 0 represents false
```

**Note:** for strings you can use something called an "array", to do that you just type:
```c
char name[] = "Ahmed";
```

### Displaying Variables:
**printf(); ==  أظهر على الشاشة**

In C, you can display the values of variables using the `printf` function, which is part of the C standard library. The `printf` function uses format specifiers to determine how the values should be displayed.

Here's how you can display different types of variables:

1. **`int` (Integer)**
- Format Specifier: `%d`
- Example:
```c
int age = 25;
printf("Age: %d\n", age);

//Output:
// Age: 25
```

2. **`float` (Floating Point)**
- Format Specifier: `%f`
- Example:
```c
float temperature = 36.5;
printf("Temperature: %.2f\n", temperature); // .2 specifies two decimal places

//Output:
// Temperature: 36.5
```

3. **`double` (Double Precision Floating Point)**
- Format Specifier: `%lf`
- Example:
```c
double pi = 3.14159;
printf("Value of Pi: %.5lf\n", pi); // .5 specifies five decimal places

//Output:
// Value of Pi: 3.14159
```

4. **`char` (Character)**
- Format Specifier: `%c`
- Example:
```c
char grade = 'A';
printf("Grade: %c\n", grade);

//Output:
// Grade: A
```

5. **`_Bool` (Boolean)**

- Format Specifier: `%d` (Booleans are typically displayed as integers, where `1` is true and `0` is false)
- Example:
```c
_Bool isTrue = 1;
printf("Boolean Value: %d\n", isTrue);

//Output:
// Boolean Value: 1
```
