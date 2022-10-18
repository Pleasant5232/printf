# Printf

---

## Summary

## This is a simple implementation of printf function that formats and prints data

## Representation

The \_printf() function produces output according to a format which is described below. This function write its output to the the standard output stream, stdout. It returns the count of printed characters when the function is successful and 1 when the function fails.

## The available conversion specifiers are:

- %c: Prints a single character.

- %d: Prints integers.

- %b: Prints the binary representation of an unsigned decimal.

- %x: Prints the hexadecial representation of an unsigned decimal in lowercase letters

- %X:Prints the hexadecial representation of an unsigned decimal in uppercase letters

- %R: Prints the Rot13 interpretation of a string

- %s: Prints a string of characters.

## Usage

---

- All the files are to be compiled on Ubuntu 14.04 LTS

- Include the "main.h" header file on the functions using the \_printf()

- Compile your code with $ gcc -Wall -Werror -Wextra -pedantic -std=gnu89 \*.c

---

## Example

---

```
#include "main.h"
#include <stdio.h>
/**
* main - Entry point
*
* Return: Always 0
*/
int main(void)
{
  int a;
  int b;
  char *str;
  str = "school";
  a = _printf("%r\n", "Alx"); /*expected: xlA*/
  printf("--->%d\n", a); /*expected: 10*/
  b = _printf("%r\n", str); /*expected: loohcs*/
  printf("%d\n", b); /*expected: 7*/
  b = _printf("%r\n", str); /*expected: loohcs*/
  printf("%d\n", b); /*expected: 7*/
  return (0);
}
```

---

## File Functions

---

### \_printf.c

Custom Printf Function That Performs Formatted Output Conversion And Print Data.

#### main.h

Header File Were All Prototypes Are Saved.

#### get_print_func.c

Pointer To A Function That Selects The Correct Function To Perform The Operation.

#### print_buf.c

Function That Prints The Buffer.

#### handl_buf.c

Function That Concatenates The Buffer Characters.

#### print_chr.c

Function That Writes The Character C To Stdout.

/_ Identifier : %c _/

#### print_str.c

Function That Writes The String To Stdout.

/_ Identifier : %s _/

#### print_int.c

Function That Prints An Integer.

/_ Identifier : %i or %d _/

#### print_bnr.c

Function That Prints Decimal In Binary.

/_ Identifier : %b _/

#### print_oct.c

Function That Prints Decimal In Octal.

/_ Identifier : %o _/

#### print_hex.c

Function That Prints Decimal In Hexadecimal.

/_ Identifier : %x _/

#### print_upx.c

Function That Prints Decimal In Uppercase Hexadecimal.

/_ Identifier : %X _/

#### print_usr.c

Function That Prints A String And Values Of Non-Printed Chars.

/_ Identifier : %S _/

#### print_unt.c

Function That Prints An Unsigned Integer.

/_ Identifier : %u _/

#### print_rev.c

Function That Writes The String To Stdout In Reverse.

/_ Identifier : %r _/

#### print_rot.c

Function That Writes The String To Stdout In Rot13.

/_ Identifier : %R _/

#### print_add.c

Function That Prints The Address Of An Input Variable.

/_ Identifier : %p _/

#### print_long_oct.c

Function That Prints Long Decimal Number In Octal.

/_ Identifier : %lo _/

#### print_long_hex.c

Function That Prints Long Decimal Number In Hexadecimal.

/_ Identifier : %lx _/

#### print_long_int.c

Function That Prints A Long Integer.

/_ Identifier : %li _/

#### print_long_upx.c

Function That Prints A Long Decimal In Uppercase Hexadecimal.

/_ Identifier : %lX _/

#### print_long_unt.c

Function That Prints A Long Unsigned Integer.

/_ Identifier : %lu _/

#### print_short_oct.c

Function That Prints Short Decimal Number In Octal.

/_ Identifier : %ho _/

#### print_short_hex.c

Function That Prints Short Decimal Number In Hexadecimal.

/_ Identifier : %hx _/

#### print_short_int.c

Function That Prints A Short Integer.

#### print_short_upx.c

Function That Prints A Short Decimal In Uppercase Hexadecimal.

/_ Identifier : %hX _/

#### print_short_unt.c

Function That Prints A Short Unsigned Integer.

/_ Identifier : %hu _/

#### print_num_hex.c

Function That Print A Number In Hexadecimal Begining With 0 And x.

/_ Identifier : %#x _/

#### print_num_oct.c

Function That Prints A Number In Octal Begining With 0 And o.

/_ Identifier : %#o _/

#### print_num_upx.c

Function That Prints A Number In Uppercase Hexadecimal.

/_ Identifier : %#X _/

#### print_plus_int.c

Function That Prints An Integer With Plus Symbol.

/_ Identifier : %+i _/

#### print_space_int.c

Function That Prints An Integer Begining With 0 And u.

/_ Identifier : % i _/

#### ev_print_func.c

Function That Returns The Amount Of Identifiers.

# Authors

<a href="https://github.com/Mykell404/printf">Mileba Micheal</a>
<br/>
<a href="https://github.com/Pleasant5232/printf">Sobukola Oladayo</a>

# End
