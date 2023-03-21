<h1 align="center">
	:books: LIBFT
</h1>

<p align="center">
<b><i>Implementation of some of the Standard C Library functions</i></b><br>
</p>

<p align="center">
	<img alt="GitHub code size in bytes" src="https://img.shields.io/github/languages/code-size/Bettercallous/libft?color=red" />
	<img alt="Code language count" src="https://img.shields.io/github/languages/count/Bettercallous/libft?color=yellow" />
	<img alt="GitHub top language" src="https://img.shields.io/github/languages/top/Bettercallous/libft?color=blue" />
	<img alt="GitHub last commit" src="https://img.shields.io/github/last-commit/Bettercallous/libft?color=green" />
</p>

---

## 💡 About the project :

Libft is the first project in the 42 curriculum. It requires us to re-create some standard C library functions including some additional ones that can be used in the future projects.
At 42 we're not allowed to use some standard libraries on our projects, therefore we have to keep growing this library with our own functions as we go farther in the curriculum.

**:heavy_exclamation_mark: NOTE** <br />
Because of 42 School norm requirements: <br />
* All variables are declared and aligned at the top of each function <br />
* Each function can't have more then 25 lines of code <br />
* C++ style code commenting is forbidden <br />
* Project should be created just with allowed functions otherwise it's cheating. <br />

### The project consists of 3 main logical parts:
* Standart Libc functions
* Additional functions
* Bonus part functions

### 🛠️ How to compile library:

Using Makefile you can create library file libft.a<br/>
Makefile has 4 main options:<br/>
* **make** - to compile C files - create object files and library libft.a<br/>
* **make clean** - to remove object files<br/>
* **make fclean** - remove libft.a file<br/>
* **make re** - recompile the library<br/>

### Short description of each function:

#### Main part

| Function      | Description                                                                           |
| ------------- | --------------------------------------------------------------------------------------| 
| memset | fill a byte string with a byte value |
| bzero | write zeroes to a byte string |
| memcpy | copy memory area |
| memmove | copy byte string |
| memchr | locate byte in byte string |
| memcmp | compare byte string |
| strlen | get length of string |
| strdup | save a copy of a string |
| strcpy | copy strings |
| strncpy | copy strings size of n |
| strcat | concatenate strings |
| strncat | concatenate n symbols of one string to another |
| strlcat | size-bounded string copying and concatenation |
| strchr | locate character in string |
| strrchr | locate character in string |
| strstr | locate a substring in a string |
| strnstr | locate a substring in a string |
| strncmp | compare strings |
| atoi | convert ASCII string to integer |
| isalpha | alphabetic character test |
| isdigit | decimal-digit character test |
| isalnum | alphanumeric character test |
| isascii | test for ASCII character |
| isprint | printing character test (space character inclusive) |
| toupper | lower case to upper case letter conversion |
| tolower | upper case to lower case letter conversion |

#### Additional functions

| Function      | Description                                                                           |
| ------------- | --------------------------------------------------------------------------------------| 
| ft_striteri   | Applies the function f to each character of the string passed as argument, and passing its index as first argument. Each character is passed by address to f to be modified if necessary |
| ft_strmapi    | Applies the function f to each character of the string passed as argument by giving its index as first argument to create a “fresh” new string (with malloc(3)) resulting from the successive applications of f |
| ft_substr     | Allocates (with malloc(3)) and returns a new substring from the string given as argument. The substring begins at indexstart and is of size len. If start and len aren’t refering to a valid substring, the behavior is undefined. If the allocation fails, the function returns NULL |
| ft_strjoin    | Allocates (with malloc(3)) and returns a new string ending with ’\0’, result of the concatenation of s1 and s2. If the allocation fails the function returns NULL |
| ft_strtrim    | Allocates (with malloc(3)) and returns a copy of the string given as argument without whitespaces at the beginning or at the end of the string. Will be considered as whitespaces the following characters ’ ’, ’\n’ and ’\t’. If s has no whitespaces at the beginning or at the end, the function returns a copy of s. If the allocation fails the function returns NULL |
| ft_split      | Allocates (with malloc(3)) and returns an array of “fresh” strings (all ending with ’\0’, including the array itself) obtained by spliting s using the character c as a delimiter. If the allocation fails the function returns NULL. Example: ft_strsplit(" hello fellow    students ", ’ ’) returns the array ["hello", "fellow", "students"] |
| ft_itoa       | Allocate (with malloc(3)) and returns a new string ending with ’\0’ representing the integer n given as argument. Negative numbers must be supported. If the allocation fails, the function returns NULL |
| ft_putchar    | Outputs the character c to the standard output |
| ft_putstr     | Outputs the string s to the standard output |
| ft_putendl    | Outputs the string s to the standard output followed by a ’\n’ |
| ft_putnbr     | Outputs the integer n to the standard output |
| ft_putchar_fd | Outputs the char c to the file descriptor fd |
| ft_putstr_fd  | Outputs the string s to the file descriptor fd |
| ft_putendl_fd | Outputs the string s to the file descriptor fd followed by a ’\n’ |
| ft_putnbr_fd  | Outputs the integer n to the file descriptor fd |

#### Bonus part

| Function        | Description                                                                           |
| --------------- | --------------------------------------------------------------------------------------| 
| ft_lstnew       | Allocates (with malloc(3)) and returns a “fresh” link. The variables content and content_size of the new link are initialized by copy of the parameters of the function. If the parameter content is nul, the variable content is initialized to NULL and the variable content_size is initialized to 0 even if the parameter content_size isn’t. The variable next is initialized to NULL. If the allocation fails, the function returns NULL |
| ft_lstdelone    | Takes as a parameter a link’s pointer address and frees the memory of the link’s content using the function del given as a parameter, then frees the link’s memory using free(3). The memory of next must not be freed under any circumstance. Finally, the pointer to the link that was just freed must be set to NULL (quite similar to the function ft_memdel in the mandatory part) |
| ft_lstadd_front | Adds the element new at the beginning of the list |
| ft_lstiter      | Iterates the list lst and applies the function f to each link |
| ft_lstmap       | Iterates a list lst and applies the function f to each link to create a “fresh” list (using malloc(3)) resulting from the successive applications of f. If the allocation fails, the function returns NULL |
| ft_lstsize      | Counts the number of nodes in a list |
| ft_lstlast      | Returns the last node of the list |
| ft_lstadd_back  | Adds the node ’new’ at the end of the list |
| ft_lstclear     | Deletes and frees the given node and every successor of that node, using the function ’del’ and free(3) |
