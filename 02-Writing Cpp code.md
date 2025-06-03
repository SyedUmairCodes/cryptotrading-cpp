# Writing C++ Code

C++ code starts with `#include <iostream>`. This line includes the `iostream` library, which provides input/output functionalities. This is similar to importing modules in JavaScript.

Every single C++ code has a `int main(){}` function in it. This is the entry point of any C++ program. The int indicates that the function will return an integer value and `return 0;` is used to signal that the program has executed successfully.

## Hello world

To print the text "Hello world" in our console we write it using `std::cout` which is the standard output stream object (console output).

```C++
std::cout << "Hello World" << std::endl;
```


The `<<` is the stream insertion operator, used to "feed" data to the output stream. "Hello World" is the string literal to be printed. `std::endl` represents the "end of line" character, which moves the cursor to the next line on the console. Using `std::endl` ensures cross-platform compatibility for line endings.

## Compiling and Running the Code:

We will use the g++ command (GNU C++ compiler) in the terminal to compile the code. g++ main.cpp compiles the main.cpp file and creates an executable file named a.out (by default on Unix-like systems). Running `./a.out` executes the compiled program.

**The Compilation Process:**

- The first step is preprocessing, this handles directives like `#include`, which inserts the content of the included files into the source code.

- The C++ code is then translated into assembly, and then to object code. Object code is machine-level code but not fully linked yet.

- The object code is linked with other object files and libraries to create the final executable. Linking resolves external references and combines all the necessary code into a single executable file. 

The unlinked code wouldn't know how to handle the std::cout call. The g++ main.cpp command implicitly performs linking as the final step.

> [!NOTE]
> Compiling C++ code is a multi-stage process. Each stage converts the code to a lower level representation, getting closer to the machine's instructions. Linking is crucial for combining different parts of the code and libraries.

