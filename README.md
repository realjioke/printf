# Custom `printf` Implementation  

## Overview  
This project is a custom implementation of the standard C **`printf`** function. It mimics the behavior of `printf` by formatting and printing output to the console, supporting various format specifiers such as **`%c` (char), `%s` (string), `%d` (integer), and `%x` (hexadecimal)**.  

## Features  
- **Handles Standard Format Specifiers**:  
  ✅ `%c` - Character  
  ✅ `%s` - String  
  ✅ `%d` / `%i` - Integer  
  ✅ `%x` / `%X` - Hexadecimal  
  ✅ `%o` - Octal  
  ✅ `%u` - Unsigned Integer  
- **Supports Escape Sequences** like `\n` for new lines  
- **Error Handling** for incorrect format specifiers  

## Tech Stack  
- **Language**: C  
- **Standard Libraries**: `<stdarg.h>`, `<unistd.h>`  

## Installation  
### Prerequisites  
Ensure you have **GCC (GNU Compiler Collection)** installed.  

### Steps  
1. Clone the repository:  
   ```bash
   git clone https://github.com/realjioke/printf.git
   ```
2. Navigate into the project folder:  
   ```bash
   cd printf
   ```
3. Compile the project:  
   ```bash
   gcc -Wall -Wextra -Werror -pedantic *.c -o printf
   ```

## Usage  
You can use the custom `_printf` function in your C programs as follows:  

```c
#include "main.h"

int main(void)
{
    _printf("Character: %c\n", 'A');
    _printf("String: %s\n", "Hello, World!");
    _printf("Integer: %d\n", 42);
    _printf("Hexadecimal: %x\n", 255);
    return (0);
}
```

## Contributing  
Contributions are welcome! If you find a bug or want to add support for more specifiers, fork the repository and submit a pull request.  

## License  
This project is licensed under the **MIT License** – see the [LICENSE](LICENSE) file for details.  


