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


## questions
1. similarities and differences between [[#^462881]] [s1 and s2]
2. intellisense show, some method marked with star and some normally, why?
3. 