# C Programming Basics

## 1. Data Types

| Data Type | Description                                                                            |
| --------- | -------------------------------------------------------------------------------------- |
| `int`     | Used to store whole numbers, including positive and negative integers.                 |
| `float`   | Used to store decimal numbers with single precision.                                   |
| `double`  | Used to store decimal numbers with double precision and greater accuracy than `float`. |
| `char`    | Used to store a single character.                                                      |
| `bool`    | Used to store a Boolean value, either true or false.                                   |
| `void`    | Represents the absence of a value or data type.                                        |

## 2. Format Specifiers

| Format Specifier | Description                                                               |
| ---------------- | ------------------------------------------------------------------------- |
| `%d`             | Used to display a signed integer.                                         |
| `%u`             | Used to display an unsigned integer.                                      |
| `%o`             | Used to display an integer in octal format.                               |
| `%x`             | Used to display an integer in hexadecimal format using lowercase letters. |
| `%X`             | Used to display an integer in hexadecimal format using uppercase letters. |
| `%f`             | Used to display a floating-point value.                                   |
| `%e`             | Used to display a floating-point value in scientific notation.            |
| `%c`             | Used to display a single character.                                       |
| `%s`             | Used to display a string.                                                 |
| `%ld`            | Used to display a long integer.                                           |

## 3. Input/Output Functions

### scanf()

`scanf()` is used to read formatted input from the user.

Example:

```c
scanf("%d", &age);
```

### printf()

`printf()` is used to display formatted output on the screen.

Example:

```c
printf("Age = %d", age);
```

### getchar()

`getchar()` reads a single character from the keyboard.

Example:

```c
char ch;
ch = getchar();
```

### putchar()

`putchar()` displays a single character on the screen.

Example:

```c
putchar(ch);
```

### fgets()

`fgets()` is used to read a line of text, including spaces.

Example:

```c
fgets(name, sizeof(name), stdin);
```

### puts()

`puts()` displays a string followed by a new line.

Example:

```c
puts(name);
```

## 4. Escape Sequences

Escape sequences are special characters used inside strings and character constants.

| Escape Sequence | Meaning               | Example                   |
| --------------- | --------------------- | ------------------------- |
| `\n`            | New line              | `printf("Hello\nWorld");` |
| `\t`            | Horizontal tab        | `printf("Hello\tWorld");` |
| `\\`            | Backslash             | `printf("C:\\Program");`  |
| `\"`            | Double quotation mark | `printf("\"Hello\"");`    |
| `\'`            | Single quotation mark | `printf("\'A\'");`        |

## 5. Precision

Precision specifies the number of digits displayed after the decimal point for floating-point output.

It is specified using a dot followed by the number of decimal places between `%` and `f`.

For example:

```c
printf("%.2f", value);
```

This displays the floating-point value with **2 digits after the decimal point**.

Another example:

```c
printf("%.4f", value);
```

This displays the value with **4 digits after the decimal point**.
