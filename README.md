# My Own C Standard Library
Libft is a custom implementation of essential C library functions, built entirely from scratch.
Fully implemented & memory-leak checked with Valgrind.

## 🔹 Part 1: Standard C Re-implementations
Rebuilt commonly used libc functions:
- Memory manipulation: memset, memcpy, memmove, calloc, bzero, etc.
- String handling: strlen, strchr, strlcpy, strnstr, strjoin, etc.
- Character checks: isalpha, isdigit, isalnum, toupper, tolower,...

## 🔹 Part 2: Additional Utility Functions
- Convenience helpers that helps dealing with C strings
- String operations: substr, split, trim, itoa
- Function mapping: strmapi, striteri
- Memory-safe helpers: free() for ft_split,...

## 🔹 Part 3: Linked List Library
A small but clean generic linked list implementation:
- lstnew, lstadd_front, lstadd_back
- lstdelone, lstclear, lstiter, lstmap
- Makes you deal with function pointers and memory ownership properly.

## 🔹 Part 4: Ft_dprintf Function
A custom implementation of the C printf-inspired function.
- Supports formatted output with conversions like: %c, %s, %p, %d, %i, %u, %x, %X
- Includes own buffering, numeric base conversions, and pointer formatting, without using the real printf.

## 🔹 Part 5: get_next_line Function
A line-by-line file reading function that returns the next line from a file descriptor at each call.
- Reads from file descriptor
- Handles arbitrarily long lines using dynamic buffers
- Manages internal state between calls
- Implements own buffering logic with read()
Great for learning memory ownership, static buffers, and avoiding leaks.
  
## 🧠 How to Build
```
make        # compile libft.a
make clean  # remove object files
make fclean # remove everything
make re     # rebuild from scratch
```
----
### 📝 Include it in C project
#include "libft.h"

### Link to the library
```
cc code1.c code2.c libft.a
```
