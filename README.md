# ft_printf - A Custom Implementation of the C Library printf

**A versatile project focused on mastering variadic functions in C and replicating the core formatting logic of the standard `printf` function.**

## 🧠 Key Learning Objectives

* **🟢 Variadic Functions**: Utilizing `va_start`, `va_arg`, and `va_end` to handle an unknown number of arguments.
* **🔵 String Parsing**: Iterating through a format string to identify and process conversion specifiers.
* **🟡 Recursion & Bases**: Implementing recursive logic to handle number conversions (Decimal, Hexadecimal).
* **🔴 Return Value Management**: Accurately tracking the total number of characters printed to the standard output.


## 📂 Supported Conversions

| Specifier | Description |
| :--- | :--- |
| **%c** | Prints a single character. |
| **%s** | Prints a string. |
| **%p** | Prints a void * pointer in hexadecimal format. |
| **%d / %i** | Prints a decimal (base 10) number. |
| **%u** | Prints an unsigned decimal (base 10) number. |
| **%x / %X** | Prints a number in hexadecimal (base 16) lowercase/uppercase. |
| **%%** | Prints a percent sign. |


## 🛠️ Usage & Compilation

### 1. Compilation
generate statice library: libftprintf.a
```bash
make
```
### 2. Linking the Library to Test Code
```bash
# -L.  tells the compiler to look for the library in the current directory (.)
# -lftprintf  links the libftprintf.a library (note: prefixes 'lib' and extensions '.a' are omitted)
cc main.c -L. -lftprintf -o test_printf
```
## 3. Run
```bash
./test_printf
```
