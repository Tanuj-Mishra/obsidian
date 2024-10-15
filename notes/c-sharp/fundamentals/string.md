- strings behave like array.
- They have tons of build-in methods and properties, which provide functionality and behavior. 
	- **Methods** provide _functionality_ by allowing you to do something with an object (like changing the case of a string, finding a substring, or splitting it).
	- **Properties** expose the state of an object and affect how it behaves or is used in certain methods[i.e. behavior of it].
- 

## Useful methods and properties
### Empty
```c#
string s1 = "";
string s2 = string.Empty;
```

^462881

	both s1 and s2 are identical.
### other
- first classification - most used.
- second classification - different type of input output etc.
- Properties
	- Length
- Methods
	- Trim(), ToUpper(), ToLower(), Replace(), Substring() -> string as output
	- Contains() -> bool as output.
- Different ways to add two string, most preferred is string interpolation.
	- using + operator.
	- using Concat()
	- using Format()
	- using string interpolation.
```c#
string firstName = "Tanuj";
string lastName = "Mishra";

var a = "hello";            // implicit typing also works here
string l = firstName.ToLower();
string u = firstName.ToUpper();
string r = firstName.Replace('j', 'n');
string s = firstName.Substring(1);
string t = firstName.Trim();
bool c = firstName.Contains("an");
int len = firstName.Length;

// adding two strings

// using + operator
string add1 = firstName + " " + lastName;       

// using Concat()
string add2 = String.Concat(firstName, " ", lastName);                                      
// using format()
string add3 = String.Format("Hello {0} {1}, how are you doing.", firstName, lastName);

// String interpolation [Most preffered]
string add4 = $"Hello {firstName} {lastName}, how are you doing.";
```

## other

## comparing strings

#pending


| **Feature**               | **== Operator**                                                                                                                                              | **Equals Method**                                                                                                         |
|---------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------|
| **Definition**            | A binary operator that checks for value equality or reference equality, depending on how it's overridden.                                                      | A method that checks for value equality, can be overridden in custom types for specific equality checks.                   |
| **Default Behavior**      | For reference types, `==` checks for reference equality (whether two references point to the same object in memory). For value types, it checks if values are the same. | For reference types, `Equals` also checks for reference equality unless overridden. For value types, it checks if values are the same. |
| **Overridable**           | Can be overloaded in custom types to redefine what equality means for `==`.                                                                                     | Can be overridden in custom types to define specific equality logic.                                                       |
| **Null Handling**         | Can throw a `NullReferenceException` if the left operand is `null` in a custom `==` implementation.                                                              | Typically handles `null` safely unless overridden with custom logic that doesn't account for `null`.                       |
| **Comparison Type**       | Often used for simple comparisons, like numbers or strings, or to check if two references are the same.                                                          | Can be used for more complex equality checks where the internal state of objects is compared.                              |
| **Usage in Strings**      | For strings, `==` checks for value equality (checks if two strings have the same content).                                                                       | `Equals` also checks for value equality with strings and can be more explicit when comparing object types.                 |
| **Static vs. Instance**   | It’s a static operator, used like `a == b`.                                                                                                                     | It’s an instance method, called like `a.Equals(b)`.                                                                        |
| **Performance**           | May be faster for simple comparisons (e.g., primitive types) but depends on the implementation if overloaded.                                                    | Slightly slower as it is a method call but more flexible for complex comparisons when overridden.                          |
| **Example for Reference Types** | `object a = "Hello"; object b = "Hello"; Console.WriteLine(a == b); // False` (default reference check)                                                      | `object a = "Hello"; object b = "Hello"; Console.WriteLine(a.Equals(b)); // True` (value comparison)                       |

```c#
if ("ab" == "Ab")
	Console.WriteLine("equal-1");
else
	Console.WriteLine("different-1");

if ("Ab" == "Ab")
	Console.WriteLine("equal-2");
else
	Console.WriteLine("different-2");


if (String.Equals("ab", "Ab"))
	Console.WriteLine("equal-3");
else
	Console.WriteLine("different-3");

if (String.Equals("Ab", "Ab"))
	Console.WriteLine("equal-4");
else
	Console.WriteLine("different-4");
```
	different-1
	equal-2
	different-3
	equal-4

- Note: Best way to actually compare two strings is to compare them after applying either of ```toLower()``` or ```toUpper()```on them.

## questions
1. similarities and differences between [[#^462881]] [s1 and s2]
2. intellisense show, some method marked with star and some normally, why?
3. comparing string -> table is not that much clear.
