# Static vs dynamic typed languages

- Difference is in the way that they handle variable types and type checking

:: Dynamically Typed Languages ::

:: Statically Typed Languages ::

# Compile-Time vs Run-time

:: Compile-time ::

- When the source code is converted into machine code by the compiler
- Compiler checks the syntax and structure of the code
- If there are any syntax error or type-related issues, the compiler raises compilation errors and prevents the program from being executed

:: Run-time ::

- When the compiled code is executed by the computero r the virtual machine
- At runtime, the program interacts with the OS and hardware, reads input, processes data, and produces output
- At this point, the program can encounter runtime errors, also known as expections (i.e. division by 0, array index out of bounds)
- When the error occurs, the program may terminate abruptly or raise an exceptions

# Stack vs Heap

:: Stack ::

- Region of memory used for storing function/method call frames and local variables
- LIFO (last-in-first-out) manner
- Manages the execution flow of the programs, keeping track of function calls, and storing local variables
- When a function is called, a new frame is added to the stack with space for its local variables and return address
- When the function exits, its frame is removed from the stack, and control returns to the previous function

:: Heap ::

- Region of memory for dynamic memory allocation
- Used to store objects and data structures whose size cannot be determined at compile time
- Objects in the heap have a longer lifetime than local variables on the stack.
- In languages like C and C++, the heap is managed by the programmer

# Primitive vs Reference Types

:: Primitive Types ::

- All data is stored on the stack
- Basic data types built into the programming language
- They represent simple values and correspond to a fixed amount of memory
- Java Examples: byte, short, int, long, float, double, char, boolean
- Assigning a primitive value to another primitive variable copies the actual value
  --> int x = 5
  --> int y = x
  --> y now contains a copy of the value of x

:: Reference Types ::

- All data is stored on the heap
- Refer to objects (instances of classes) in memory rather than holding the actual value
- Typically store memory addresses, which point to the location in memory where the object is stored

# Multivariable Assignment and Object Destructuring

:: Multivariable Assignment ::

- Example: x, y, z = 1,2,3
- A syntactic sugar which makes it easy to assign different variables values

:: Object Destructuring ::

- Specifically deals with objects
- Let's you unpack values from objects into variables based on the property names
- Example:
  const person = {name: "Alice", age: 30};
  const {name, age} = person;
- Another example:
  const [x,y,z] = [1,2,3]
