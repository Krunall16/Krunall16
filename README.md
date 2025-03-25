# interview question


## 1. What is Flutter ?
Flutter is Google's open-source UI toolkit for natively compiled applications for mobile, web, and desktop from a single codebase.

Flutter uses Dart as its primary language

Powerful Features :

- Hot Reload
- Code Reusability
- Rich UI capabilities, including animations, scrolling, and transitions.


## 2. What a widget is in Flutter?
In Flutter, everything on the screen is a widget. 

a widget is the fundamental building block of the user interface (UI)

2 types of widget :

StatelessWidget is a immutable. Once they are built, their properties cannot change. For example, Icon, text, container, etc..

StatefulWidget has a mutable state and can change any time. 
buttons, forms, counters, text fields, and progress bars etc..


## 3.Difference between StatelessWidget and StatefulWidget.
a StatefulWidget can change its state and appearance dynamically, while a StatelessWidget remains static after being built, with its properties and UI being immutable.

Stateless Widget :  
Stateless Widget Used for UI elements that don't change or update during the app's runtime; they are static.
Do not depend on any external data or user input. 
For Example: Text, Icon, container, RaisedButton are Stateless Widgets. 
 
Stateful Widget:  
Stateful Widgets are the ones that change its properties during run-time. They are dynamic and mutable
They can be updated during runtime based on user action or data change.  
For Example: Checkbox, Radio Button, Slider are Stateful Widgets


## 4. Some major features of flutter why choose flutter  
#### Cross-Platform Development:  
Flutter allows you to write a single codebase that can be deployed on multiple platforms (Android, iOS, web, desktop).   
#### Expressive and Customizable UI:  
Flutter's widgets are highly customizable, allowing developers to create unique and visually appealing user interfaces. 
#### Fast Development Cycle:
Flutter's "hot reload" feature allows developers to see changes instantly, speeding up the development process. 
#### Rich Widget Library:
Flutter provides a comprehensive set of pre-built widgets, making it easier and faster to create user interfaces. 
#### Open Source and Free:
Flutter is an open-source framework, meaning it's free to use and has a large and active community. 
#### Dart Programming Language:
Flutter uses Dart, a modern, object-oriented language known for its efficiency and ease of learning. 
``
### Why Choose Flutter?
Cost-Effective,
Faster Time to Market,
High-Quality Apps,
Large and Active Community
Google Support



## 5. Difference between var let and const varialble
#### var:  
Function-scoped, meaning a variable declared with var is accessible throughout the entire function in which it's declared, or globally if declared outside any function.  
#### let and const:  
Block-scoped, meaning a variable declared with let or const is only accessible within the block (code enclosed in curly braces {}) where it's declared.  

#### var and let: 
Allow re-assignment (changing the value of the variable).  
#### const: 
Does not allow re-assignment. Once a variable is declared with const, its value cannot be changed


## 6. What is Function and Method ?
a function is a standalone block of code designed to perform a specific task. It is called by its own name/independently   
a method is a function that is associated with a class or an object, defining behaviors and operations related to those objects. It is called by its object’s name/referenced.


## 7. Difference between dynamic, var, and final
Dynamic allows type changes at runtime, var infers the type at compile time but doesn't allow type changes, and final declares a variable whose value cannot be changed after initialization.  
#### Dynamic:  
Allows the variable's type to change during runtime.   
Skips type checking at compile time, providing maximum flexibility.   
Type checking occurs during runtime, potentially leading to errors if type mismatches occur.   
Example:  Dynamic myVariable = 10; myVariable = "Hello"; (valid)  
#### Var:  
Infers the type of the variable at compile time based on the assigned value. 
The type cannot be changed after initialization.  
Example: var myVariable = 10; // myVariable is inferred as int. myVariable = "Hello"; // Error: type mismatch.  
#### Final:  
Creates variables whose values cannot be changed once assigned, ensuring immutability.  
Example: final myVariable = 10; // myVariable is final. myVariable = 20; // Error: cannot reassign a final variable. 


## 8. What is State ?
- The state of a Flutter app refers to all the objects it uses to display its UI or manage system resources.  
- "state" refers to the data or information that a widget uses to determine its visual appearance and behavior, which can change over time and affect the UI
#### Types of State:
You can think of state as either ephemeral (local to a single widget) or app state (shared across multiple widgets).  
- Ephemeral State:  
This is state that is contained within a single widget and doesn't need to be shared with other parts of the app. 
- App State:  
This is state that needs to be shared or accessed by multiple widgets. 


## 9. Difference between a flutter package and plugin.
- Packages in Flutter are pre-built collections of code that provide more features and capabilities to your app.
- Plugins are a subset of packages that are specifically designed for interfacing with platform-specific, native code or services.  
- "package" contains only Dart code.  
"plugin" contains both Dart and Native code (kotlin/js/swift/...)


## 10. What language does Flutter use for app development?
Flutter is a UI toolkit for building natively compiled applications, uses the Dart programming language for app development.  
Flutter draws its strengths from the powerful Dart programming language. Dart, designed by Google.  
Dart allows Flutter to create apps that run on multiple platforms, including mobile (Android and iOS), web, and desktop.


## 11. How do you create a scrollable list in Flutter?
Two primary choices for Create a scrollable list in Flutter : ListView and GridView.
- **ListView** : Vertical or horizontal scrollable list.
- **GridView** : Grid-based list - can be scrollable in both axes.
#### Listview Types : 
**ListView** : Basic vertical list.  
**ListView.builder** : Recommended for large datasets to render on-demand.  
**ListView.separated** : Useful for adding separate dividers or specific items between list items.  

#### GridView Types
**GridView.builder** : Like ListView.builder, it's best for large datasets to render on-demand for performance reasons.  
**GridView.count** : For a fixed number of grid columns or rows.  
**GridView.extent** : Specifies the maximum cross-axis extent of each grid item.  
**GridView.staggered** : For grid items of varying sizes.


## 12.Flutter app lifecycle.
The Flutter app lifecycle describes the different states an app transitions through during its execution, including starting, running in the foreground, being paused in the background, and eventually being terminated.  
The lifecycle refers to the various states an app goes through from its launch to its termination.
- **Resumed** : Running and fully visible.
- **Inactive** : Visible but can't interact, often during calls.
- **Paused** : The app is either partially visible or fully covered.


## 13. How do you handle user input in Flutter?
In Flutter, you handle user input primarily using widgets like **TextField** and **TextFormField**.
**Flutter** offers various widgets to manage user input, including textual, selection-based, and platform-specific inputs.

#### Common Input Widgets

- **Text**: For basic textual input
- **TextField**: Provides a more comprehensive experience, supporting gestures such as tapping and dragging

#### Text Input

- **TextField**: Offers robust text entry capabilities, including keyboard input, selection, and auto-correction.
- **CupertinoTextField**: Customized for iOS to maintain platform familiarity.

#### Numerical Input

- **CupertinoTextFormField**: Optimized for numerical input in iOS.
- **TextField**: Set the input type to **TextInputType.number**.

#### Password Input

- **CupertinoTextField**: Utilize the `obscureText` property within a Material-based or Cupertino-styled **TextFormField**.


## 14. Explain the purpose of the `main.dart` file.

In a Flutter project, **main.dart** serves as the **entry point** for the application. When you run your Flutter app, this is the first file that gets called.

#### File Structure

1. **Lib Directory**: This is the default location for all of your Dart code files.
2. **Asset Directory**: For resources such as images, fonts, and data files.
