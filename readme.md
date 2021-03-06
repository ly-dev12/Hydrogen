# Hydrogen 

Hydrogen is a programming language designed for the versatility and ease that can offer static data types and a new concept called BLOCKS.

# WARNING: (Building the compiler)

`Interprete not compiled`

---

### Version:
Beta 0.0.1

### Warning:
Hydrogen is still under development, it is just in its early stages, it is almost useless.

`Now available for windows and linux arch amd64`

### How to use:
- Install the executable file
- Create a file with extension `.hg`
- Write code
- Run executable file and type the enxt command:
```
run ${filepath}
Example:
run C:/Users/main.hg
```

## Tutorial
- <h2>Types</h2>
`int`: Example: 234
`bool`: Example: true; false
`string`: example: "sdffsdsfd"
- <h2>Variables</h2>
Variables are declared with the reserved word `dec` followed by the name and then the type of the variable, then the assignment operator` -> `followed by the value of the variable. 
Example:
```
dec number int -> 345;
println(number); 
// OUTPUT: 345
```
- <h2>If</h2>
The if's are the normal ones in every programming language. Example:
```
if(3 < 5){
    return 34
}else{
    return 10
}
```

- <h2>Functions</h2>
The functions in an initial state, they need to mature enough, they are not yet able to check the return type, the syntax of a function is the following:
```
fn callPrint(x int) <- int {
    return x + 23
}

println(callPrint(234));
// OUTPUT: 234
```
As I said, the functions are not yet able to evaluate the return value, you can even insert a string in the parameter, it does not verify the type aprameter either.

- <h2>Aritmetic operators</h2>
```
4 + 2

2 / 2 + 4

8 + 4 + 2
```
---

# New features 1/1/2021 21:54
- <h2>Functions<h2> 
Functions now strongly support return values ​​and parameter types. Example:
```hg
fn Hi(hi string) <- string {
    return hi
}

println(Hi("Hello World"))
// OUTPUT: Hello World
```

- <h2>STOP keyword</h2> Experimental
The stop keyword is used to tell the program not to continue its execution. Example:
```hg
if(3 < 7) {
    STOP; ## comment: Hey stop here, don't run the program or block any more
}
```
The STOP keyword is still in the experimental phase, you have to be careful with this because it is a bad step and unfortunately our program may stop working.

# New features 2/1/2021 12:35
- <h2>Blocks</h2> Experimental
The blocks execute a functionality that is given, the blocks do not take parameters or return values so they are lighter. Example:
```hg
Block printHelloWorld{
    println("Hello World")
}

pritnHelloWorld?
```
A block is called with the `name of the block` and the `?` sign in front with this block call everything in your body is going to run as many times as you call it, but remember it has no return value

- <h2>Macros</h2> Experimental
Macros are used to declare some static and dynamic value, it is declared with the reserved word `def` followed by the `name` and then the `value` that is dynamic the user does not indicate the type that the macro will be. Example:
```hg
def quality 1024
println(quality)
## OUTPUT: 1024
Rules:
def xd 23
def xd 46  ## ERROR: Unable to shade a macros.
dec xd int -> 345 ## ERROR: You cannot declare a variable with the name of a macro
```

The macros in the future will have a complement that will be the macro conditionals. Example:
```
def mod 234
ifdef mod {
    println("mod is defined")
}
```

## New Experimentals
- `imports` import files and functions
- `loops` loops `for` `while`
- `macros complements` a complements for macros (ifdef)

## Experimentals (WORKING)
- `STOP` keyword `Working`
- `Block` Blocks `Working`
- `String` String data Type, `SUCCESS✓`
- `functions` functions return value and parameters type. `SUCCESS✓`
- `macros` a macros implementation `Working`