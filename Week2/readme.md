# Week 2 - Chapter 2: Processing Data

## Introduction

Chapter 2 is about processing data in a C# Windows Forms application. I learned how to get input, store data, perform calculations, convert values, and handle errors.

## 1. TextBox Input

A TextBox allows the user to enter data.

The entered value can be accessed through the `Text` property.

```csharp
string name = nameTextBox.Text;
````

TextBox input is treated as a string.

To remove the entered text:

```csharp
nameTextBox.Clear();
```

## 2. Variables

A variable is used to store a value in memory.

```csharp
string name;
int age;
```

A variable can also be given a value when it is declared:

```csharp
int age = 20;
```

## 3. Data Types

The data type tells C# what kind of value a variable stores.

* `string` - text
* `int` - whole numbers
* `double` - decimal numbers
* `decimal` - decimal values

Example:

```csharp
string name = "Ahmed";
int age = 20;
double temperature = 36.5;
decimal price = 25.50m;
```

## 4. Variable Names

Variable names should describe the information they contain.

```csharp
string firstName;
int studentAge;
double totalAmount;
```

Spaces are not allowed in variable names, and C# keywords cannot be used as names.

## 5. String Values

A `string` stores text.

```csharp
string name = "Ahmed";
string university = "Jamhuriya University";
```

Strings can contain letters, numbers, spaces, and other characters.

## 6. Concatenation

Concatenation means joining values together.

The `+` operator can be used for this.

```csharp
string firstName = "Ahmed";
string lastName = "Ali";

string fullName = firstName + " " + lastName;
```

The result is:

```text
Ahmed Ali
```

A string can also be joined with a number.

```csharp
int age = 20;
string message = "Age: " + age;
```

## 7. Local Variables

A local variable is declared inside a method.

It can only be used in the area where it is declared.

```csharp
private void button1_Click(object sender, EventArgs e)
{
    int age = 20;
    MessageBox.Show(age.ToString());
}
```

Here, `age` is a local variable.

## 8. Initializing Variables

Initialization means giving a variable its first value.

```csharp
int age = 20;
```

A local variable needs a value before it can be used.

## 9. Numeric Types

C# has different types for numbers.

```csharp
int students = 30;
double temperature = 36.5;
decimal price = 25.50m;
```

`int` is mainly used for whole numbers, while `double` and `decimal` can store decimal values.

## 10. Numeric Literals

A numeric literal is a number written directly in the code.

```csharp
int age = 20;
double value = 15.5;
decimal price = 25.50m;
```

The `m` shows that `25.50` is a decimal value.

## 11. Type Casting

Type casting changes a value from one type to another.

```csharp
decimal money = 100.75m;
int value = (int)money;
```

The decimal part is removed when converting this value to `int`.

Another example:

```csharp
int number = 10;
double result = (double)number;
```

## 12. var Keyword

The `var` keyword allows C# to determine the type from the value.

```csharp
var name = "Ahmed";
var age = 20;
var price = 25.50m;
```

A `var` variable must have a value when it is declared.

## 13. Arithmetic Operators

Arithmetic operators are used for calculations.

| Operator | Meaning        |
| -------- | -------------- |
| `+`      | Addition       |
| `-`      | Subtraction    |
| `*`      | Multiplication |
| `/`      | Division       |
| `%`      | Remainder      |

Example:

```csharp
int x = 10;
int y = 5;

int sum = x + y;
int difference = x - y;
int product = x * y;
int division = x / y;
```

Parentheses can be used when the order of calculation matters.

## 14. Integer Division

When two integers are divided, the result is also an integer.

```csharp
int x = 7;
int y = 3;

int result = x / y;
```

The result is `2`, because the decimal part is not included.

## 15. Reading Numeric Input

TextBox values are strings, so numeric input needs to be converted before calculations.

```csharp
int age = int.Parse(ageTextBox.Text);
```

For decimal values:

```csharp
double temperature = double.Parse(temperatureTextBox.Text);
```

## 16. Parse Method

The `Parse()` method converts a string into a numeric value.

Common examples:

```csharp
int.Parse()
double.Parse()
decimal.Parse()
```

Example:

```csharp
int number = int.Parse(numberTextBox.Text);
```

## 17. ToString Method

The `ToString()` method converts a value into a string.

This is useful when displaying numbers in Labels.

```csharp
int number = 100;

resultLabel.Text = number.ToString();
```

A number can also be joined with text:

```csharp
int age = 20;

resultLabel.Text = "Your age is " + age;
```

## 18. Formatting Numbers

`ToString()` can also be used to format numbers.

```csharp
double number = 12345.678;

string result = number.ToString("N2");
```

`N2` displays the number with two decimal places.

## 19. Exception Handling

An exception is an error that happens while the program is running.

For example, entering letters where a number is expected can cause an exception.

Exception handling allows the program to deal with these errors.

## 20. try-catch

The `try` block contains code that may cause an error.

The `catch` block handles the error.

```csharp
try
{
    int age = int.Parse(ageTextBox.Text);
}
catch
{
    MessageBox.Show("Please enter a valid number.");
}
```

If the input is not a valid number, the `catch` block runs.

## 21. Exception Message

The exception object contains information about the error.

```csharp
try
{
    int number = int.Parse(numberTextBox.Text);
}
catch (Exception ex)
{
    MessageBox.Show(ex.Message);
}
```

`ex.Message` gives the message related to the error.

## 22. Named Constants

A named constant is a value that does not change while the program is running.

The `const` keyword is used to create one.

```csharp
const double INTEREST_RATE = 0.05;
```

After a constant is assigned a value, it cannot be changed.

Constants are useful for values that should remain the same in the program.

## Conclusion

Chapter 2 helped me understand how data is entered and processed in C#. I learned about variables, data types, TextBox input, calculations, type conversion, `Parse()`, `ToString()`, number formatting, exception handling, and named constants.
