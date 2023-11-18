# ft_printf - Recreating the printf Function

## Introduction

This project involves creating a custom printf function, named `ft_printf`, that mimics the behavior of the original `printf` function from the C standard library. The goal is to implement a subset of format specifiers and conversions to handle character, string, pointer, decimal, integer, unsigned decimal, and hexadecimal printing.

## Project Files

- **Makefile:** Contains rules for compilation (`all`), cleaning (`clean`), force cleaning (`fclean`), and recompilation (`re`).
  
- **libftprintf.h:** Header file containing function prototypes and necessary declarations.

- **\*.c:** Source files containing the implementation of the `ft_printf` function and related helper functions.

## How to Use

1. Clone the repository:

   ```bash
   git clone https://github.com/your-username/ft_printf.git
   ```

2. Navigate to the project folder:

   ```bash
   cd ft_printf
   ```

3. Compile the library:

   ```bash
   make
   ```

   This will generate the `libftprintf.a` library.

4. Use the library in your C projects:

   - Copy the `libftprintf.a` file to your project folder.
   - Include the `libftprintf.h` header file in your C files.
   - Compile your project with the library:

     ```bash
     gcc -Wall -Wextra -Werror -o your_program your_file.c libftprintf.a
     ```

5. Clean up:

   ```bash
   make clean
   ```

   This removes object files.

6. If you want to remove the library and object files:

   ```bash
   make fclean
   ```

## Functionality

The `ft_printf` function can be used to format and print data to the standard output. It supports the following conversions:

- `%c`: Prints a single character.
- `%s`: Prints a string.
- `%p`: Prints a void pointer in hexadecimal format.
- `%d` / `%i`: Prints a decimal (base 10) number.
- `%u`: Prints an unsigned decimal (base 10) number.
- `%x`: Prints a number in hexadecimal (base 16) lowercase format.
- `%X`: Prints a number in hexadecimal (base 16) uppercase format.
- `%%`: Prints a percent sign.

## Additional Notes

- The `ft_printf` function does not implement the buffer management of the original `printf`.
