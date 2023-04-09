# Unit 1 - Programming 

## 3.1. Variables

- Variables represent storage locations.
- Every variable has a type that determines what values can be stored in the variable.
- C# is a type-safe language, and the C# compiler guarantees that values stored in variables are always of the appropriate type.
- The value of a variable can be changed through ***assignment*** or through ***use of the ++ and -- operators***.
- A variable shall be definitely assigned before its value can be obtained.
- Syntax:

```csharp
class Demo {
	static void Main(string[] args) {
		// Declaration
		type identifier;

		// Initialization
		identifier = value;

		// Declaration and initialization
		type identifier = value;

	}
}
```
- Read more about variables at [Variables - C# language specification | Microsoft Learn](https://learn.microsoft.com/en-us/dotnet/csharp/language-reference/language-specification/variables)

![C# Variables in Action (VS Code)](00_Src/csharp_vars_ex.png "C# Variables in Action (VS Code)")

- In the above example
	1. <b style="color: green;">&#x2713;</b> Declaration of variable `num1`
	2. <b style="color: green;">&#x2713;</b> Initializing `num1` to value `20`
	3. <b style="color: green;">&#x2713;</b> Declaring `num2` and initializing it to value `10`
	4. <b style="color: red;">&#x2715;</b> Trying to read the value from `sum` which has not been initialized

## 3.2. Constants

- Constants are immutable values which are known at compile time and do not change for the life of the program.
- Constants are declared with the const modifier.
- Only the C# built-in types (excluding System.Object) may be declared as const.
- User-defined types, including classes, structs, and arrays, cannot be const.

![C# Constants in Action (VS Code)](00_Src/csharp_const_ex.png "C# Constants in Action (VS Code)")

- In the above example
	1. Gravitational constant $G$ is defined with its value in ***class-level***
	2. Mathematical constant $\Pi$ is defined with its value computed in ***class-level***
	3. Speed of light $C$ is defined with its value computed in in ***method-level***
	4. Reading a constant

## 3.3 Types System

![C# Types System Hierarchy](00_Src/csharp_types_system.png "C# Types System Hierarchy")

## 3.4 Identifiers

***
[Home](README.md) | [Prev](01_Intro.md) | [Next](03_ConstVar.md)