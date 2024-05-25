# Libft
_Libft_ is the first training project that was implemented at _42_ (Moscow campus).
The purpose of this project was to code very first own _**C**_ library.

### Studied concepts:
_Makefile, leaks, file descriptor, linked list_
## Detailed description of the project
All functions’ names must be prefixed by “ft_”.<br />
### Allowed external functions:
malloc, free, write
### The library consists of:
1. A set of the re-coded _libc_ functions, as defined in their ``man``. These functions have the same prototype and behaviors as the original. <br />

| memset | bzero | memcpy | 
| :---: |:---:|:---:|
| **memccpy** | **memmove** | **memchr** |
| **memcmp**| **strlen** |**strlcpy** | 
| **strlcat**| **strchr** |**strrchr** |
| **strnstr** | **strncmp** | **atoi** |
| **isalpha** | **isdigit** |**isalnum** |
| **isascii**| **isprint**| **toupper** |
| **tolower** | **calloc**| **strdup** |

2. Additional functions for writing, working with strings and numbers.

| Function's name | Description|
|:---:| ---|
| substr | Returns the substring from the string using a specified start index and  length. NULL if the allocation fails. |
| strjoin | Returns a new string that is the concatenation of prefix and suffix string. NULL if the allocation fails. |
| strtrim | Returns a copy of the string with the characters specified in the second string ‘set’ removed from the beginning and the end of the string. NULL if the allocation fails. |
| split | Returns an array of strings obtained by splitting string using the character ‘c’ as a delimiter. The array is ended by NULL pointer. NULL if the allocation fails. |
| itoa | Return a string representing the integer received as an argument. NULL if the allocation fails. |
| strmapi | Applies the functions ’f’ to each character of the string. Returns a new string with successful applications of ’f’. NULL if the allocation fails. |
| putchar_fd | Outputs the character to the given file descriptor. |
| putstr_fd | Outputs the string to the given file descriptor  |
| putendl_fd | Outputs the string to the given file descriptor, followed by a new line. |
| putnbr_fd | Outputs the integer to the given file descriptor. |
3. Additional function for working with lists.

| Function's name | Description|
|:---:|---|
| lstnew | Returns a new element.
| lsdadd_front | Adds the element at the beginning of the list.
| lstadd_back | Adds the element at the end of the list.
| lstsize | Count the number of elements in a list.
| lstlast | Returns the last element of the list.
| lstdelone |  Takes as parameter an element and frees the memory of the element’s content using the function ‘del’ given as a parameter and free the element. The memory of ‘next’ must not be freed.
| lstclear | Deletes and frees the given element and every successor of that element, using the function ‘del’ and free(3).
| lstiter | Iterates the list and applies the function ’f’ to the content of each element.
| lstmap | Iterates the list and applies the functions ‘f’ to the content of each element. Creates a new list resulting. The ‘del’ function is delete the content of an element if needed. Returns the new list. NULL if the allocation fails.

## Usage
Create library: ``make bonus``<br />
Remove \*.o files: ``make clean``<br />
Remove \*.o and \*.a files: ``make fclean``

### Compilation
Create ``main.c`` file and compile:
```bash
gcc main.c libft.a
```
### Execution
```bash
./a.out
```
### Main tamplate:
```c
#include "ft_libft.h"

int main()
{
      return (0);
}
```

## Additional information
**_42_** is a computer programming school that is entirely free and available to students who are 18-years or older. Its teaching methods are based on peer learning: no teachers, no lectures, fully hands on. The education model focuses on project-based learning and teamwork, rather than theoretical education. There are a lot of campuses all over the world in the **_42 NETWORK_**.
