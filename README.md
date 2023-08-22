# printf :fax:

## Description :hourglass_flowing_sand:

------------


The printf function sends formatted output to stdout.
_printf() function format string is a character string

------------


## Resources :wrench:

------------


Secrets of printfby Don colton
https://www.cypress.com/file/54761/download

------------



## Authorized functions and macros

------------


write (man 2 write)

malloc (man 3 malloc)

free (man 3 free)

va_start (man 3 va_start)

va_end (man 3 va_end)

va_copy (man 3 va_copy)

va_arg (man 3 va_arg)

------------

## Compilation

------------



The code must be compiled this way:

```` c
**$ gcc -Wall -Werror -Wextra -pedantic *.c\***

````

As a consequence, be careful not to push any c file containing a `main` function in the root directory of your project (you could have a `test` folder containing all your tests files including `main` functions)

The main files will include your main header file (`main.h`): **#include main.h**

------------

## Use & Examples


------------

**Prototype:** int _printf(const char *format, ...);
**Use - General:** _printf("format string", var1, var2, ...);

**Examples:**
 - Basic String: _printf("%s World", "Hello");`
	 - Output: Hello World

- Print integers: _printf("This is an array element: arr[%d]:%c", 32, arr[32]);`
	- Output: This is an array element arr[32]:A

Many other specifiers and flags were added and by combinig those the _printf() function generate a different ouput. The following list are the specifiers and flags allowed.

------------

## Files contained in this repository


------------

| Name                | Information                        |
|----------------|-------------------------------|
| `_printf.c`	|formatted output conversion and print data.|

| `main.h` | Header file with the data type struct, standard libraries and custom prototypes. |
| `ev_print_func.c`| returns the amount of identifiers.|
| `fill_binary_array.c`| prints decimal in binary|
| `fill_hex_array.c` | writes the character c to stdout | 
| `fill_long_oct_array.c` | calculates a long octal number |
| `fill_oct_array.c` | writes the character c to stdout |
| `fill_short_oct_array.c` | calculates a short octal number |
| `get_print_func.c` | selects the correct function to perform the operation. |
| `handl_buf.c` | concatenates the buffer characters | 
| `print_add.c` | prints the address of an input variable |
| `print_bnr.c` | prints decimal in binary |
| `print_buf.c` | prints buffer | 
| `print_chr.c` | writes the character c to stdout |
| `print_hex.c` | prints a decimal in hexadecimal |
| `print_int.c` | prints an integer |
| `print_long_hex.c` | prints a long decimal in hexadecimal |
| `print_long_int.c` | prints a long integer |
| `print_long_oct.c` | prints long decimal number in octal |
| `print_long_unt.c` | prints a long unsigned integer | 
| `print_long_upx.c` | prints a long decimal in hexadecimal |
| `print_num_hex.c` | print number in hex begining with zero |
| `print_num_oct.c` | print the number in octal begining with zero | 
| `print_num_upx.c` | prints number in uppercase hex |
| `print_oct.c` | prints decimal number in octal |
| `print_prg.c` | writes the character c to stdout |
| `print_rev.c` | writes the str in reverse |
| `print_rot.c` | writes the str in ROT13 |
| `print_short_hex.c` | prints a short decimal in hexadecimal |
| `print_short_int.c` | prints a short integer | 
| `print_short_oct.c` | prints long decimal number in octal |
| `print_short_unt.c` | prints a short unsigned integer |
| `print_short_upx.c` | prints a short decimal in hexadecimal | 
| `print_space_int.c` | prints int begining with space |
| `print_str.c` | writes the string to stdout |
| `print_unt.c` | prints an unsigned int |
| `print_upx.c` | prints a decimal in hexadecimal |
| `print_usr.c` | prints a string and values of |


------------

## Tasks required for this project


------------

## 0.  0. I'm not going anywhere. You can print that wherever you want to. I'm here and I'm a Spur for life.

* Write a function that produces output according to a format.
	- Prototype: `int _printf(const char *format, ...);`
	- Returns: the number of characters printed (excluding the null byte used to end output to strings)
	- write output to stdout, the standard output stream
	- `format` is a character string. The format string is composed of zero or more directives. See `man 3 printf` for more detail. You need to handle the following conversion specifiers:
		* `c`
		* `s`
		* `%`
	- You don’t have to reproduce the buffer handling of the C library `printf` function
	- You don’t have to handle the flag characters
	- You don’t have to handle field width
	- You don’t have to handle precision
	- You don’t have to handle the length modifiers

## 1. Education is when you read the fine print. Experience is what you get if you don't

* Handle the following conversion specifiers:
	- `d`
	- `i`
	- You don’t have to handle the flag characters
	- You don’t have to handle field width
	- You don’t have to handle precision
	- You don’t have to handle the length modifiers

## 2. With a face like mine, I do better in print

* Handle the following custom conversion specifiers:
	- `b`: the unsigned int argument is converted to binary

## 3. What one has not experienced, one will never understand in print

* Handle the following conversion specifiers:
	- `u`
	- `o`
	- `x`
	- `X`
	- You don’t have to handle the flag characters
	- You don’t have to handle field width
	- You don’t have to handle precision
	- You don’t have to handle the length modifiers

## 4. Nothing in fine print is ever good news

* Use a local buffer of 1024 chars in order to call `write` as little as possible.

## 5. My weakness is wearing too much leopard print

* Handle the following custom conversion specifier:
	- `S` : prints the string.
	- Non printable characters (0 < ASCII value < 32 or >= 127) are printed this way: `\x`, followed by the ASCII code value in hexadecimal (upper case - always 2 characters)

## 6. How is the world ruled and led to war? Diplomats lie to journalists and believe these lies when they see them in print

* Handle the following conversion specifier: `p`.
	- You don’t have to handle the flag characters
	- You don’t have to handle field width
	- You don’t have to handle precision
	- You don’t have to handle the length modifiers

## 7. The big print gives and the small print takes away

* Handle the following flag characters for non-custom conversion specifiers:
	- `+`
	- space
	- `#`

## 8. Sarcasm is lost in print

* Handle the following length modifiers for non-custom conversion specifiers:
	- `l`
	- `h`
* Conversion specifiers to handle: `d`, `i`, `u`, `o`, `x`, `X`

## 9. Print some money and give it to us for the rain forests

* Handle the field width for non-custom conversion specifiers.


## 10. The negative is the equivalent of the composer's score, and the print the performance

Handle the precision for non-custom conversion specifiers.

## 11. It's depressing when you're still around and your albums are out of print

Handle the `0` flag character for non-custom conversion specifiers.

## 12. Every time that I wanted to give up, if I saw an interesting textile, print what ever, suddenly I would see a collection

Handle the `-` flag character for non-custom conversion specifiers.

## 13. Print is the sharpest and the strongest weapon of our party

* Handle the following custom conversion specifier:
	- `r` : prints the reversed string

## 14. The flood of print has turned reading into a process of gulping rather than savoring

* Handle the following custom conversion specifier:
	- `R`: prints the rot13'ed string

## 15. *

* All the above options work well together.


## Authors :octocat:

[Abeer Ragab](https://www.linkedin.com/in/abeer-ragab-b25872260/) | [Twitter](https://twitter.com/abeerragab5211) | [Github](https://github.com/Abeer-M-Ali)

[Khaled Ali](https://www.linkedin.com/in/khaled-ali-32a39318a/) | [Twitter](https://twitter.com/khaledali0907) | [Github](https://github.com/KhaledAli0907)
