- record was introduced in c#9.
## traditional approach
- method are wrapped inside class, which itself was nested in namespace.

## top-level statements
- pre phase of it, traditional approach was used.
- was introduced in c-sharp-10, mapped to .net-6.
- removed the requirement of main method in Program.cs file.
- although in background:
	- **Namespace** , **Program.cs** class, and **Main** method is added in it .
- reason for doing so
	- Top-level statements are specifically designed for the entry point of an application, not for defining reusable classes or methods.
	- Since the other files are meant to contain reusable logic (like your `sum` method), it naturally follows the traditional class-based structure.
	- Conversely, `Program.cs`, which is the entry point, is well-suited for the simpler, top-level approach since it directly interacts with the application's startup logic.
- however, in all other files other then Program.cs, **Traditional Approach** is still used.
- example
	![[method-being-called-from-other-file.png]]	


## other

