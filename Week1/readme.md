# Week 1 - Chapter 1: Introduction to Visual C#

## Introduction

Chapter 1 introduces the basic parts of C# Windows Forms and how Visual Studio is used to create applications.

## 1. Objects

An object is a part of a program that has properties and methods.

- Properties describe the object.
- Methods perform actions.

Example: A Button has a `Text` property and can perform an action when clicked.

## 2. Controls

Controls are objects placed on a Windows Form.

Examples:

- Label
- Button
- TextBox
- PictureBox

## 3. .NET Framework

.NET provides classes and tools used to build applications. C# is one of the languages that works with .NET.

## 4. Visual Studio

Visual Studio is an IDE used to create C# applications.

Important parts:

- Designer - design the form
- Toolbox - contains controls
- Solution Explorer - shows files and projects
- Properties Window - changes object properties
- Code Editor - writes code

## 5. Projects and Solutions

A project contains the files of an application.

A solution can contain one or more projects.

```text
Solution
   └── Project
        └── Files
```

## 6. Forms and Controls

A Form is the main window of a Windows Forms application.

Controls can be added from the Toolbox and can be moved, resized, deleted, or changed through the Properties Window.

## 7. Properties

Properties control the appearance and behavior of objects.

Examples:

```text
Text
Size
BackColor
Name
```

## 8. Naming Controls

Controls need names so they can be used in code.

C# commonly uses camelCase.

Examples:

```csharp
showDayButton
scoreLabel
displayTotal
```

Spaces are not allowed in control names.

## 9. GUI

GUI means Graphical User Interface.

It allows users to interact with the application using controls such as Buttons, TextBoxes, Labels, and Pictures.

## 10. C# Code

C# code is organized into:

- Namespace
- Class
- Method

A method contains statements that perform an operation.

## 11. Form1.cs

`Form1.cs` contains the code for the Form1 form.

The constructor normally contains:

```csharp
InitializeComponent();
```

This initializes the controls and components of the form.

## 12. Event-Driven Programming

Windows Forms applications are event-driven.

The program waits for an event and then responds to it.

Examples:

- Button click
- Key press
- Mouse movement

An event handler contains the code that runs when an event happens.

## 13. MessageBox

A MessageBox is used to display a message to the user.

```csharp
MessageBox.Show("Hello World");
```

## 14. Label Controls

A Label is used to display text.

Common properties include:

- `Text`
- `Name`
- `Font`
- `AutoSize`
- `TextAlign`

## 15. IntelliSense

IntelliSense helps while writing code in Visual Studio.

It gives suggestions for methods, properties, variables, and other code elements.

## 16. PictureBox

A PictureBox is used to display images.

Important properties include:

- `Image`
- `SizeMode`
- `Visible`

## 17. Sequential Execution

C# normally executes statements from top to bottom.

```csharp
pictureBox1.Visible = true;
pictureBox2.Visible = false;
```

The first statement runs before the second one.

## 18. Comments

Comments explain code and are ignored when the program runs.

Single-line comment:

```csharp
// Close the form.
```

Block comment:

```csharp
/*
   This is a comment.
*/
```

## 19. Blank Lines and Indentation

Blank lines and indentation make code easier to read.

```csharp
private void button_Click(object sender, EventArgs e)
{
    MessageBox.Show("Hello World");
}
```

## 20. Closing a Form

To close the current form:

```csharp
this.Close();
```

To exit the application:

```csharp
Application.Exit();
```

## 21. Syntax Errors

A syntax error happens when code does not follow C# rules.

Visual Studio usually shows syntax errors with a red underline.

Examples include missing brackets, quotes, or other required symbols.

## Conclusion

Chapter 1 helped me understand the basic parts of C# Windows Forms, including objects, controls, forms, properties, Visual Studio, events, MessageBox, Labels, PictureBox, comments, and syntax errors.