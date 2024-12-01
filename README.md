
# History of C#                                                                     Telerik Academy
> Developed by Mircrosoft in 2000
> Base on Java and C++, but has many additional features
> Java and C# are both being updated to keep up with each other
> Cross-development with Visual Basic, Visual C++, and many other .NET languages.

# Why to use C#?
> Pure Object Oriented Language.
> Power of C and Microsoft Visual Basics
> Easy to learn for everybody
> Provides More support for Web development 
> More powerful like Java
> Latest version of C# 13, that is released in 2024.

# C# : A component oriented language
> The first "component oriented" language in the C/C++ family
    => In OOP a component is: A reusable program that can be combined with other components in the sme system to form an application.
    => Example: a single button in a graphical user interface, a small interest calculator 
    => They can be deployed on different servers and communicate with each other.

> Always use Main() unlike main() in C/C++ 
> Do not terminate class by semicolon

C# Overview
-------------
> Object oriented
> Everything belongs to a class
> complete C# program

    using System;
    namespace ConsoleTest
    {
        class Class1
        {
            static void Main(string[] args)
            {

            }
        }
    }

# C# Program Structure

=> Namespaces
> Contain types and other namespaces
=> Type declareations
> Classes, structs, interfaces, enums, and delegates
=> Members
> Constants, fields, methods, properties, indexers, events, operators, constructors, destructors

# Learning strategies of C#

1. Data types
2. Operators
3. Console I/O
4. Conditional Statements
5. Loops
6. Arrays
7. Funcitons 
8. OOP's

 1. Data Types:
 --------------
> Integer Types
    => byte, sbyte(8bit)              // sbite store signed data that is negative data only 
    => short(16bit)
    => int, uint(32bit)                // uint
    => long, ulong (64bit)

> Floating Point Types
    => float (precision of 7 digits)
    => double (precision of 14 digits)

> Exact Numeric Type
    => decimal (28 significant digits)

> Character Types
    => char (single character)
    => string (rich functionality, by-reference type)

> Boolean Type
    => bool

# Console I/O
-------------
=> Provides methods for input and output
=> Input 
    > Read(...) - reads a single character
    > ReadLine(...) - reads a single line of characters

=> Output
    > Write(...) - prints the specified argument on the console
    > WriteLine(...)- prints specified data to the console and moves to the next line
    
# Working with Directories and Files in C#:
-------------------------------------------

=> C# has a built-in namespace "System.IO" that is used to work with files and folders.
=> Files are known as Directory in C#.
=> Directory class works for folder and "File" class works for files.
=> Directory.CreateDirectory() function is used to create a new folder using C#.
=> Directory.Exists() function is used to check that folder exists or not.
=> Directory.Delete() function is used to remove a folder.
=> "FileInfo" class is used to tpo get (read) all information about a File.

# Starting a System Process using C#
-------------------------------------
=> "System.Diagnostics" is a namespace that provides us a class named as "Process". This process class is used to start a system process.

=> Process.Start() function starts a process.

=> We have to specify name of executable file of process to start a process.
    Ex: Process.Start("mspaint.exe);

# Types of Loops in C#
------------------------
=> For while                                (just like c)
=> While Loop                               (just like c)
=> Do while loop                            (just like c)
=> For each loop                            (new loop)

# Working with Date and time
----------------------------
=> In c#, there is  a "DateTime" class that is used to work with date and time
=> To get the current date and time we have to use "DateTime.Now". It will return current DateTimeis DAteTime format.
=> To create the object of a specific date time we have to create object of DateTime class as shown below:
    DateTime dt = new DateTime(1999,5,22);
=> We can convert a value of any type in string format by using ".ToString()" function.

# Foreach loop
---------------
=> For each is a loop in C#  that is used to work with collections of string, array, array of objects, etc.

=> Foreach loop works on the basis of items. It not works on index. It is an item based on loop

=> This loop is used to fetch each item from the collection one by one.

    Syntax:
        foreach(VarName in CollectinName)
        {
            //statements...
        }

> Note: Here VarName must be a local variable variable of foreach loop. It is a read only variable. VarName must be of type  of a single item in collection.

Ex: 
    string friends = "Amit Vikas Durgesh Shivam Sandeep Satya"
    foreach(char ch in friends)
    {
        Console.write(ch);
    }

# Implenting some delay in program
-----------------------------------
=> To mention some delay between execution of code we have to use "Sleep()" function of "Threa" class.

=> Thread class is located under "System.Thread
" namespace.

=> Sleep() is a static method. We have to specify duration of delay in milliseconds.
    Ex: Thread.Sleep(4000);

# Array in C#
-------------
=> An array is a collection of same type of various data items.
=> It is used to store bulk data.
=> First index of an array is 0 and last index is size - 1.
=> C# provides "Length" property in array to find the number of items (size) of an array.

Syntax to declare an array:
-----------------------------
DataType [] ArrayName = new DataType[size];

    e.g.: int [] arr = new int [10];

Syntax to declare to initilize an array
------------------------------------------
DataType [] arrayName = {item1,item2,item3,item4,........};

    e.g.: string [] names = {"Amar","Ramesh","Mahesh","Sarvesh","Indra"};

# Array class
==============

=> C# provides a built-in class with name "Array". This Array class provides us some functions to perform operatons on an Array.

Sort(): This function is used to sort the items of an array in ascending order.

BinarySearch(): This funciton is used to search an item in an array by using binary search algorithm.

IndexOf(): This function is used an item in an array by using linear search algorithm. It returns -1 if item not found otherwise it return index of search item in array.

# 2-D Array
=============
=> Two dimentional array is used to store data in matrix format.
=> 2-D array is used to store large amount of data.
=> It stores data in pair of row,column index.

>Syntax to create a 2-D array
------------------------------
data_type [,]ArrayName=new data_type[Number_of_rows,Number_of_columns];

Ex: int [,]arr = new int[3,2];
Note : Above 2-D array can store max 6 items.

2-D array is also known as Matrix. We have to use nested loop to process a 2-D array.

# String in C#
===============
=> In C# string is a data type and string is a class also.
    Ex: data type: string
            class: String

=> String is a sequence (collection) of characters.

Syntax to declare a string variable:
-------------------------------------
string var_name;
Ex; string name;

Syntax to declare and initilize a string variable:
----------------------------------------------------
string var_name = "value"
Ex: string name = "Ramesh Kumar";

>Notes: In C# string is written inside double quotes.

# Some important properties and method of string in C#
========================================================
1. Length: Used to number of characters in a string.
2. ToUpper(): Used to convert a string into uppercase.
3. ToLower(): Used to convert a string into lowercase.
4. Contains(): Used to check for a character or word in given string. If found then it returns true otherwise returns false. 
5. IndexOf(): Used to find firat occurance index of a character or word ina given string. If found then it return indexof that , otherwise it returns -1
6. LastIndexOf(): Used to find last occurance or word in given string. If found then it returns index of that item; otherwise it returns -1.
7. Trim() : Used to remove whitespace from beginning and ending of string.
8. Substring(): Used to get part of a string (substring)
    Syntax 1: StringVar.Substring(int StartIndex);

    Note: It will provide a substring starting from the specified index and ending to length of main strin.

    Syntax 2: StringVAr.Substring(int StartIndex, int Length);

    Note: It will provede fixed number of characters starting from the specified start index
9. Split(): Used to break a string into an array.
10. Insert(): Used to insert new string into existing and returns result in new string.
        Syntax: 
            str = mystr.Insert(5,"Hello");

            Note: - String will be inserted into existing string just after specified index.

# Static Function: 
------------------
=> Static functions are special kind of functions in a class.

=> If a function is of static type then it can use (call) only static members (variables) and static methods. It can't use any non -static methods. It can't use any non-static element.

=> By default all members of a static function are of static type.

=> Default values of a static function is 0.

=> Static functions of a class are called by using the class name just before the function name. Ex if Student class have a static function having anme "PrintData()". Then we call it as given below:
    Student.PrintData();

=> No need to create object of class for calling static method.Static functions can be loaded in memory directly without creating object of it's class.

=> "static" is a store specifier. It preserve it's value during program execution. A static variable not losses it's value.
Static variables are allocated memory in the data segment; not in stack or heap

===================================================================================================================
# Branching Statement
----------------------
1) break:
        => It is used to terminate the execution of current block.
        => Generally is used inside switch and looping statements.
    
2) continue:
        => It is used to skip the current iteration of a loop.

        => After skipping the current iteration it continuous in next iteration.

============================================================================================================================

# Object Oriented Programming
------------------------------
=> Object Oriented Programming is a concept of writing computer programs in modern ways.
=> It is methodology to write computer programs.
=> It is very famous and trustful method to write programs.
=> "Object oriented programming is a concept that uses the concept of object to write computer programs."
=> Object Oriented programming tries to implement the real world human behaviour in computer programs.
=> Object Oriented programming is a collection of some objects and when we use that concept in our program then our program will be an object oriented program.
That concepts are also known as OOP's Concepts or Features of OOP's.

=> The languages that are providing support for concepts of object oriented language, are known as Object Oriented Programming languages.

    Example of OOP's Languages are: C++, Java, PHP, C#, VB.NET, Python,etc.

> C# is pure object oriented programming language . It supports all concepts of OOP's. It strictly uses concepts of OOP's.

====================================================================================================================================

# Features/Concepts/Pillers of OOP'S
1. class
2. object
3. Data Encapsulation
4. Data Abstraction
5. Inheritance
6. Polymorphism
7. Message Passing


----------------------------------
# 1. Class
==========
=> Class is a container.

=> A class is a collection of various variables and various functions.

=> In OOP's ; variables of a class is known as "data members" and functions of a class are known as "data methods". Hence, Class is a collection of various data members and various data methods in a single unit.

=> Class provides security to data members and data methods.

=> Class implements portability in our program. We can use a class easily from one program to another program also.

=> Class provides reuseability to code. We can create object of a class many times.

=> "class" keyword is used to declare /create a class.

    Syntax: 
    ------
        class <Class_Name>
        {
            //data members
            //data methods
        }

2) Object
-----------
=> Object is a runtime entity that is used to represent the features of a class. It means object exist in runtime of program and by using object we can access the features of a class. (Features means class variable and function)

=> Object is a copy of class in memory. means It is a copy of class that is loaded into memory. 

=> Object creation is a memory initilization. It means when object created at that time memory will be allocated to all members of class.

=> We can create n number of object of a class as per need. 

=> All object of a class is separate separate memory space.

Syntax to create a object of a class
-----------------------------------
    <Class_Name> ObjectName = new <Class_Name>();

    Ex: Student s = new Student();


> Note:- Class is user defined data type also.

# Constructor
================
=> Constuctor is a special member function of a class.

=> Constructor is used to initilize the members of a class. Means we can assign/allocate some value to the members of a class by using constructor.

=> We can perform any operation inside constructor but generally it is used to assign members of class. 

Characteristics of Constructor
===============================
1) Name of constructor must be same as name of class.
    Ex: For class Employee constructor name must be "Employee".

2) No need to call constructor function because it automatically executes when we create object on that class.

3) A constructor can't return any value . So need to specify any return type for constructor. Even "void" is also not allowed.

4) It is recommended to put/ make a constructor with public access.
    Becuase, It will execute automatically when we create object of class from outside the class.

5) A constructor can be of static type. But It can't be a constant.

6) Constructor can have parameters or it can be without any parameters.

7) We can create multiple constructor in a class.

# Types of Constructor
-----------------------
1. Default Constructor: 
    => A constructor that has no any parameter is known as deffault constructor. It assigns default values to members of class.

2. Parameterised Constructor:
    => A constructor having some parameters is known as parameterised constructor.

3. Copy Constructor:
    => A constructor that have address of some members in parameter is known as copy constructor. It works on the basis of address of parameter. In C#, pointer is not supported in safe mode, Hence copy constructor in not generally used in C#.

# Destructor
------------

=> Destructor is used to destroy (free/release ) memory space occupied of un-necessary variables adn objexts.

=> It impoves the performance of program /software.

### 3. Data Encapsulation
* Wrapping of data members and data methods in a single unit is known as "Data Encapsulation".
* Data Encapsulation makes portable to a program/class.
* "class" is used to implement data encapsulation.

### 4. Data Abstraction
* Data Abstraction is used to implement security in our program.
* "Data abstraction means data hiding". To provide only necessary information to the end user without providing details of internal functionality is known as "Data Abstraction".
* Data abstraction can be achieved by using two below concepts.
1. Access Specifiers.
2. Abstract Class.

#### 1. Access Specifiers :
---------------------------
* Access specifiers are used to define the access level or lifespan or programming elements.
* Access specifiers are used before variables, constants, classes,functions etc to define it's access level.
* Access specifiers are also known as access modifiers or protection level.
* In C#; We have 4 types of access specifiers.
A. Private:
* It is most Rectricted access specifiers.
* Private members / functions will be accessible only with-in the block where they are declared.

B. Protected:
* Protected is more usefull in parent-child relationship.
* Protected members of a class will be accessible inside the same class and also inside it's child class.
* Protected members are accessible from the child class located in same assembly and also from the child class located inside another assembly.

C. Public:
* Public is most flexible access specifier.
* Public members of a class will be accessible in whole program.

D. Internal:

* Internal access specifiers is of assembly level.
* Internal members can be accessed from any where in same assembly.

Note: Here assembly is a namespace or a collection of more 
than one namespaces.

2. Abstract Class:
* We will cover this topic later on after inheritance.


Assembly
=========
=> An assembly is a collection of namespaces. We can put one or many namespaces inside an assembly.

=> Assemblies are also known as "Class Library" or DDL files.

=> DDL stands for "Dynamic Link Library".

=> DDL is a ready to use library that can be dynamically and quickly used in another program.

=> "Class Library" contains some code without any entry point (main).

===================================================================================================
# 5) Inheritance:
------------------

=> Inheritance is the ability to access the features of a class inside another class.

=> The class that provides features is known as base class/parent class/super class/main class.

=> The class that uses features is known as derived class/child class/sub class

=> Inheritance is one of the most important concept of OOP's. 
    > It provides  reusuability of code.

=> Inheritance saves time and effort of a programmer. Because it provides reusability.

=> In C# ":" colon symbol is used to inherit the class.

Syntax to inherit a class:
--------------------------
    class<Sub_Class_name>: <Super_Class_Name>
    {
        //data members
        //data methods
    }

# Types of Inheritance
----------------------
1. Single Inheritance
2. Multilevel Inheritance
3. Hierarchical Inheritance
4. Hybrid Inheritance

Note: Multiple Inheritance is not supported in C#.


* 1) single inheritence

            class-A
                ⬇
                ⬇
            class B

* 2) multilevel inheritence

                class A
                    ⬇
                    ⬇
                Class B
                    ⬇
                    ⬇
                Class C
                    ⬇
                    ⬇
                class D
* 3) Hierarchical inheritence

                class A
                    |
            --------------------
            |                 |
            ⬇                 ⬇
          Class B            Class C


* 4) hybrid inheritence

            class A
               ⬇    Singlular
            class B
       _________|___________  Hierarchical
       ⬇                    ⬇
    Class C             Class D

* 5) Multiple inheritance : (Not supported in C#)


    Class A         Class B             Class C
       |______________|____________________|
                      | 
                      ⬇
                    Class D

* 6) Polymorphism:
-------------------
=> Polymorphism means "one thing in many form"/

=> Poly means many an dmorphism means "form". Hence, Polymorphism means one thing in many form.

=> We can use same function name for different different purpose by using Polymorphism. It makes easy to remember name of functions for a developer.

## Types of Polymorphism:
===========================
1) Compile Time Polymorphism (Early Binding)
--------------------------------------------
=> When a function call decides actual calling function during compilation process of program then it is knoen as compile time Polymorphism.

=> Function overloadig is known as compile time Polymorphism.

2) Run Time Polymorphism (Late Binding)
---------------------------------------
=> When a function call decides actual calling function during run-time of program then it is known as run time Polymorphism.

=> Function overriding is known as run time Polymorphism.

### Function Overloading
-----------------------
=> To define more than one function having same function name and different-2 signature (syntax/parameters) is known as function overloading.

=> All overloaded function are defined in same class. 

=> We can overlaod a function in tow below basis;
    
    A) On the basis of number of parameters:
    ------------------------------------------
    Ex: int Add(int num1,int num2)
        int Add(int num2,int num2, int num3)

    B) On the basis of types of parameters:
    -----------------------------------------
    Ex: void PrintMax(int num1,int num2)
        void PrintMax(float num1, int num2)
        void PrintMax(float num1, int num2)

Note: - We can't overload a function on the basis of it's return type.

### Function Overriding:
----------------------
=> To define more than one function with same function name and same signature (syntax/parameter) is known as function overriding.

=> Function overriding is used to redefine (to give a new definition to a function of base class) a function of base class inside child class.

=> By using function overriding a child class can change definition of a function of base class as per need.

=> To perform function overriding we need two classes parent and child class.

=> To make overridable function we need to use a virtual or abstract function in base class.

## Virtual Function:
--------------------
=> Virtual Function is special function of a class. This function can be redefined (override) by its child classes.

=> "virtual" keyword is used to create a virtual function.

=> Virtual function has a default definition in base class also.

=> It is not mandatory to child classes to override virtual function of base class.

=> It is optional for child class to override a virtual function of base class.

=> To override a virtual function in child class we have to use "override" keyword.

## abstract function:
===========================
=> An abstract function is a function of base class that has not any definition is has declaration only

=> It is mandatory for child class to ovverride abstract function of base class or child class cam also be declared as an abstact class then it can deney(ignor) to override abstarct class
   

=> An abstract function is a funtion without definition in base class.

=> abstract function are create by using "abstract" keyword.

=> We have to use "override" keyword in chilsd class during function ovverriding.

=> Syntaxt to create an abstract function:
-------------------------------------------
<access_specifier> abstract <return_Type> FunctionName
(List_of_Parameters);

Note : abstract function are terminated by using semicolon in base class. it does not have any body.

=> abstract function can be created only with in an abstract class.

 # abstarct class:
--------------------
 => An abstract class is a collection of various abstract and non-abstact function.

 => Abstarc class is a special class. We can't instantialte an abstract class.

 => We can't create object of an abstact class.

 => Abstarct class is only for inheritance.

 => Data abstraction is used to implement data security(hiding) in program. We can achieve abstarction by using abstact class. Because this class can be use only by it's only child class.

 => Abstarct keyword is used to create an abstract class.

 Syntaxt:
 --------
  <access_Specifier> abstract class<Class_Name>
  {
     // data member
     // abstarct & not-abstract data method
  }

 ## abstract function example

     public abstract class Shape
{
    // Abstract method (no body)
    public abstract double GetArea();

    // Concrete method (with body)
    public void Display()
    {
        Console.WriteLine("This is a shape.");
    }
}

public class Circle : Shape
{
    private double radius;

    public Circle(double radius)
    {
        this.radius = radius;
    }

    // Implementation of the abstract method
    public override double GetArea()
    {
        return Math.PI * radius * radius;
    }
}



## Sealed class:
----------------
  => Sealed class is a special class in c#

  => A Sealed class is a class that can't be inherited by any other class.

  => Sealed Keyword is define a sealed class

  ## Syntact:
  -----------
  <access_specifier> sealed class <Class_Name>
   {
    // data members
    // data methods
   } 

## Interface:
===================
=> An interface is a complete abstract class>

=> An interface is a special type that has only function decration.

=> Interface is a collection of various abstract method. All the methods of interface are by default public and abstract. Also no need to write public and abastract keyword.

=> In C# We can't declare of an interface . It is used by child classed

=> Interface is used to implement some concept like multiple inheritance. We can inherit one class and multiple interface inside a child class.

=> It is mandatory for child class to define( implement) all method of an interface.

=> Interface "Keyword" is used to define

 ## Syntax:
 ----------
 
 <access_specifier> interface <interface_name>
 {

    // Declaration of abstract class
 }





