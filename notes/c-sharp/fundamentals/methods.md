
### Properties
- code block.
- receives parameters and(optionally) returns value.
- readable code and code reuse.
- declared using class and struct.

### Syntax
```c#
<access_modifier> <return_type> Method_Name (Parameters) 
{
	// method statements
	// return 
}
```
	access_modifier and return are optional.
- If a method is returning a value then, value must be returned for all possible execution paths.
```c#
public int AddTwoNumbers(int a, int b)
{
	if(a > b) {
		return 1;
	}
			
	/* 
		nothing to return, if execution reches here -> therefore results in 
		compile time error
	*/
}
```
	here compile time error will be thrown. 



### Calling a method present in some other file
- that method needed to be **public**.
- calling method
	- <class_name>.<method_name>
- use of **using**
	- namespace image is required, where the class resides in.
- Example ^f97a0d
	- ![[method-being-called-from-other-file.png]]
	- Although the name of application is **console-app-1**, but the name of namespace is **console_app_1** why?



### Optional Parameters and Expression-bodied Members
- **Optional Parameters** are needed to be defined at end of parameter list, they can't be mixed with non-optional ones.
	- However, while invoking it, if named arguments is used, then order of invoking doesn't matter.
- **User expression-bodied syntax**
	- used to make short methods even more shorter.
	- fat arrow operator is used here. [=>]
- Example
```c#
// definition
	public static int sum(int a, int b) => a + b;
	public static int sum(int a, int b, int c) => a + b + c;
	
	public static int Advanced_Sum(int a, int b, int c = 0) => a + b + c;	
// call
	Console.WriteLine(sum(1, 2));
	Console.WriteLine(sum(1, 2, 3));
	
	Console.WriteLine(Advanced_Sum(1, 2));
	Console.WriteLine(Advanced_Sum(1, 2, 3));
```
	- Observe, by using optional parameter, we can have only single function to do work for both sum(), however, it was possible because the sole purpose of both the methods were same.
	- using => has reduced the redundant code.
- 
### Named arguments
- **Named Arguments**: not required to follow order of parameters, one or more parameters can have name defined when provoking the method.
```c#
	public static int product(int a, int b, int c = 1) => a * b * c;
	Console.WriteLine(Utilities.product(c: 2, b: 5, a:10));
```
	Observe, here that we have called the optional parameter first, i.e. mixed optional and non-optional parameters.
- 
### questions
- what is use of named arguments.
- in which cases fat operator can be used[expression-bodied members]
	- method having multiple lines.
	- method returning void.
- how the name of namespace is determined, example [[#^f97a0d]].
- 
### parsing
- converting string to other datatypes.

| Feature            | `Parse` Method                                                                                                         | `TryParse` Method                                                                                                               |
| ------------------ | ---------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------- |
| Purpose            | Converts a string to a specified type, throwing an exception if the conversion fails.                                  | Attempts to convert a string to a specified type without throwing an exception if the conversion fails.                         |
| Exception Handling | Throws an exception (`FormatException`, `ArgumentNullException`, `OverflowException`) if the input is invalid or null. | Does not throw an exception. Instead, returns `true` or `false` to indicate success or failure.                                 |
| Return Type        | Returns the parsed value directly (e.g., `int`, `double`).                                                             | Returns a `bool` indicating success or failure and outputs the parsed value using an `out` parameter                            |
| Use Case           | Useful when you are sure that the input is valid and expect it to succeed.                                             | Useful when you are uncertain about the input’s validity and want to handle the parsing result without dealing with exceptions. |
| Performance        | Slightly slower if the input is invalid because of exception handling overhead.                                        | More efficient when dealing with invalid inputs, as it avoids exception overhead.                                               |
```c#

Console.WriteLine("Provide integer input: ");
string ip = Console.ReadLine();

try
{
	int a = int.Parse(ip);
	Console.WriteLine($"Correct input: {a}");
}
catch (Exception ex) { 
	Console.WriteLine(ex.Message);
}

int b;
bool isInputValid = int.TryParse(ip,out b);
if (isInputValid) 
	Console.WriteLine($"Correct input: {b}");
else 
	Console.WriteLine("InCorrect input");
	
```


### running
