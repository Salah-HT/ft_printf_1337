    
  <p align="center">
  <img src="https://github.com/user-attachments/assets/c03cfe0a-a360-459c-8896-c1091304140b" alt="ft-printf" />
</p>


This project is a custom implementation of the standard C `printf` function. The goal is to gain a deeper understanding of how variadic functions work in C by recreating the behavior of `printf` from scratch.

## 🧠 Project Objective

Reimplement a simplified version of `printf`:

```c
int ft_printf(const char *format, ...);
```

By completing this project, we aim to:
- Understand variadic functions and how they work internally.
- Handle formatted output with various format specifiers.
- Improve our C programming skills by managing low-level memory operations and string manipulations.

## 🔧 Features

- Supports various format specifiers:
  - `%c` – character  
  - `%s` – string  
  - `%d` / `%i` – signed decimal integer  
  - `%u` – unsigned decimal integer  
  - `%x` / `%X` – hexadecimal  
  - `%p` – pointer  
  - `%%` – print a literal `%` character  
- Handles flags and format parsing  
- Mimics the behavior of the standard `printf`

## 🛠️ Technologies

- Language: C  
- Standard Libraries: `unistd.h`, `stdarg.h`

## 🚀 Getting Started

### Compilation

Use the following command to compile:

```bash
gcc -Wall -Wextra -Werror ft_printf.c -o ft_printf
```

### Usage

```c
#include "ft_printf.h"

int main(void) {
    ft_printf("Hello %s, your score is %d/100\n", "Alice", 95);
    return 0;
}
```

## 📚 Learning Outcome

This project is a great exercise to understand:
- Variadic functions using `va_start`, `va_arg`, and `va_end`
- Low-level output using `write()`
- Manual parsing and formatting of strings and integers

## 👨‍💻 Author

Made with 💻 by [shamsate]

	
	
	———————————————————————————————————————————————————————————————------------------------------                  
    |Variadic functions in C|          :->                                                                 
    ———————————————————————————————————————————————————————————————------------------------------             
    1- Variadic functions are functions that can take a variable number of                       
    arguments. In C programming, a variadic function adds flexibility to the                    
    program. It takes one fixed argument and then any number of arguments can                    
    be passed.                                                                                    
    The variadic function consists of at least one fixed variable and then                       
    an ellipsis(…) as the last parameter. 
    ———————————————————————————————————————————————————————————————------------------------------        
    header file :	#include <stdarg.h>                                                                
    ———————————————————————————————————————————————————————————————------------------------------
    <stdarg.h> includes the following methods:                                                  
    va_start(va_list ap, argN) : va_start(va_list ap, argN)                                      
    va_arg(va_list ap, type) : This one accesses the next variadic function argument.            
    va_end(va_list ap) : This ends the traversal of the variadic function arguments.
    —————————————————————————————————————————————————————————————————————————————----------------  
