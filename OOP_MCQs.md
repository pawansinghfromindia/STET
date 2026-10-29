
## Object Oriented Programming (OOP)

Q1. What is the purpose of the `super` keyword in java and other similar languages?
- [x] A. It refers to the superclass in inheritance
- [ ] B. It creates a new object instance
- [ ] C. It defines a new class
- [ ] D It handles exceptions

<details>
 <summary> <b> Super keyword in java </b> </summary>

### `super`keyword in Java

The `super` keyword in Java refers to the immediate parent class object. <br/>
It is commonly used in inheritance to access parent-class constructors, methods, and variables.

### 1. Three main uses of super

**Use 1: Access a parent-class variable**
```java
class Parent {
    int x = 10;
}

class Child extends Parent {
    int x = 20;

    void display() {
        System.out.println(super.x);
        System.out.println(x);
    }
}
----------------------------------
Output:
10
20
```
- `super.x` accesses the parent variable.
- `x` accesses the child variable.

**Use 2: Call a parent-class method**
```java
class Parent {
    void show() {
        System.out.println("Parent method");
    }
}

class Child extends Parent {
    void show() {
        super.show();
        System.out.println("Child method");
    }
}

--------------------------
Output:
Parent method
Child method
```

Here, `super.show()` calls the parent method even though the child overrides it.

**Use 3: Call a parent-class constructor**
```java
class Parent {
    Parent() {
        System.out.println("Parent constructor");
    }
}

class Child extends Parent {
    Child() {
        super();
        System.out.println("Child constructor");
    }
}

-------------------------------
Output:
Parent constructor
Child constructor
```

`super()` invokes the parent constructor. <br/>
In Java, it must be the first statement in a constructor when explicitly used.

### 2. Visualize inheritance

<img width="461" height="315" alt="image" src="https://github.com/user-attachments/assets/8dbfbbd6-87ad-437a-9a8b-f38c5e71d654" />


### 3. `this` vs `super`

| Keyword	| Refers to                       |
|---------|---------------------------------|
| `this`	| Current class instance          |
| `super`	| Immediate parent class instance |


> **`this` refers to the current object; `super` accesses members of the immediate parent class.**

</details>
<!---------------------------->

---

Q 2. What are  `abstract` methods?
- [ ] A. Methods that are inaccessible to the outside world
- [ ] B. Methods that have implementations details
- [x] C. Methods without body, defined in an abstract class
- [ ] D. Methods that cannot be inherited
      
<details>
 <summary> <b> Abstract class </b> </summary>

### Abstract class in Java

An abstract class is a class declared with the `abstract` keyword that is designed to be a base class for other classes. <br/>

It can contain both **abstract methods (without a body)** and **concrete methods (with a body)**.

> **An abstract class provides a shared base with some implementation, while subclasses fill in the missing behavior.**

Example
```java
abstract class Animal {
    abstract void sound();  // Abstract method

    void sleep() {          // Concrete method
        System.out.println("Sleeping");
    }
}

class Dog extends Animal {
    @Override
    void sound() {
        System.out.println("Bark");
    }
}

-----------------------
Usage:
Dog d = new Dog();
d.sound();
d.sleep();
------------------------
Output:
Bark
Sleeping
```

### 2. Key rules for exams

- An `abstract` class **cannot be instantiated directly**: `new Animal()` is not allowed.

An `abstract class` is intended to act as a blueprint or base class for other classes. <br/> 
We cannot create its object directly using `new`.
```java
abstract class Animal {
    abstract void sound();
}

// Animal a = new Animal();  // ❌ Compilation error

class Dog extends Animal {
    @Override
    void sound() {
        System.out.println("Bark");
    }
}

Dog d = new Dog();  // ✅ Allowed
d.sound();
```

- It **can contain abstract and concrete methods**.
- A **concrete subclass must implement inherited abstract methods**, unless the subclass is also abstract.
- An abstract class **can have constructors, fields, and static methods**.
- A class can extend only one class in Java, whether abstract or concrete.

### 4. `Abstract class` vs `interface`

| Feature	             | Abstract class	            | Interface                                                     |
|----------------------|----------------------------|---------------------------------------------------------------|
| Keyword	             | `abstract class`	          | `interface`                                                   |
| Constructors	       | Yes	                      | No                                                            |
| Instance fields	     | Yes	                      | No ordinary instance fields                                   |
| Multiple inheritance | One class can be extended	| A class can implement multiple interfaces                     |
| Methods	             | Abstract and concrete	    | Abstract methods and permitted default/static/private methods |


</details>
<!---------------------------->

---

Q 3. What is the term for creating a new class that inherits properties and behaviour from an existing class?
- [ ] A. Polymorphism
- [ ] B. Encapsulation
- [ ] C. Abstraction
- [x] D. Derivation (Inheritance -  Derive class)

<details>
 <summary> Solution </summary>

</details>
<!---------------------------->

---


Q 4. What is the primary purpose of interface in OOP?
- [ ] A. To provide a blueprint for creating object
- [x] B. To define a set of methods must be implemented by implementing class
- [ ] C. To define constructor for classes
- [ ] D. To create static methods


<details>
 <summary> Solution </summary>

<br/>

The primary purpose of an **interface** is to define a contract that specifies what methods a class must provide, 
without requiring the class to inherit a particular implementation.

Example: <br/>
Imagine several animals can make sounds, but each animal makes a different sound.
```java
interface Animal {
    void sound();
}

class Dog implements Animal {
    public void sound() {
        System.out.println("Bark");
    }
}

class Cat implements Animal {
    public void sound() {
        System.out.println("Meow");
    }
}
```
Both `Dog` and `Cat` implement the `Animal` interface, but each supplies its own behavior.

<img width="962" height="282" alt="image" src="https://github.com/user-attachments/assets/be4c37c5-3375-48ec-81b0-5c4cd2abf553" />


### 3. Key terms for exams

- **Abstraction**: Exposes essential behavior while hiding implementation details.
- **Contract**: Specifies behavior a class agrees to provide.
- **`implements`**: Java keyword used when a class implements an interface.
- **Multiple interfaces**: A Java class can implement more than one interface.
- **Polymorphism**: Different classes can be used through the same interface type.

### 4. Interface vs abstract class

| Interface	                                | Abstract class                                               |
|-------------------------------------------|--------------------------------------------------------------|
| Defines a contract	                      | Provides a common base and may provide shared implementation |
| A class can implement multiple interfaces | A class can extend only one class                            |
| Cannot be instantiated	                  | Cannot be instantiated directly                              |
| No constructors	                          | Can have constructors                                        |


> An interface defines **what a class must do**, while the implementing class defines **how it does it.**

</details>
<!---------------------------->

---


Q 5. What is the term for a condition that occurs during program execution that **disrupt the normal flow** of instructions?
- [ ] A. Abstraction
- [ ] B. Inheritance
- [x] C. Exception
- [ ] D. Encapsulation

<details>
 <summary> Solution </summary>

### Error Handling and Exception Handling in Java

**Error handling** is the process of dealing with problems that occur while a program runs, 
so the program can respond appropriately instead of terminating unexpectedly.

**Exception handling** is a specific mechanism in Java for detecting and handling exceptional situations during 
program execution.

**1. What is an exception?**
- An exception is an event that interrupts the normal flow of a program.

Example
```
int a = 10;
int b = 0;

System.out.println(a / b);
```
This causes an `ArithmeticException` because integer division by zero is not allowed in Java.

### 2. The five important keywords

**`try` - test risky code** <br/>
Place code that might throw an exception inside the `try` block.

**`catch` - handle the exception** <br/>
Runs when a matching exception is thrown in the associated `try` block.

**`finally` - cleanup code** <br/>
Usually runs whether an exception occurs or not. It is often used for cleanup.

**`throws` - declare possible exceptions** <br/>
Appears in a method declaration to indicate exceptions the method may pass to its caller.


### 3. How exception handling works

<img width="947" height="451" alt="image" src="https://github.com/user-attachments/assets/fc106c56-30ac-4dc9-ac35-87ffcede0e07" />


```java
public class Main {
    public static void main(String[] args) {
        try {
            int result = 10 / 0;
            System.out.println(result);
        }
        catch (ArithmeticException e) {
            System.out.println("Cannot divide by zero");
        }
        finally {
            System.out.println("Execution completed");
        }
    }
}
--------------------------------------------
Output:
Cannot divide by zero
Execution completed
```
The division throws an exception, so the remaining statements in the `try` block are skipped. <br/>
The matching `catch` handles it, and the `finally` block runs afterward.

### 5. Types of exceptions in Java

**Checked exceptions** <br/>
Checked by the compiler. They must be caught or appropriately declared. <br/>
Examples: `IOException`, `SQLException`.

**Unchecked exceptions** <br/>
Runtime exceptions that do not have to be caught or declared. <br/>
Examples: `NullPointerException`, `ArithmeticException`, `ArrayIndexOutOfBoundsException`.

**Errors** <br/>
Serious problems, generally outside the normal scope of application-level exception handling. <br/>
Examples: `OutOfMemoryError`, `StackOverflowError`.


Note: in Java, `Exception` and `Error` are both subclasses of `Throwable`, but they represent different kinds of problems.

</details>
<!---------------------------->

---


Q 6. What is **Encapsulation** in OOP?
- [ ] A. The ability to inherit properties from multiple classes
- [ ] B. The process of creating object
- [x] C. The bundling of data and methods that operate on data
- [ ] D. The use of abstract class only

<details>
 <summary> Solution </summary>

### Encapsulation in OOP

Encapsulation is the OOP principle of bundling data (variables) and the methods that operate on that data into a 
single unit (a class), while controlling access to the data.

In Java, encapsulation is commonly implemented using private variables and public getter/setter methods.

**1. Real-life example**

Think of an ATM:
- You cannot directly access the bank's internal account balance.
- You interact through controlled operations, such as checking your balance or withdrawing money.
- The system can validate whether a withdrawal is allowed.
This is similar to encapsulation in programming.

```java
class BankAccount {
    private double balance;

    public void deposit(double amount) {
        if (amount > 0) {
            balance += amount;
        }
    }

    public double getBalance() {
        return balance;
    }
}
---------------------------------------
Usage:
BankAccount account = new BankAccount();

account.deposit(500);
System.out.println(account.getBalance());
------------------------------------------
Output:
500.0
```
Here, `balance` is private, so other classes cannot access it directly. <br/>
The `deposit()` method controls how the balance changes, and `getBalance()` allows controlled reading.

<img width="960" height="362" alt="image" src="https://github.com/user-attachments/assets/bc9ae09f-32d1-495d-a5ee-5b9c25150e8d" />


### 4. Important terms

| Term	            | Meaning                                                                            |
|-------------------|------------------------------------------------------------------------------------|
| **Encapsulation**	| Bundles data and methods and controls access.                                      |
| **`private`**     | Restricts access to within the declaring class.                                    |
| **Getter**	      | A method that reads and returns a value.                                           |
| **Setter**	      | A method that updates a value, often after validation.                             |
| **Data hiding**	  | Restricting direct access to internal data; closely associated with encapsulation. |


### Encapsulation vs abstraction

- **Encapsulation**: Controls access to internal data and implementation.
- **Abstraction**: Hides unnecessary implementation details and exposes essential functionality.

> **Encapsulation = data + methods + controlled access.**

</details>
<!---------------------------->

---


Q 7. What is the purpose of a destructor in OOP?
- [ ] A. To create instances of classes
- [ ] B. To handle exception
- [x] C. To free up resources when an object is destroyed
- [ ] D. To define deafult values for properties

<details>
 <summary> Destructor </summary>

<br/>

A **destructor** is a special member function used to perform cleanup when an object is being destroyed, 
such as releasing resources it owns.

**Main purposes**
- Release resources, such as dynamically allocated memory.
- Close files or release other resources when appropriate.
- Perform cleanup before an object's lifetime ends.

Example:
```cpp
#include <iostream>
using namespace std;

class Student {
public:
    Student() {
        cout << "Object created\n";
    }

    ~Student() {
        cout << "Object destroyed\n";
    }
};

int main() {
    Student s;
}
----------------------
Output:
Object created
Object destroyed
```
The destructor is written as `~Student()`. In this example, it runs when the local object `s` goes out of scope.

### 3. Important points
- A destructor has the same name as its class, preceded by `~` in C++.
- It has no `return type` and takes no parameters.
- A class can have only one destructor in C++; it cannot be overloaded.
- Destructors are commonly used for resource cleanup.
- Java does not have C++-style destructors. Java uses garbage collection for memory management, and
   resources such as files should generally be closed using `try-with-resources`.

| Concept	                  | Purpose                                          |
|---------------------------|--------------------------------------------------|
|  **Constructor**	        | Initializes an object                            |
|  **Destructor**	          | Performs cleanup when an object is destroyed     |
|  **Inheritance**	        | Reuses or extends class functionality            |
|  **Operator overloading**	| Defines operator behavior for user-defined types |

> Remember: **Constructor = setup; destructor = cleanup**.

In java we don't have the concept of Destructor bcuz there we have a concept of **Garbage Collector**, automatic freeup memory
and resources by removing the unused variables by default.

</details>
<!---------------------------->

---


Q 8. What is the **main purpose of inheritance** in OOP?
- [ ] A. To create instances of classes
- [ ] B. To prevent data abstraction
- [x] C. To establish a parent-child relationship between classes
- [ ] D. To define exceptions

<details>
 <summary> <b> Inheritance </b> </summary>

<br/>

The main purpose of inheritance in OOP is **to reuse existing code and create new classes from existing classes,
reducing code duplication and supporting extensibility**.

### 1. How inheritance works

<img width="950" height="292" alt="image" src="https://github.com/user-attachments/assets/5390b705-9b1c-4336-b462-8817427c6d1c" />


Both `Dog` and `Cat` inherit the common behavior from `Animal`, while each can define its own behavior.

Example:
```java
class Animal {
    void eat() {
        System.out.println("Eating");
    }
}

class Dog extends Animal {
    void bark() {
        System.out.println("Barking");
    }
}
---------------------------
Usage:
Dog d = new Dog();
d.eat();   // Inherited from Animal
d.bark();  // Defined in Dog
-----------------------------
Output:
Eating
Barking
```
The `extends` keyword establishes class inheritance in Java.

### 3. Points to remember

- **Code reusability**: use existing class functionality.
- **Extensibility**: add new features in child classes.
- **Hierarchical classification**: represent relationships such as Animal → Dog.
- **Method overriding**: a child class can provide its own implementation of an inherited method, supporting runtime polymorphism.

> **Inheritance = `IS-A` relationship + code reuse**.

For example, a `Dog` is an `Animal`.

</details>
<!---------------------------->

---


Q 9. What is the term for defining multiple methods in a class with the same name but different parameters?
- [ ] A. Overriding
- [x] B. Overloading
- [ ] C. Inheriting
- [ ] D. Inheritance

<details>
 <summary> Method overloading </summary>

**Method overloading** means defining multiple methods in the same class with the same name but different parameter lists.

```java
class Calculator {
    int add(int a, int b) {
        return a + b;
    }

    int add(int a, int b, int c) {
        return a + b + c;
    }

    double add(double a, double b) {
        return a + b;
    }
}
```
All three methods are named `add`, but their parameters differ.
- `add(int, int)` -> two integer parameters
- `add(int, int, int)` -> three integer parameters
- `add(double, double)` -> two double parameters
Java determines which method to call based on the arguments supplied.

| Method overloading	                   | Method overriding                                              |
|----------------------------------------|----------------------------------------------------------------|
| Same method name, different parameters | Same method signature, with a new implementation in a subclass |
| Usually occurs within the same class   | Requires inheritance for the usual Java case                   |
| Compile-time polymorphism              | Runtime polymorphism                                           |

> Trap: **Changing only the return type does not create valid method overloading** in Java if the method name
and parameter list remain identical.

> **Overloading = same name + different parameters**.

> **Overriding = subclass provides a new implementation of an inherited method.**

</details>
<!---------------------------->

---

Q 10. Which type of method does not have an implementation in the base class and must overriden by derive class?
- [ ] A. Virtual Method
- [x] B. Abstract Class
- [ ] C. Sealed method
- [ ] D. Static method

<details>
 <summary> Solution </summary>

</details>
<!---------------------------->

---

Q 11. Which of the following best defines a class?
- [ ] A. An instance of an object
- [x] B. A blueprint for creating objects
- [ ] C. A varible holding data
- [ ] D. A function with a return type

<details>
 <summary> <b> Class and Object </b> </summary>

In OOP, a class is a blueprint or template used to create objects. <br/>
It defines the data (fields/attributes) and behavior (methods) that its objects can have.

Example:
```java
class Student {
    String name;  // Attribute

    void study() {  // Method
        System.out.println("Student is studying");
    }
}
```
- `Student` -> class name
- `name` -> field (data)
- `study()` -> method (behavior)
- `new Student()` -> creates an object of the class

> **Class = Blueprint; Object = Instance of a class.**

</details>
<!---------------------------->

---

Q 12. What is the purpose of data abstraction in OOP?
- [x] A. To hide the implementation details
- [ ] B. To expose all internal details
- [ ] C. To limit the scope of data
- [ ] D. To make methods public

<details>
 <summary> <b> Abstraction </b> </summary>

<br/>

The main purpose of data abstraction in OOP is **to hide implementation details and expose only the essential 
features that a user needs to interact with an object**.

Example:

Think of an ATM. <br/>
You enter your PIN and request a withdrawal.  <br/>
You don't need to know how the ATM internally verifies your account or communicates with the bank.

You use what the system does, without needing to know how it does it.

```java
abstract class Shape {
    abstract double calculateArea();
}

class Circle extends Shape {
    double radius = 5;

    @Override
    double calculateArea() {
        return Math.PI * radius * radius;
    }
}
```
The `Shape` class specifies what a shape must provide: `calculateArea()`. <br/>
The `Circle` class implements how to calculate the area.

**How abstraction works?**

<img width="402" height="361" alt="image" src="https://github.com/user-attachments/assets/05e5c730-8eeb-4c37-84d7-e352ebe971be" />


### Abstraction vs Encapsulation

| Abstraction	                   | Encapsulation                                    |
|--------------------------------|--------------------------------------------------|
| Hides implementation details	 | Bundles data and methods and controls access     |
| Focuses on what an object does | Focuses on protecting and managing internal state|
| Commonly uses abstract classes and interfaces in Java	| Commonly uses private fields and controlled public methods |

> **Abstraction = hide how; show what**.

### Points to remember

- **Interface**: defines a contract.
- **Abstract class**: can combine abstract methods with implemented methods.
- **Encapsulation**: bundles data and methods and controls access.
- **Inheritance**: enables a class to reuse or extend another class's functionality.

One useful nuance: modern Java interfaces can also contain default, static, and private methods with implementations,
 so an interface does not necessarily contain only abstract methods.

</details>
<!---------------------------->

---

Q 13. What is the primary function of **namespace** in OOP?
- [x] A. Group related classes and functions
- [ ] B. Manages object references
- [ ] C. Define instance variables
- [ ] D. Store data values

<details>
  <summary> Namespace </summary>

<br/>

The primary function of a namespace is to organize related identifiers 
and prevent naming conflicts between classes, functions, variables, and other names in a program.

Example: Suppose two departments in a school both have a class named Student. A namespace lets us distinguish between them.

<img width="617" height="200" alt="image" src="https://github.com/user-attachments/assets/330247b6-9d33-494c-9b10-664a731e0268" />

```cpp
#include <iostream>

namespace Science {
    class Student {};
}

namespace Commerce {
    class Student {};
}

int main() {
    Science::Student s1;
    Commerce::Student s2;
}
```
Both classes are named `Studen`t, but the namespaces distinguish them using the **scope-resolution operator `::`**.

### Important Points

- **Main purpose**: avoid naming conflicts.
- **Additional purpose**: organize related code into logical groups.
- **C++ syntax**: `namespace MyNamespace { }`
- **Scope-resolution operator: `::`**
- **Java distinction**: Java primarily uses packages to organize classes and avoid naming conflicts;
  it does not use C++-style namespace declarations.

  
</details>
<!------------------------>

---

Q 14. What is the main purpose of using namespace in programming?
- [ ] A. To provide data encapsulation
- [x] B. To organize code into logical group
- [ ] C. To define abstract class
- [ ] D. To handle exceptions

<details>
  <summary> Solution </summary>
  
</details>
<!------------------------>

---

Q 13. In OOP, what is the purpose of the `this` keyword?
- [ ] A. To create a new instance of a class
- [ ] B. To refer to the superclass
- [ ] C. To call a static mathod
- [x] D. To refer the current instnace of the class

<details>
  <summary> "this" keyword  </summary>

<br/>

### `this` Keyword in OOP (Java)

The `this` keyword refers to the current object - the object whose instance method or constructor is currently executing.

It is commonly used to distinguish an object's instance variables from local variables or parameters with the same name.

```java
class Student {
    int marks;

    Student(int marks) {
        this.marks = marks;
    }
}
-------------------------
create an object:
Student s = new Student(90);
System.out.println(s.marks);
--------------------------
Output:
90
```

### Important uses of `this`

| Use	                        | Example	            | Purpose                                     |
|-----------------------------|---------------------|---------------------------------------------|
| Refer to instance variable	| `this.name = name;`	| Distinguishes a field from a parameter      |
| Call an instance method	    | `this.display();`	  | Calls a method on the current object        |
| Call another constructor	  | `this(10);`	        | Calls another constructor in the same class |
| Pass the current object	    | `process(this);`	  | Supplies the current object as an argument  |

### Difference between `this` and `super`

| `this`	                                             | `super`                                                              |
|------------------------------------------------------|----------------------------------------------------------------------|
| Refers to the current object	                       | Refers to the superclass portion of the current object               |
| `this.display()` calls the current class's method	   | `super.display()` calls the superclass implementation, if accessible |
| `this()` calls another constructor in the same class | `super()` calls a superclass constructor                             |
  
</details>
<!------------------------>

---

Q 16. What is the purpose of `super` keyword in python?
- [x] A. It refers to the superclass of the current class
- [ ] B. It create a new instance of a class
- [ ] C. It handles exceptions
- [ ] D. It defines a new class

<details>
  <summary> super keyword </summary>

In Python, `super()` is used to access methods from a parent class, especially when a child class overrides a 
parent method or needs to call the parent class's constructor.

```py
class Animal:
    def __init__(self, name):
        self.name = name

class Dog(Animal):
    def __init__(self, name, breed):
        super().__init__(name)
        self.breed = breed

dog = Dog("Bruno", "Labrador")

print(dog.name)
print(dog.breed)
---------------------------
Output:
Bruno
Labrador
```
- `Animal` initializes `name`.
- `Dog` adds its own attribute, `breed`.
- `super().__init__(name)` calls the parent class's initializer so name is initialized without repeating the code.

**Calling a parent method**
```py
class Animal:
    def sound(self):
        print("Animal makes a sound")

class Dog(Animal):
    def sound(self):
        super().sound()
        print("Dog barks")

Dog().sound()
---------------
Output:
Animal makes a sound
Dog barks
```
The child calls the parent implementation and then adds its own behavior.


| Concept	     | Purpose                                                    |
|--------------|------------------------------------------------------------|
| `super()`	   | Access the next class in the method resolution order (MRO) | 
| `self`	     | Refers to the current instance                             |
| `__init__()` | Initializes a new instance                                 |

Important Python nuance: `super()` does not always mean "call the immediate parent directly." <br/>
It follows the class's method resolution order, which matters in multiple inheritance.


</details>
<!------------------------>

---

Q 17. What is the term for the ability of a class to provide different implementation of a method based on the input 
parameters?
- [x] A. Overloading
- [ ] B. Polymorphism
- [ ] C. Inheritance
- [ ] D. Encapsulation

<details>
  <summary> Overloading </summary>

Both Polymorphism and Overloading, but more precisely Overloading.
  
</details>
<!------------------------>

---

Q 18. What is the purpose of constructor in OOP?
- [ ] A. To destroy objects
- [ ] B. To create instances of abstract classes
- [x] C. To initialize object properties
- [ ] D. To define abstract methods

<details>
  <summary> <b> Constructor </b> </summary>

<br/>

The primary purpose of a constructor is **to initialize an object when it is created**. <br/>
It can assign initial values to the object's fields and perform setup needed for the object to be used.

```java
class Student {
    String name;
    int marks;

    Student(String n, int m) {
        name = n;
        marks = m;
    }
}

Student s = new Student("Aman", 90);

System.out.println(s.name);
System.out.println(s.marks);
---------------------------
Output:
Aman
90
```
When `new Student("Aman", 90)` creates the object, the constructor initializes its `name` and `marks` fields.

**How Constructor works**

<img width="307" height="360" alt="image" src="https://github.com/user-attachments/assets/7cf78a0e-ed71-4a75-951d-c755e17b36fd" />

### 3. Important points

- A constructor is invoked during object creation.
- In Java, its name must match the class name.
- A Java constructor has no return type, not even void.
- Constructors can be overloaded using different parameter lists.
- If no constructor is declared, Java provides a default constructor.
- Constructors are not inherited in Java.

Trap: A constructor initializes an object; a destructor (in languages such as C++) performs cleanup when 
an object's lifetime ends.

| Concept	            | Main purpose                        |
|---------------------|-------------------------------------|
| Constructor	        | Initialize an object                |
| Destructor	        | Perform cleanup                     |
| Inheritance	        | Reuse or extend class functionality | 
| Exception handling	| Handle exceptional situations       |

Important Java fact: A constructor has the same name as its class and has no return type—not even void.
  
</details>
<!------------------------>

---

Q 19. In OOP, what does the term **method signature** refers to?
- [ ] A. The name of the method
- [ ] B. The return type of the method
- [ ] C. The parameter of the method
- [x] D. The combination of method name and parameter types

<details>
  <summary> <b>method signature</b>  </summary>

<br/> 

In OOP, a **method signature identifies a method by its name and parameter list**.

For Java, a method signature consists of:
- Method name
- Parameter types (including their order)

It does not include the return type or access modifier.

Example:
```java
int add(int a, int b) {
    return a + b;
}

double add(double a, double b) {
    return a + b;
}
```
These methods have different signatures:
- `add(int, int)`
- `add(double, double)`

**What is not part of a Java method signature?**

| Element	                  | Part of signature? |
|---------------------------|--------------------|
| Method name	              | Yes                |
| Parameter types and order	| Yes                | 
| Return type	              | No                 |
| Access modifier (public, private)	| No         |
| Parameter variable names	| No                 |

For example, `int show(int x)` and `double show(int y)` have the same Java method signature: `show(int)`. <br/>
They cannot be overloaded solely by changing the return type.
  
</details>
<!------------------------>

---

Q 20. In OOP, what is method overloading?
- [ ] A. Creating multiple constructors
- [ ] B. Using multiple inheritance
- [x] C. Defining multiple methods with the same name but different parameters
- [ ] D. Inheriting multiple methods from a parent class

<details>
  <summary> method overloading </summary>

<br/> 

**Method overloading** means defining multiple methods in the same class with the same name but different parameter lists.
```java
class Calculator {
    int add(int a, int b) {
        return a + b;
    }

    int add(int a, int b, int c) {
        return a + b + c;
    }

    double add(double a, double b) {
        return a + b;
    }
}
```
All three methods are named add, but their parameter lists are different.
- `add(int, int)` -> takes two integers.
- `add(int, int, int)` -> takes three integers.
- `add(double, double)` -> takes two decimal numbers.
Java chooses which method to call based on the arguments supplied.

> **Method overloading = same name, different parameters**.

> **Method overriding = a subclass provides its own implementation of an inherited method**.

| Method overloading	                        | Method overriding |
|---------------------------------------------|-------------------|
| Same method name, different parameter lists	| Subclass redefines an inherited method |
| Usually occurs within the same class	      | Requires inheritance or another applicable overriding relationship |
| Compile-time polymorphism	                  | Runtime polymorphism in typical instance-method cases |
  
</details>
<!------------------------>

---

Q 21. What is the main advantage of using abstract class over interfaces?
- [ ] A. Abstract classes can have multiple inheritance, unlike interfaces
- [ ] B. Interfaces can have constructors, while abstract classes can't
- [x] C. Abstract classes can provide default implementation of methods
- [ ] D. Interfaces allow for private access modifiers, unlike abstract classes

<details>
  <summary> Abstract Class vs Interfaces </summary>

<br/>

Abstract classes can have concrete methods(define) as well as abstract methods(not defined).

In interfaces all methods must be abstract without body.

The main advantage of an abstract class over an interface in Java is that an abstract class can maintain 
shared state (instance variables) and provide common implementation for related subclasses.

**Example:** <br/>
Suppose we are developing software for different animals. <br/>
All animals have a name and can eat, but each animal makes a different sound.
```java
abstract class Animal {
    String name;                 // Shared state

    Animal(String name) {
        this.name = name;
    }

    void eat() {                 // Common implementation
        System.out.println("Eating...");
    }

    abstract void makeSound();   // Subclasses must implement
}
```
A subclass can reuse the shared code while implementing its own behaviour:
```java
class Dog extends Animal {
    Dog(String name) {
        super(name);
    }

    @Override
    void makeSound() {
        System.out.println("Bark");
    }
}
```
Here, `Animal` provides a shared field, a constructor, a concrete method (`eat()`), and an abstract method (`makeSound()`).

### Abstract class vs interface

| Feature	                          | Abstract class	                   | Interface                                 |
|-----------------------------------|------------------------------------|-------------------------------------------|
| Instance variables / object state	| Yes	                               | No ordinary per-instance state            |
| Constructor	                      | Yes	                               | No                                        |
| Concrete methods	                | Yes	                               | Yes, including default methods            |
| Abstract methods	                | Yes	                               | Yes                                       |
| Inheritance	                      | A class can extend only one class	 | A class can implement multiple interfaces |

Important exam nuance: Modern Java interfaces can contain `default`, `static`, and `private methods`, <br/>
so it is incorrect to say that interfaces can contain only abstract methods.
  
</details>
<!------------------------>

---

Q 22. Which principle esures that only essential information is visible to the outside world?
- [ ] A. Polymorphism
- [ ] B. Information Hiding
- [ ] C. Encapsulation
- [x] D. Abstraction

<details>
  <summary> <b> Abstraction </b> </summary>

<br/>

**Abstraction** is an OOP principle that exposes only essential features to the outside world 
while hiding unnecessary implementation details.

For example, when you drive a car, you use the steering wheel, accelerator, and
brakes without needing to understand the internal workings of the engine.

> **Abstraction = what is necessary to know;**

> **encapsulation = how data and access are organized and protected.**

| Principle	    | Main purpose                                                |
|---------------|-------------------------------------------------------------|
| Abstraction	  | Hides implementation details and exposes essential features |
| Encapsulation |	Bundles data and methods together and controls access       |
| Inheritance	  | Reuses and extends an existing class                        |
| Polymorphism	| Allows the same interface or method name to exhibit different behaviours |
  
</details>
<!------------------------>

---

Q 23. What is the term for creating a new class based on an existing class?
- [ ] A. Overriding 
- [ ] B. Implementing
- [x] C. Inheriting
- [ ] D. Overloading

<details>
  <summary> <b> Inheritance </b>  </summary>

<br/>

**Inheritance** is an Object-Oriented Programming (OOP) principle in which a new class is created based on an existing class,
allowing it to reuse and extend the existing class's properties and methods.

```java
class Animal {             // Parent class
    void eat() {
        System.out.println("Eating");
    }
}

class Dog extends Animal { // Child class
    void bark() {
        System.out.println("Barking");
    }
}
```
Here, `Dog` inherits the `eat()` method from `Animal` and adds its own `bark()` method. <br/>
In Java, the keyword `extends` is used for class inheritance.

<img width="266" height="290" alt="image" src="https://github.com/user-attachments/assets/9bf54493-b86f-42e0-885a-7ae4aada568c" />

### Five types of inheritance

**1. Single inheritance** <br/>
One child class inherits from one parent class. <br/>
Example: `Dog` inherits from `Animal`. <br/>
`A -> B`

**2. Multilevel inheritance** <br/>
A class inherits from a class that itself inherits from another class. <br/>
Example: Animal → Mammal → Dog. 
`A -> B -> C`

**3. Hierarchical inheritance** <br/>
Multiple child classes inherit from the same parent. <br/>
Example: Dog and Cat inherit from Animal.
`A -> B and A -> C`

**4. Multiple inheritance** <br/>
One child class inherits from two or more parent classes. <br/>
Example: C inherits from A and B.
`A and B -> C`

**5. Hybrid inheritance** <br/>
A combination of two or more inheritance types. <br/>
Example: combining hierarchical and multiple inheritance.

**Java supports these inheritance patterns through classes:**
| Type	       | Supported directly through Java classes? |
| Single	     | Yes                                      |
| Multilevel	 | Yes                                      |
| Hierarchical | Yes                                      |
| Multiple	   | No - a class cannot extend two classes   |
| Hybrid	     | Not fully through classes alone          |

Java can achieve multiple-type inheritance of behaviour/contracts through **interfaces**. <br/>
A class can implement multiple interfaces.

**Quick recap trick**
- Single: one parent, one child.
- Multilevel: a chain.
- Hierarchical: one parent, many children.
- Multiple: many parents, one child.
- Hybrid: a combination.
  
</details>
<!------------------------>

---

Q 24. Which concept allows a subclass to provide a specific implementation of a method that is already in the superclass?
- [ ] A. Overloading
- [ ] B. Inheritance
- [ ] C. Polymorphism
- [x] D. Overriding

<details>
  <summary> <b>Method Overriding</b> </summary>

<br/>

**Method overriding** occurs when a subclass provides its own specific implementation of a method already defined in its superclass.

```java

class Animal {
    void sound() {
        System.out.println("Animal makes a sound");
    }
}

class Dog extends Animal {
    @Override
    void sound() {
        System.out.println("Dog barks");
    }
}
```
Here, `Dog` overrides the `sound()` method inherited from `Animal`.
- Superclass: `Animal`
- Subclass: `Dog`
- Overridden method: `sound()`

  
</details>
<!------------------------>

---

Q 25. Which concept allows a class to inherit properties and behaviours from multiple classes?
- [ ] A. Encapsulation
- [ ] B. Inheritance
- [ ] C. Polymorphism
- [x] D. Multiple Inheritance

<details>
  <summary> <b> Multiple Inheritance </b> </summary>

**Multiple inheritance** is an OOP concept in which a single child class inherits properties and behaviours from two or more parent classes.

Conceptually, a class `SmartPhone` might inherit features from both `Phone` and `Camera`

<img width="706" height="247" alt="image" src="https://github.com/user-attachments/assets/b91c43cd-6e68-41e0-92a5-d83b3863eedd" />


- Java doesn't support Multiple Inheritance, bcuz of diamond problem occurs which causes ambiguity.

In Java, a class cannot extend multiple classes, but it can implement multiple interfaces.
```java
class SmartPhone implements Phone, Camera {
    // Implement interface methods
}
```
Here, `Phone` and `Camera` must be interfaces for this Java declaration to be valid.
  
</details>
<!------------------------>

---

Q 26. In OOP, which term refers to a mechnism by which a class can inherit properties and behaviors from another class?
- [ ] A. Polymorphism
- [ ] B. Abstraction
- [ ] C. Encapsulation
- [x] D. Inheritance

<details>
  <summary> Inheritance </summary>

<br/>

Inheritance is an OOP mechanism through which a class (the subclass) 
acquires properties and behaviours from another class (the superclass).

```java
class Animal {
    void eat() {
        System.out.println("Eating");
    }
}

class Dog extends Animal {
    void bark() {
        System.out.println("Barking");
    }
}
```

- Inheritance: acquiring features from another class.

- Polymorphism: one interface, different behaviours.

- Encapsulation: bundling data and methods while controlling access.

- Abstraction: exposing essential features and hiding implementation details.
  
</details>
<!------------------------>

---

Q 27. Which method is automatically called when an object is created:
- [x] A. Constructor
- [ ] B. Destructor
- [ ] C. Main method
- [ ] D. Inherited method

<details>
  <summary> <b> Constructor </b> </summary>

<br/>

A **constructor** is a special member of a class that is called when an object is created. <br/>
Its main purpose is to initialize the object's state.

**Important characteristics of a Java constructor**
- Its name must be the same as the class name.
- It has no return type, not even void.
- It can accept parameters.
- Constructors can be overloaded.
- Constructors are not inherited by subclasses.
- If no constructor is declared, Java generally provides a default no-argument constructor.
- Constructors are called during object creation, but a constructor is not itself a method.

**Types of constructors**
| Type	                        | Meaning                              |
|-------------------------------|--------------------------------------|
| **No-argument constructor**	  | Takes no arguments                   |
| **Parameterized constructor** | Takes arguments to initialize fields |
| **Copy constructor** | A constructor pattern that initializes an object using another object; Java does not provide one automatically |
  
</details>
<!------------------------>

---

Q 28. What is an abstract class in OOP?
- [ ] A. A class with no methods
- [x] B. A class that can't be instatiated
- [ ] C. A class that can only have private members
- [ ] D. A class that can't have methods with parameters

<details>
  <summary> Solution </summary>

In Java, an abstract class cannot be instantiated directly because it may contain abstract methods that have no implementation yet.

```java
abstract class Animal {
    abstract void makeSound();
}
---------------------
Animal a = new Animal(); // Compilation error
```
The method `makeSound()` has no method body. Java doesn't know what specific sound an animal should make.

```java
abstract class Animal {
    abstract void makeSound();
}

class Dog extends Animal {
    @Override
    void makeSound() {
        System.out.println("Bark");
    }
}

Dog d = new Dog(); // Valid
d.makeSound();
-----------------------
Bark
```

An abstract class can have constructors, fields, and fully implemented methods. <br/>
It cannot be instantiated directly, but its constructor executes when a concrete subclass object is created.

Also, an abstract class does not necessarily need to contain an abstract method.  <br/>
A class declared abstract still cannot be instantiated directly, even if all its methods have implementations.

> **Abstract class = incomplete or intentionally restricted blueprint;** <br/>
> **concrete subclass = usable class from which objects can be created**.

  
</details>
<!------------------------>

---

Q 29. What is the main focus of procedural programming?
- [ ] A. Data abstraction
- [ ] B. Object creation
- [ ] C. Code resuability
- [x] D. Sequential execution

<details>
  <summary> Sequential execution </summary>

<br/>

**Procedural programming** is organizing a program into procedures or functions that perform a sequence of instructions to 
solve a problem.

Procedural programming follows a step-by-step approach: the program specifies how a task should be performed.

```c
#include <stdio.h>

void greet() {
    printf("Hello!");
}

int main() {
    greet();
    return 0;
}
```
Here, the program uses functions (`main()` and `greet()`) to organize its instructions.

**Key characteristics**
- **Functions/procedures**: Divide a program into smaller tasks.
- **Step-by-step execution**: Instructions generally execute in a defined sequence.
- **Control structures**: Use sequence, selection (`if/else`), and iteration (`for, while`).
- **Data and functions**: Data is often passed to functions or accessed through variables.

| Procedural programming	            | Object-oriented programming              |
|-------------------------------------|------------------------------------------|
| Focuses on procedures and functions	| Focuses on objects and classes           |
| Emphasizes steps to solve a problem	| Combines data and behaviour into objects |
| Example: C	                        | Examples: Java, C++                      |

  
</details>
<!------------------------>

---

Q 30. What is the term for a variable that references an instance of a class?
- [ ] A. Property
- [ ] B. Method
- [x] C. Object
- [ ] D. Constructor

<details>
  <summary> <b> Object </b>  </summary>

### What is an Object in OOP?

- An object is an instance of a class. 
- It represents a real-world entity and contains data (properties) and behaviour (methods).

<img width="862" height="352" alt="image" src="https://github.com/user-attachments/assets/d99dbfbc-14c3-46f2-9ec6-8b88ac8a3030" />

```java
class Student {
    String name;       // Property
    void study() {     // Behaviour
        System.out.println("Studying");
    }
}

Student s1 = new Student();
s1.name = "Aman";

s1.study();
```
- `Student` -> class
- `s1` -> reference variable
- `new Student()` -> creates an object
- `name` -> property (data)
- `study()` -> method (behaviour)

> **Class = Blueprint; Object = Instance of the class.**
  
</details>
<!------------------------>

---

Q 31. Which keyword is used to define an abstract method within an abstract class?
- [x] A. abstract
- [ ] B. virtual
- [ ] C. override
- [ ] D. implement

<details>
  <summary> abstract </summary>

  
We use `abstract` keyword in java, in C++ we use `virtual` keyword.


The `abstract` keyword is used to declare an abstract method. <br/>
An abstract method has no method body and must be implemented by a concrete subclass unless that subclass is also abstract.

```java
abstract class Animal {
    abstract void makeSound();
}
```
Here, `abstract` declares `makeSound()` without a body.

A concrete subclass provides the implementation:
```java
class Dog extends Animal {
    @Override
    void makeSound() {
        System.out.println("Bark");
    }
}
```

- `abstract` -> declares an abstract class or method.
- `extends` -> establishes class inheritance.
- `implements` -> implements an interface.
- `final` -> prevents a method from being overridden.
  
</details>
<!------------------------>

<details>
  <summary> <b> Virtual keyword </b> </summary>

### What is the `virtual` keyword?

The virtual keyword is used in C++, not Java, to enable a member function to be overridden and called according to the object's actual type at runtime.

This supports runtime polymorphism.

```cpp
class Animal {
public:
    virtual void sound() {
        cout << "Animal sound";
    }
};

class Dog : public Animal {
public:
    void sound() override {
        cout << "Bark";
    }
};

-------------------------
Animal* a = new Dog();
a->sound();
------------------------
Output: Bark
```
Because `sound()` is virtual, C++ calls the `Dog` implementation even though the pointer's declared type is `Animal*`.

</details>

---

Q 32. Which keyword is used to create an instance of a class in most programming languages?
- [ ] A. alloc
- [x] B. new
- [ ] C. create
- [ ] D. instance

<details>
  <summary> new </summary>

```java
Student s1 = new Student();
```
- `Student` -> class name
- `s1` -> reference variable
- `new` -> creates an object (instance)
- `Student()` -> calls the constructor

> **Class = blueprint; object = instance; new = commonly used to create an instance.**
  
</details>
<!------------------------>

---

Q 33. Which term is used to describe the ability of different classes to be treated as objects of the same parent class?
- [ ] A. Overloading
- [x] B. Polymorphism
- [ ] C. Abstraction
- [ ] D. Encapsulation

<details>
  <summary> Overriding which comes under Polymorphism </summary>

<br/>

Polymorphism means "many forms." <br/>
It allows objects of different classes to be treated through a common parent-class type while providing their own specific behaviour.

```java
class Animal {
    void sound() {
        System.out.println("Animal sound");
    }
}

class Dog extends Animal {
    @Override
    void sound() {
        System.out.println("Bark");
    }
}

class Cat extends Animal {
    @Override
    void sound() {
        System.out.println("Meow");
    }
}
----------------------------

// Both objects can be referenced using the parent class Animal

Animal a1 = new Dog();
Animal a2 = new Cat();

a1.sound();  // Bark
a2.sound();  // Meow
```
The same parent-class reference type, `Animal`, can refer to different child-class objects and invoke their specific 
implementations.
  
</details>
<!------------------------>

---

Q 34. Which keyword is used to indicate that a class or method can be accessed within the same package?
- [ ] A. private
- [ ] B. protected
- [x] C. package-private
- [ ] D. public

<details>
  <summary> package-private </summary>

<br/>

default access (package-private) in Java. There is no keyword used for it.

When you declare a class or method without an access modifier, 
it can be accessed by other code within the same package, subject to the usual class and member access rules.

```java
class Student {          // Package-private class
    void study() {       // Package-private method
        System.out.println("Studying");
    }
}
```
Here, neither `Student` nor `study()` has an access modifier.

| Access modifier	| Accessibility                                                              |
|-----------------|----------------------------------------------------------------------------|
| `private`	      | Same class                                                                 |
| `(no modifier)`	| Same package                                                               |
| `protected`	    | Same package, plus subclasses in other packages under Java's access rules  |
| `public`	      | Accessible wherever the containing type and other access conditions permit |

  
</details>
<!------------------------>

---

Q 35. Which keyword is used to indicate that a class cannot be inherited by other classes?
- [ ] A. sealed
- [x] B. final
- [ ] C. private
- [ ] D. static

<details>
  <summary> final </summary>

The `final` keyword prevents a class from being extended (inherited) by another class.

```java
final class Animal {
    void sound() {
        System.out.println("Animal sound");
    }
}

// Compilation error:
class Dog extends Animal {
}
```
Because `Animal` is declared `final`, Java does not allow `Dog` to inherit from it.

| Use of `final`	| Meaning                                   |
|-----------------|-------------------------------------------|
| `final` variable| Cannot be reassigned after initialization |
| `final` method	| Cannot be overridden                      |
| `final` class	  | Cannot be extended                        |

### 1. `sealed`

Purpose: Restricts which classes can inherit from a class or implement an interface.
```java
public sealed class Animal permits Dog, Cat { }

final class Dog extends Animal { }
final class Cat extends Animal { }
```
Only the permitted classes (`Dog` and `Cat`) can directly extend Animal. 
In Java, permitted subclasses must declare how they allow further inheritance, using final, sealed, or non-sealed.

> **`sealed` = restricts inheritance to specified subclasses.**

### 2. `final`

Purpose: Prevents reassignment, overriding, or inheritance, depending on where it is used.

```java
final int age = 20;  // Cannot be reassigned

class Animal {
    final void eat() { }  // Cannot be overridden
}

final class Dog { }  // Cannot be extended
```

> **`final` class cannot be inherited; `final` method cannot be overridden.**

### 3. `private`

Purpose: Restricts access to within the enclosing class.
```java
class Student {
    private int marks = 90;

    private void displayMarks() {
        System.out.println(marks);
    }
}
```
Code outside `Student` cannot directly access `marks` or call `displayMarks()`.

> **`private` = restricted access.**

### 4. `static`

Purpose: Makes a member belong to the class rather than to individual instances.

```java
class Student {
    static String school = "ABC School";

    static void showSchool() {
        System.out.println(school);
    }
}

--------------------------------------
Student.showSchool();
System.out.println(Student.school);
```
We can access these members through the class:

> **`static` = class-level member, shared rather than separately belonging to each object.**

### Keywords

| Keyword	   | Main purpose                                      |
|------------|---------------------------------------------------|
|  `sealed`	 | Restricts which classes can inherit               |
|  `final`	 | Prevents reassignment, overriding, or inheritance |
|  `private` | Restricts access to the enclosing class           |
|  `static`	 | Associates a member with the class                |
  
</details>
<!------------------------>

---

Q 36. A class allows access to its data only through specified member functions. Which OOP priciple is primarily demonstrated?
- [ ] A. Inheritance
- [x] B. Encapsulation
- [ ] C. Polymorphism
- [ ] D. Generalization

<details>
  <summary> <b> Encapsulation </b> </summary>

<br/>

**Encapsulation** is the OOP principle of bundling data and methods into a class and controlling access to that data through 
specified member functions.

```java
class BankAccount {
    private double balance = 1000;

    public double getBalance() {
        return balance;
    }

    public void deposit(double amount) {
        if (amount > 0) {
            balance += amount;
        }
    }
}
```
- `private balance` prevents direct access from outside the class.
- `getBalance()` allows controlled access to the balance.
- `deposit()` allows changes through a defined method.
The data is protected from unrestricted access, and the class controls how it is read or modified.

| Principle	        | Main purpose                                                             |
|-------------------|--------------------------------------------------------------------------|
| **Encapsulation**	| Bundles data and methods; controls access                                |
| **Abstraction**	  | Hides implementation details and exposes essential features              |
| **Inheritance**	  | Allows a class to derive from another class                              |
| **Polymorphism**	| Allows different types to respond differently through a common interface |


  
</details>
<!------------------------>

---

Q 37. Which statement is true about abstract class is generally correct?
- [ ] A. It can't contain methods
- [ ] B. It must contain only static members
- [ ] C. It can never have constructors
- [x] D. It can't normally be instatiated directly

<details>
  <summary>  </summary>
  
</details>
<!------------------------>

---

Q 38. Which inheritance type allows a derived class to inherit from two more base class?
- [ ] A. Single Inheritance
- [ ] B. Multi-level inheritance
- [ ] C. Hierachical inheritance
- [x] D. Multiple Inheritance

<details>
  <summary> <b> Multiple Inheritance </b> </summary>

<br/>

Multiple inheritance occurs when a single derived class inherits from two or more base classes.

<img width="405" height="207" alt="image" src="https://github.com/user-attachments/assets/92e4bbda-2680-4ff0-85ae-9d13a2d473cb" />

```cpp
class A {
public:
    void showA() {}
};

class B {
public:
    void showB() {}
};

class C : public A, public B {
};
```
Class `C` inherits from both `A` and `B`.

Java does not support multiple inheritance through classes, **but a class can implement multiple interfaces**.
```java
class C implements A, B {
}
```
Here, `A` and `B` must be interfaces.

| Inheritance type | Structure                        |
|------------------|----------------------------------|
| Single	         | One base -> one derived          |
| Multiple	       | Two or more bases -> one derived |
| Multilevel	     | A -> B -> C                      |
| Hierarchical	   | One base -> multiple derived     |
| Hybrid	         | Combination of inheritance types |


</details>
<!------------------------>

---

Q 39. In C++, which access specifier allows class members to be accessed by derived classes while restricting ordinary 
external access?
- [ ] A. private
- [x] B. protected
- [ ] C. public
- [ ] D. static

<details>
  <summary> protected  </summary>

<br/>

| Modifier    | Type	              | Meaning                                      |
|-------------|---------------------|----------------------------------------------|
| `private`	  | Access modifier	    | Accessible only within the enclosing class   |
| `protected` |	Access modifier	    | Accessible within the same package and, under Java's inheritance access rules, in subclasses in other packages|
| `public`    | Access modifier	    | Broadest access, subject to other access rules|
| `static`    | Non-access modifier	| Makes a member belong to the class rather than individual objects |

```java
class Student {
    private int marks = 90;
    protected String name = "Aman";
    public void display() { }
    static int count = 0;
}
```
- `marks` is private.
- `name` is protected.
- `display()` is public.
- `count` is `static`, meaning it belongs to the class.
  
</details>
<!------------------------>

---

Q 40. Which statement about a pure virtual function in C++ is correct?
- [ ] A. It must be a constructor
- [ ] B. It can't be overriden
- [x] C. It is declared using `= 0`
- [ ] D. It must be declared private

`virtual void display() = 0` -> Pure Virtual Function

<details>
  <summary> <b> Pure Virtual Function </b> </summary>

### What is a Pure Virtual Function in C++?

A pure virtual function is a virtual function declared in a base class with `= 0`.

It is used to make the base class abstract and require derived classes to provide an implementation if they are to be concrete.

Syntax:
```cpp
virtual void display() = 0;
```

Example
```cpp
#include <iostream>
using namespace std;

class Animal {
public:
    virtual void sound() = 0;  // Pure virtual function
};

class Dog : public Animal {
public:
    void sound() override {
        cout << "Bark";
    }
};

int main() {
    Dog d;
    d.sound();  // Output: Bark
}
```
- `virtual `enables runtime polymorphism.
- `= 0` declares the function as pure virtual.
- `Animal` becomes an `abstract` class, so you cannot instantiate it directly.
- `Dog` implements `sound()`, so it can be instantiated.

A derived class that does not implement all inherited pure virtual functions remains abstract.

| Term	                | Meaning                                            |
|-----------------------|----------------------------------------------------|
| Virtual function      | Supports runtime polymorphism                      |
| Pure virtual function	| Declared with `= 0`; makes the base class abstract |
| Abstract class	      | Cannot be instantiated directly                    |

  
</details>
<!------------------------>

---

Q 41. Which keyword prevent a java class from being subclass?
- [ ] A. static
- [x] B. final
- [ ] C. super
- [ ] D. abstract

<details>
  <summary> final </summary>
  
</details>
<!------------------------>

---

Q 42. Which statement about java constructor is correct?
- [x] A. They have the same name as the class
- [ ] B. They must return void
- [ ] C. They are inherited by subclasses
- [ ] D. They must always be declared static

<details>
  <summary> Solution </summary>
  
</details>
<!------------------------>

---

Q 43. Which java features allows a class to specify a contract that implementing classes must fulfill?
- [ ] A. package
- [ ] B. constructor
- [x] C. interface
- [ ] D. garbage collector

<details>
  <summary> package, constructor, inteface, garbage collector </summary>

<br/>

### 1. Package

Definition: A package in Java is a mechanism for grouping related classes, interfaces, and subpackages. <br/>
It helps organize code, avoid naming conflicts, and control access.

```java
package school;

class Student {
    void study() {
        System.out.println("Studying");
    }
}
```
Here, `school` is the package name.
- `java.util` is a built-in Java package.
- `import java.util.Scanner`; imports the Scanner class.

> **Package = organizes related Java classes and interfaces**

### 2. Constructor

Definition: A constructor is a special member of a class that is called when an object is created to initialize the object.

```java
class Student {
    String name;

    Student(String n) {
        name = n;
    }
}

Student s = new Student("Aman");
```
Here, `Student(String n)` is a constructor that initializes the student's name.

Key points:
- Has the same name as the class.
- Has no return type, not even void.
- Can be overloaded.
- Is not inherited.
- If no constructor is declared, Java provides a default no-argument constructor.

> **Constructor = initializes an object when it is created.**


### 3. Interface

Definition: An interface in Java defines a contract that implementing classes agree to follow. <br/>
It can declare abstract methods and can also contain  `default`, `static`, and `private` methods.

```java
interface Animal {
    void sound();
}

class Dog implements Animal {
    public void sound() {
        System.out.println("Bark");
    }
}
```
Here:
- `Animal` is an interface.
- `Dog` implements the interface.
- `Dog` provides the implementation of `sound()`.

> A class uses implements to implement an interface. <br/>
> A class can implement multiple interfaces.


### 4. Garbage Collector

Definition: The **garbage collector** (GC) is a part of the Java runtime that automatically reclaims memory used by objects 
that are no longer reachable by the program.


```java
Student s = new Student("Aman");
s = null;
```
If no other reachable reference points to that `Student` object, it becomes eligible for garbage collection.

The JVM decides when to collect it; setting `s = null` does not immediately destroy the object.


### Summary

| Term	            | Main purpose                                |
|-------------------|---------------------------------------------|
| Package	          | Organizes related classes and interfaces    |
| Constructor	      | Initializes objects                         |
| Interface	        | Defines a contract for implementing classes |
| Garbage collector	| Reclaims memory from unreachable objects    |
  
</details>
<!------------------------>

---

Q 44. Which mechanism automatically reclaims memory occupied by unreachable object in java?
- [ ] A. constructor chaining
- [ ] B. method overloading
- [ ] C. exeption handling
- [x] D. garbage collection

<details>
  <summary> <b> Garbage collection </b> </summary>

<br/>

Garbage Collector

Definition: The **garbage collector** (GC) is a part of the Java runtime that automatically reclaims memory used by objects 
that are no longer reachable by the program.


```java
Student s = new Student("Aman");
s = null;
```
If no other reachable reference points to that `Student` object, it becomes eligible for garbage collection.

The JVM decides when to collect it; setting `s = null` does not immediately destroy the object.

  
</details>
<!------------------------>

---

Q 45. In a python instance method, what does `self` keyword normally refers to?
- [ ] A. The parent class
- [x] B. The currect instance
- [ ] C. The python interpreter
- [ ] D. the class constructor

<details>
  <summary> <b> self </b> </summary>

<br/>

`self` refers to the current instance (object) of the class

In Python, `self` is the conventional name for the first parameter of an instance method.

It lets the method access that object's attributes and other methods.

```py
class Student:
    def __init__(self, name):
        self.name = name

    def introduce(self):
        print("My name is", self.name)

s1 = Student("Aman")
s1.introduce()
#########################
Output:
My name is Aman
```
Here:
- `s1` is the object.
- `self` refers to that object when `introduce()` is called.
- `self.name` accesses the name attribute belonging to that object.

Important points
- `self` is not a reserved Python keyword; it is a strong naming convention.
- Python passes the instance automatically when you call `s1.introduce()`.
- Different objects have their own instance attributes.
  
</details>
<!------------------------>

---

Q 46. Which python method is commonly used to customized the string represenetation returned by `str(obj)`?
- [x] A. `__str__()`
- [ ] B. `__init__()`
- [ ] C. `__delattr__()`
- [ ] D. `__newclass__()`

<details>
  <summary> Solution </summary>

<br/> 

`__str__()` -> string

`__init__()` -> Constructor

`__delattr__()` -> Deleting attribute

`__newclass__()` -> new class creation

</details>
<!------------------------>

---

Q 47. Which statement about python inheritance is correct?
- [ ] A. python supports only single inheritance
- [x] B. python supports multiple inheritance
- [ ] C. python prohibits method overriding
- [ ] D. python classs can't inherit methods

<details>
  <summary> Inheritance in Python </summary>

<br/>

Inheritance is an OOP feature in which a child class acquires attributes and methods from a parent class. <br/>
It promotes code reuse.

```py
class Animal:                 # Parent class
    def eat(self):
        print("Animal is eating")

class Dog(Animal):             # Child class
    def bark(self):
        print("Dog is barking")

d = Dog()
d.eat()    # Inherited method
d.bark()   # Dog's own method
```

### Types of inheritance in Python

| Type	       | Meaning	                                | Example                  |
|--------------|------------------------------------------|--------------------------|
| Single	     | One parent → one child	                  | Dog(Animal)              |
| Multiple	   | One child inherits from multiple parents	| class C(A, B)            |
| Multilevel	 | Inheritance across multiple levels	      | C(B), B(A)               |
| Hierarchical | Multiple children share one parent	      | Dog(Animal), Cat(Animal) |
| Hybrid	     | Combination of inheritance types	        | Multiple + multilevel    |

Unlike Java classes, **Python supports multiple inheritance**.

### 3. Method overriding

A child class can provide its own implementation of a method inherited from the parent.
```py
class Animal:
    def sound(self):
        print("Animal sound")

class Dog(Animal):
    def sound(self):
        print("Bark")

d = Dog()
d.sound()  # Bark
```
Here, `Dog` overrides the `sound()` method.

> **Same method name with a child-specific implementation -> method overriding**

###  4. The `super()` function

`super()` lets a child class access parent-class methods, commonly including the parent constructor.
```py
class Animal:
    def __init__(self):
        print("Animal created")

class Dog(Animal):
    def __init__(self):
        super().__init__()
        print("Dog created")

d = Dog()
------------------
Output:
Animal created
Dog created
```

  
</details>
<!------------------------>

---

Q 48. Which statement about python `@staticmethod is correct?
- [ ] A. It automatically receive self
- [ ] B. It must modify class attributes
- [x] C. It receive neither `self` nor `cls` automatically
- [ ] D. It can only be called inside constructor


<details>
  <summary> @staticmethod in python </summary>

### What is `@staticmethod` in Python?

@staticmethod is a decorator that defines a method inside a class that **does not automatically receive `self` or `cls` as its 
first argument**.

It is useful when a function logically belongs to a class but does not need to access a particular object’s data or 
the class itself.

```py
class Calculator:
    @staticmethod
    def add(a, b):
        return a + b

print(Calculator.add(10, 20))
---------------------
Output:
30
```
Here:
- `@staticmethod` marks `add()` as a static method.
- `a` and `b` are ordinary parameters.
- The method does not need an object to access instance data.
- You can call it directly through the class: `Calculator.add(10, 20)`.

### 2. Difference between instance, class, and static methods

| Feature	                      | Instance method	  | Class method	  | Static method                 |
|-------------------------------|-------------------|-----------------|-------------------------------|
| Decorator	                    | None required	    | `@classmethod`	| @staticmethod                 |
| First parameter by convention	| `self`	          | `cls`	          | None automatically            |
| Access instance data 	        | Yes	              | Not directly	  | Not automatically             |
| Access class data	            | Yes	              | Yes	            | Only if explicitly referenced |


> **`self` -> current object**

> **`cls` -> current class**

> **`@staticmethod` -> no automatic `self` or `cls`**
  
</details>
<!------------------------>

---

Q 49. Which java keyword **explicitly raises an exception**?
- [ ] A. throws
- [ ] B. catch
- [x] C. throw
- [ ] D. finally

Which keyword **declares that a Java method may pass an exception** to its caller?
- [ ] A. throw
- [x] B. throws
- [ ] C. catch
- [ ] D. finally

<details>
  <summary> throws </summary>

<br/>

In Java, the `throw` keyword explicitly throws an exception from a particular point in the program.
```java
public class Main {
    public static void main(String[] args) {
        int age = 15;

        if (age < 18) {
            throw new IllegalArgumentException("Age must be 18 or above");
        }
    }
}
```
Here, `throw` explicitly raises an `IllegalArgumentException`.


| Keyword	  | Purpose                                             |
|-----------|-----------------------------------------------------|
| `throw`	  | Explicitly throws an exception                      |
| `throws`	| Declares exceptions a method may pass to its caller |
| `try`	    | Encloses code where exceptions may occur            |
| `catch` 	| Handles an exception                                |

> **throw = raise an exception.**

> **throws = declare possible exceptions.**
```java
throw new IOException();        // Throws an exception
void read() throws IOException  // Declares an exception
```
  
</details>
<!------------------------>

---

Q 50. Which block is generally used for cleanup after `try` block?
- [ ] A. finally
- [ ] B. throw
- [ ] C. throws
- [x] D. catch

<details>
  <summary> <b> finally </b> </summary>
  
</details>
<!------------------------>

---

Q 51. Which exception is unchecked(runtime) in java?
- [ ] A. IOException
- [x] B. ArithmeticException/NullPointerException
- [ ] C. SQLException
- [ ] D. ClassNotFoundException

Common unchecked exceptions
- `NullPointerException`
- `ArithmeticException`
- `ArrayIndexOutOfBoundsException`
- `NumberFormatException`
- `IllegalArgumentException`

| Checked	                | Unchecked                        |
|-------------------------|----------------------------------|
| `IOException`           |	`NullPointerException`           |
| `SQLException`          |	`ArithmeticException`            |
| `FileNotFoundException` |	`ArrayIndexOutOfBoundsException` |

<details>
  <summary> <b> IOException </b> </summary>

<br/>

Unchecked exceptions occur at runtime, and Java does not require you to `catch` them or declare them with `throws`

```java
String name = null;
System.out.println(name.length());
```
This causes a `NullPointerException` because `name` refers to no string object.

Common unchecked exceptions
- `NullPointerException`
- `ArithmeticException`
- `ArrayIndexOutOfBoundsException`
- `NumberFormatException`
- `IllegalArgumentException`

  
</details>
<!------------------------>

---

Q 52. In java, what is the primary purpose of `new`
- [x] A. To create an object
- [ ] B. To inherit a class
- [ ] C. To destroy an object
- [ ] D. To handle exceptions

<details>
  <summary>  To create an object </summary>
  
</details>
<!------------------------>

---

Q 53. In java, which keyword is used for class inheritance?
- [ ] A. implements
- [ ] B. inherits
- [x] C. extends
- [ ] D. super

<details>
  <summary> extends </summary>

<br/>

Interface to class -> `implements`

class to class -> `extends`

Interface to Interface -> `extends`

| Situation	                              | Keyword     |
|-----------------------------------------|-------------|
| Interface inherits another interface    | `extends`   |
| Class inherits another class	          | `extends`   |
| Class implements an interface	          | `implements`|
| Interface inherits multiple interfaces	| `extends`   |

  
</details>
<!------------------------>

---

Q 54. In java, an interface uses which keyword to inherit another interface?
- [x] A. extends
- [ ] B. implements
- [ ] C. super
- [ ] D. instanceof

<details>
  <summary> implements </summary>

<br/>

| Situation	                              | Keyword     |
|-----------------------------------------|-------------|
| Interface inherits another interface    | `extends`   |
| Class inherits another class	          | `extends`   |
| Class implements an interface	          | `implements`|
| Interface inherits multiple interfaces	| `extends`   |

In Java, an interface uses the extends keyword to inherit another interface.
```java
interface Animal {
    void eat();
}

interface Pet extends Animal {
    void play();
}
```


multiple interface inheritance:
```java
interface A { }
interface B { }

interface C extends A, B { }
```
  
</details>
<!------------------------>

---

Q 55. What is the purpose od sealed class in java?
- [ ] A. to prevent object creation
- [ ] B. to make all methods static
- [ ] C. to prohibits all inheritance
- [x] D. to restrict permitted subclasses

<details>
  <summary> to restrict permitted subclasses </summary>
  
</details>
<!------------------------>

---

Q 56. What is thr primary purpose of a virtual function in C++?
- [x] A. Runtime polymorphism
- [ ] B. Memory allocation
- [ ] C. Exception Handling
- [ ] D. Data Conversion

<details>
  <summary> Runtime polymorphism </summary>

<br/>

A virtual function allows a derived class to override a base-class function so that, when called through a base-class 
pointer or reference, the appropriate implementation is selected at runtime according to the actual object type.

```cpp
#include <iostream>
using namespace std;

class Animal {
public:
    virtual void sound() {
        cout << "Animal sound";
    }
};

class Dog : public Animal {
public:
    void sound() override {
        cout << "Bark";
    }
};

int main() {
    Animal* a = new Dog();
    a->sound();  // Bark
    delete a;
}
```


- `virtual` -> supports runtime polymorphism.
- `override` -> indicates that a derived-class method overrides a virtual method.
- `= 0` -> declares a pure virtual function.
  
</details>
<!------------------------>

---

Q 57. In java, a static data member belongs to:
- [ ] A. every method separately
- [ ] B. each object individually
- [x] C. the class
- [ ] D. the constructor only

<details>
  <summary> the class </summary>
  
</details>
<!------------------------>

---

Q 58. What does `this` refers to in a java instance method?
- [ ] A. the supperclass
- [x] B. the current object
- [ ] C. the current package
- [ ] D. the class loader

<details>
  <summary> the current object </summary>
  
</details>
<!------------------------>

---

Q 59. Which java statement calls another constructor in the same class?
- [ ] A. this()
- [x] B. super()
- [ ] C. new()
- [ ] D. static()

<details>
  <summary> <b> constructor chaining </b> this() </summary>

<br/>

In Java, `this()` calls another constructor within the same class. This is called constructor chaining.

```java
class Student {
    Student() {
        this("Aman");  // Calls the parameterized constructor
        System.out.println("Default constructor");
    }

    Student(String name) {
        System.out.println("Name: " + name);
    }
}
-------------------------------
Output:
Name: Aman
Default constructor
```

- `this()` -> calls another constructor in the same class.
- `super()` -> calls a constructor of the parent class.
- Both must appear as the first statement in a constructor.


  
</details>
<!------------------------>

---

Q 60. What does the friend keyword allow in C++?
- [ ] A. Multiple Inheritance
- [ ] B. Constructor Overloading
- [ ] C. Automatic Memory Allocation
- [x] D. Access to private and protected members

<details>
  <summary> friend keyword  </summary>

<br/>

In C++, the `friend` keyword allows a non-member function or another class to access the private and protected members 
of a class.

```cpp
#include <iostream>
using namespace std;

class Student {
private:
    int marks = 90;

public:
    friend void showMarks(Student s);
};

void showMarks(Student s) {
    cout << s.marks;  // Allowed because showMarks is a friend
}
----------------
Output: 90
```
Normally, a non-member function cannot access private members. <br/> 
Declaring it as a friend grants that access.

> `friend` -> grants access to private and protected members.

> `private` -> restricts access.

> `public` -> permits access through the public interface.

> **Friendship grants access; it does not make a function a class member.**
  
</details>
<!------------------------>

---

Q 61. Which programming paradigm focus obn breaking down a program into smaller procedures or functions?
- [ ] A. Object Oriented Programming
- [x] B. Procedural Programming
- [ ] C. Functional Programming
- [ ] D. Imperative Programming

<details>
  <summary> Procedural Programming </summary>
  
</details>
<!------------------------>

---

Q 62. What is the main focus of procedural programming?
- [ ] A. Data Abstraction
- [ ] B. Object Creation
- [ ] C. Code Reusability
- [x] D. Sequential Execution

<details>
  <summary> Sequential Execution </summary>
  
</details>
<!------------------------>

---

Q 63. Which keyword is used to create an instance of a class in most programming language?
- [ ] A. alloc
- [x] B. new
- [ ] C. create
- [ ] D. instance

<details>
  <summary> new </summary>
  
</details>
<!------------------------>

---

Q 64. In OOP, what does **method signature** refers to?
- [ ] A. The name of the method
- [ ] B. The return type of the method
- [ ] C. the parameters of the method
- [x] D. the combination of method name and parameters

<details>
  <summary> the combination of method name and parameters </summary>
  
</details>
<!------------------------>


