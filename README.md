# C-Sharp

## Data Types
|Data Type|Size|
|---------|----|
|int|4 bytes|
|long|8 bytes|
|float|	4 bytes|
|double|	8 bytes|
|bool|	1 bit|
|char|	2 bytes|
|string|	2 bytes per character|

## Input and Output
### Output
```cs
Console.WriteLine("Hello World!");
```
### Input
```cs
string userInput = Console.ReadLine();
```

## Conditionals and loop statements
### If statement
```cs
if (condition1)
{
  // block of code to be executed if condition1 is True
} 
else if (condition2) 
{
  // block of code to be executed if the condition1 is false and condition2 is True
} 
else
{
  // block of code to be executed if the condition1 is false and condition2 is False
}
```
#### Shortened
```cs
variable = (condition) ? expressionTrue :  expressionFalse;
```
##### Example
```cs
int time = 20;
if (time < 18) 
{
  Console.WriteLine("Good day.");
} 
else 
{
  Console.WriteLine("Good evening.");
}
```
Instead of writing this we can shortened it to:
```cs
int time = 20;
string result = (time < 18) ? "Good day." : "Good evening.";
Console.WriteLine(result);
```

### Switch
```cs
switch(expression) 
{
  case x:
    // code block
    break;
  case y:
    // code block
    break;
  default:
    // code block
    break;
}
```
### While
```cs
while (condition) 
{
  // code block to be executed
}
```
### For
```cs
for (statement 1; statement 2; statement 3) 
{
  // code block to be executed
}
```
#### Example
```cs
for (int i = 0; i < 5; i++) 
{
  Console.WriteLine(i);
}
```
### Foreach
```cs
foreach (type variableName in arrayName) 
{
  // code block to be executed
}
```
#### Example
```cs
string[] cars = {"Volvo", "BMW", "Ford", "Mazda"};
foreach (string car in cars) 
{
  Console.WriteLine(i);
}
```

## Arrays
```cs
string[] cars = {"Volvo", "BMW", "Ford", "Mazda"};
int[] myNum = {10, 20, 30, 40};
```
Array length:
```cs
string[] cars = {"Volvo", "BMW", "Ford", "Mazda"};
Console.WriteLine(cars.Length);
```
### Loop through array
```cs
string[] cars = {"Volvo", "BMW", "Ford", "Mazda"};
for (int i = 0; i < cars.Length; i++) 
{
  Console.WriteLine(cars[i]);
}
```
Or we can also do this using foreach loop explained above.

### Sort Array
String array
```cs
// Sort a string
string[] cars = {"Volvo", "BMW", "Ford", "Mazda"};
Array.Sort(cars);
foreach (string i in cars)
{
  Console.WriteLine(i);
}
```
int array
```cs
// Sort an int
int[] myNumbers = {5, 1, 8, 9};
Array.Sort(myNumbers);
foreach (int i in myNumbers)
{
  Console.WriteLine(i);
}
```
Other useful array methods, such as Min, Max, and Sum, can be found in the System.Linq namespace.
```cs
using System.Linq;
```
## Methods
### Method Overloading
With method overloading, multiple methods can have the same name with different parameters
```cs
int MyMethod(int x)
float MyMethod(float x)
double MyMethod(double x, double y)
```

# Object Oriented Programming Principles
## Namespace
Namespaces are used to organize the classes. It helps to control the scope of methods and classes in larger .Net programming projects. In simpler words you can say that it provides a way to keep one set of names(like class names) different from other sets of names. The biggest advantage of using namespace is that the class names which are declared in one namespace will not clash with the same class names declared in another namespace.

```cs
namespace name_of_namespace {

// Namespace (Nested Namespaces)
// Classes
// Interfaces
// Structures
// Delegates

}
```
## Class
Thik about a house. A class is the blue print for this house. An object is the built house itself.
```cs
public class className
{

    // field variable
    public int a, b;

      // member function or method
      public void functionName()
      {
          Console.WriteLine(“Class & Objects in C#”);
      }
}
```
