🔹 What is a Class?

	A class is a blueprint for creating objects. An object is an instance of a class, containing data (attributes) and behavior (methods or functions).

Types of class
	Concrete Class
	Abstract Class
	Sealed Class
	Static Class
	Partial Class
	Nested Class
Examples.

1.Concrete Class

A standard class that can be instantiated (you can create objects from it).

Example: Car, Person, etc.

2.Abstract Class

Cannot be instantiated.

Used as a base class.

Can have both implemented and unimplemented (abstract) methods.

csharp
Copy
Edit
public abstract class Animal
{
    public abstract void MakeSound();
    public void Sleep() => Console.WriteLine("Sleeping...");
}

3.Sealed Class

Cannot be inherited.

Useful when you want to prevent other classes from deriving from it.

csharp
Copy
Edit
public sealed class Calculator
{
    public int Add(int a, int b) => a + b;
}

4.Static Class

Cannot be instantiated.

All members must be static.

Often used for utility or helper functions.

csharp
Copy
Edit
public static class MathHelper
{
    public static int Square(int x) => x * x;
}

5.Partial Class

Allows splitting the definition of a class into multiple files.

csharp
Copy
Edit
// File1.cs
public partial class MyClass
{
    public void Method1() { }
}

// File2.cs
public partial class MyClass
{
    public void Method2() { }
}
