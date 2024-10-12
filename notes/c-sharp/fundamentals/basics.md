#string #verbatim-string #escape-sequence


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


## Escape characters
- `\n, \t`
#### How to escape escape characters
1. Use ```\``` before ```\```.
2. Verbatim string: use of ```@``` before string.
```c#
string escaped_escapedString1 = "C:\\Program Files\\Notepad";
string escaped_escapedString2 = @"C:\Program Files\Notepad";
```


## Include " inside a string
- Use backslash, ```\```.
- Note: problem arises when we try to include **"**, incase of **'** there is no such problem.
```c#
string escaped_quotes1 = "this isn't my cup of tea";
string escaped_quotes2 = "this isn\"t my cup of tea";
```