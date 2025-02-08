# Uninitialized Property Access in C#

This repository demonstrates a common but subtle error in C#: accessing a class property before it has been assigned a value.  Uninitialized property access can lead to unexpected behavior, making debugging difficult.

The `bug.cs` file contains the problematic code.  `bugSolution.cs` shows how to correctly initialize the property to avoid this issue.

## How to Reproduce
1. Clone this repository.
2. Open `bug.cs` in a C# IDE.
3. Run the `MyMethod` function.
4. Observe the default value returned for MyProperty (0 for int).

## Solution
Always initialize properties either in the constructor or before accessing them within a method to ensure predictable behavior. The correct code is shown in `bugSolution.cs`.