


## Properties
- Specify size and location[stack or heap] in memory.
- Specify data range.
- Specify supported operations.
___
## Types
- Predefined[built-in] - Primitive and Non-Primitive.  
- User-defined.
	- Primitive:
		- byte, short, int[default].
		- decimal, double[default], float.
		- char
		- bool
	- Non-Primitive
		- object
		- string
- Note: ```bool``` and ```Boolean```, both are present but we are using _bool_ till now.

## Default values
- number, float -> 0.
- char -> null
- boolean -> false.
## Members on primitive types 
fields of int and char.
```c#
int minIntValue = int.MinValue;
int maxIntValue = int.MaxValue;

char c = 'a';
bool isSymbol = char.IsSymbol(c);
bool IsPunctuation = char.IsPunctuation(c);

```

## date and time
- DateTime: to deal with date, time or combination of both.
- TimeSpan: to deal with period of time. 

```c#
DateTime d1 = new DateTime(2024, 10, 15, 15, 25, 45);
DateTime d2 = DateTime.Now;
TimeSpan t1 = new TimeSpan(10, 30, 50);
DateTime d3 = d2.AddHours(10);
DateTime d4 = d2.Add(t1);
```