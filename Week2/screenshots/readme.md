C# Windows Forms: Variables, Parsing, Type Conversion, & Error Handling

This repository contains various code snippets demonstrating fundamental C# concepts in a Windows Forms application, including variable declaration, parsing input data, type conversion, string concatenation, and error handling.

Code Screenshots & Explanations

1. Error Handling (try-catch) & Variable Initialization

Description: Demonstrates exception handling using a try-catch block. The try block declares variables, parses user inputs from text boxes, and displays the combined result in a label. The catch block catches any parsing or runtime exceptions and displays an error message using a message box.

try {
    // declaring the variables
    int std_age;
    double std_salary;
    string std_grade;

    // initializing variable
    std_age = int.Parse(textBox3.Text);
    std_salary = double.Parse(textBox4.Text);
    std_grade = textBox5.Text;

    // displaying the values in the label using concatenation
    label2.Text = std_age + ", " + std_salary + ", " + std_grade;
}
catch (Exception X)
{
    // error message
    MessageBox.Show(X.Message);
}



2. String Concatenation

Description: Shows how to combine multiple variables (std_age, std_salary, std_grade) and static string separators using the + operator to display them cleanly in a UI label.

// displaying the values in the label using concatenation
label2.Text = std_age + ", " + std_salary + ", " + std_grade;



3. Variable Initialization & Parsing

Description: Assigns values from form text boxes to pre-declared variables by converting string inputs into numeric data types using int.Parse() and double.Parse().

// initializing variable
std_age = int.Parse(textBox3.Text);
std_salary = double.Parse(textBox4.Text);
std_grade = textBox5.Text;



4. Variable Declaration

Description: The initial step of declaring variables with their respective data types (int, double, string) before assigning any values.

// declaring the variables
int std_age;
double std_salary;
string std_grade;



5. Multi-Stage Date Processing

Description: A structured three-stage approach covering:

Creating the required input variables.

Assigning values and processing/concatenating them into a full date format using forward slashes (/).

Rendering the final output to a label control.

//stage 1 : of input / creating variables
string day_week;
string name_month;
int numeric;
int year;
string full_Date;

//initial values to variables
day_week = txtweek.Text;
name_month = txtname.Text;
numeric = int.Parse(txtmonth.Text);
year = int.Parse(txttyear.Text);

// stage 2 : process - concatination of full date
full_Date = day_week + " / " + name_month + " / " + numeric + " / " + year;

// stage 3 : The Output using label
lbloutoutput.Text = full_Date;



6. Parse Methods for Numeric Conversion

Description: Converts string text from UI controls into specific numeric data formats (int and double) to enable arithmetic or logical operations.

// Parse methods to convert string data to numeric data
int hours = int.Parse(lblgross.Text);
double temp = double.Parse(temperatureTextBox.Text);



7. Implicit String Conversion

Description: Demonstrates how C# automatically converts a numeric type (int) into a string when combined with a text string using the + operator.

// implicit string conversion using the + operator
int id_Number = 1200;
string output = "Your ID number : " + id_Number;



8. Using ToString()

Description: Explicitly converts numeric or decimal values into string representations using the ToString() method for presentation in labels or message boxes.

// ToString
decimal gross_Pay = 1890.0m;
lblgross.Text = gross_Pay.ToString();
int my_Number = 100;
MessageBox.Show(my_Number.ToString());