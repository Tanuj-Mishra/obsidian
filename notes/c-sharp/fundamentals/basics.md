#string

- Code refactoring: reorganizing existing code, without changing the functionality.

- if
```c#
if(a = 100) 
	Console.WriteLine("inside if");
```
	will throw compile time error.

### switch
-![[switch-statement.png]]
- works with most of datatype except float and double.
- case labels use a pattern: constant or relational.
- default will be executed at last ,whereas it can be placed anywhere.
___
## strings
- these are collection of char objects.
- are of type string.
- they behave differently as compared to normal c# variables.



## string interpolation
```c#
int a = 2;
int b = 3;
Console.WriteLine($"Sum: {a+b}");
```
