
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
- Example
	- ![[method-being-called-from-other-file.png]]



### running
