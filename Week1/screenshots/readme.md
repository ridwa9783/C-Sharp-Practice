# C# Windows Forms: UI Controls, MessageBox, and Form Navigation

This repository contains C# Windows Forms code snippets demonstrating basic UI interactions, displaying message boxes, modifying label texts, controlling picture box visibility, and handling form/application closure.


## Code Screenshots & Explanations

### 1. Print Hello Message (`MessageBox`)
* **Description:** Displays a pop-up dialog box containing a greeting message to the user[cite: 9].
```csharp
// print hello ridwa
MessageBox.Show("hello ridwa");


### 2. Application Exit

* **Description:** Completely terminates and exits the entire running Windows Forms application.



```csharp
// application exit
Application.Exit();

```


### 3. Close the Current Form

* **Description:** Closes the currently active form window without necessarily shutting down the entire application process.



```csharp
// close the form
this.Close();


### 4. Control Picture Box Visibility

* **Description:** Changes the visibility property of a picture box control to make it visible on the form interface.



```csharp
// make visible the picture box
st_picturebox.Visible = true;

```


### 5. Change Label Text

* **Description:** Updates the text property of a specific label control (`labelanswer`) to display a new string value.


```csharp
// changing the text label
labelanswer.Text = "Roodo warsame cusmaan";