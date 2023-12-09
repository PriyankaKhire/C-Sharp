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
