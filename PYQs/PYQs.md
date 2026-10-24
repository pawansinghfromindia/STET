### STET - PYQs(Previous Year Questions)



<details>
  <summary> <b> PYQs 2025 </b> </summary>


<br/>

Q.1. What is the main purpose of inheritance in OOP?
- [ ] A. To create instances of classes
- [ ] B. To prevent data abstraction
- [x] C. To establish a parent-child relationship between classes
- [ ] D. To define exception

Correct answer: C To establish a parent-child relationship between classes.

**1. Understand the concept** <br/>
**Inheritance** is an Object-Oriented Programming (OOP) feature that allows one class to acquire properties and methods from another class.

There are two important terms:
- Parent class (base class): The class whose properties and methods can be inherited.
- Child class (derived class): The class that inherits from the parent class.

For example, a Dog is an Animal. A dog can use common animal behaviors while also having its own specific behaviors.


**2. Python example**
```py
class Animal:             # Parent class
   def eat(self):
       print("Animal is eating")

class Dog(Animal):        # Child class
   def bark(self):
      print("Dog is barking")

d = Dog()
d.eat()
d.bark()

# Output:
# Animal is eating
# Dog is barking
```
Notice that `Dog` defines only the `bark()` method, but its object can also call `eat()` because `Dog` inherits from `Animal`.

**3. Why are the other options incorrect?**
| Option	                          | Explanation                                                               |
|-----------------------------------|---------------------------------------------------------------------------|
| A. To create instances of classes	| Creating objects is called instantiation, not inheritance.                |
| B. To prevent data abstraction	  | Inheritance does not prevent abstraction. These are separate OOP concepts.|
| C. To establish a parent-child relationship	| A child class inherits features from a parent class.            |
| D. To define exception	          | Exceptions are handled using exception-handling mechanisms such as try and except in Python. |

**4. Benefits of inheritance**
- **Code reusability**: Reuse existing methods instead of writing them again.
- **Extensibility**: Add new behavior in a child class.
- **Maintainability**: Common functionality can be managed in the parent class.

**5. Exam tip: Remember these distinctions**
- **Inheritance** -> acquiring features from another class.
- **Encapsulation** -> bundling data and methods together and controlling access.
- **Abstraction** -> exposing essential features while hiding implementation details.
- **Polymorphism** -> the same interface or method call can behave differently in different contexts.

---

**Question 2: Application of Microcontrollers**

Q.2. Microcontrollers find application in various fields. What is a typical application of microcontrollers in the automotive industry? bihar-stet-class-11-12-computer-science-3Nov2025pdf.pdf
- [ ] A. Operating systems for computers
- [ ] B. Entertainment systems in airplanes
- [x] C. Engine control in cars
- [ ] D. Weather forecasting systems

Correct answer: C Engine control in cars

**1. What is a microcontroller?** <br/>
A **microcontroller (MCU) is a small integrated circuit** that contains the essential components of a computer on a single chip.

It typically includes:
- **CPU**: Executes instructions.
- **Memory**: Stores programs and data.
- **Input/output (I/O) interfaces**: Communicate with sensors and other devices.
- **Timers and other peripherals**: Help control operations and measure time.
Unlike a general-purpose computer, a microcontroller is commonly designed to perform a specific control task inside a larger device.


**2. How does a microcontroller control a car engine?**

<img width="500" height="300" alt="image" src="https://github.com/user-attachments/assets/9d2bf335-d9b1-4b0b-bdc4-fbe651210b91" />

For example, when engine conditions change, the engine control unit (ECU) processes sensor readings and adjusts fuel injection or ignition timing as needed.

The microcontroller is one of the components that makes this automatic control possible.

**3. Why are the other options incorrect?**
| Option	                            | Explanation       |
|-------------------------------------|-------------------|
| A. Operating systems for computers	| General-purpose computer operating systems are not the typical automotive microcontroller application described here. |
| B. Entertainment systems in airplanes	 | Such systems may use embedded computing, but this option is not an application in the automotive industry.  |
| C. Engine control in cars.    |  Microcontrollers process sensor inputs and control engine functions. |
| D. Weather forecasting systems | Weather forecasting generally relies on powerful computing systems rather than the specific embedded control application asked about. |


**4. Microcontroller vs. microprocessor**

This is a useful exam concept because questions often compare these two terms.

| Microcontroller	       | Microprocessor   |
|------------------------|------------------|
| CPU, memory and peripherals commonly integrated on one chip |	Primarily a processing unit; often relies on external memory and other components |
| Common in embedded control systems	| Common in general-purpose computing systems  |
| Example: engine control unit	      | Example: CPU in a desktop computer           |

These are general distinctions; modern devices can blur the boundaries.


**5. Remember for the exam: Microcontroller = embedded control**.

Common applications include:
- **Cars**: `engine control`, `airbags` and other `control systems`.
- **Washing machines**: `wash cycles` and `motor control`.
- **Microwave ovens**: `timing` and `heating control`.
- **Medical devices**: `monitoring` and `device control`.

A washing machine automatically controls its motor and wash cycle. Which component is most suitable for carrying out these predefined control tasks?
- [x] A. Microcontroller
- [ ] B. Desktop operating system
- [ ] C. Web browser
- [ ] D. Weather forecasting software

Correct!
A microcontroller can read inputs and control the motor and wash cycle according to a programmed sequence.

---

Q.2. FTA stands for _____
- [ ] A. File Allocation Tree
- [x] B. File Allocation Table
- [ ] C. File Allocation Graph
- [ ] D. All of the above

Correct answer: B. File Allocation Table


**Step 1: What is FAT?** <br/>
**FAT** stands for **File Allocation Table**. <br/>
It is a file system structure used to keep track of how files are stored on a storage device, such as a hard disk, USB drive, or memory card.

**Step 2: Why is it needed?**<br/>
A file may occupy multiple clusters on a disk. <br/>
FAT keeps track of those clusters so the operating system can locate the file's contents.

Simple example: How a file is stored

<img width="500" height="400" alt="image" src="https://github.com/user-attachments/assets/4fe682dd-4c3f-48a5-a79b-60a6a4b7b453" />

**4. Exam memory tip** <br/>  
Remember: **FAT = File Allocation Table → file system → tracks disk clusters**.

Don't confuse FAT with a folder tree: the folder structure organizes names and directories, while FAT tracks the allocation of file data.

What does FAT primarily help the operating system track?
- [ ] The CPU's instructions
- [x] The disk clusters allocated to files
- [ ] The computer's network password
- [ ] The screen resolution

Correct! FAT tracks file-data allocation on the storage device.

---

Q.4 What is CRUD an acronym for in database operations?
- [x] A. Create, Read, Update, Delete
- [ ] B. Cache, Read, Update, Delete
- [ ] C. Copy, Replace, Update, Delete
- [ ] D. Collect, Read, Use, Discard

Correct answer: A. Create, Read, Update, Delete

**1. Understand CRUD step by step** <br/>
CRUD represents the four basic operations performed on data in a database.

<img width="500" height="450" alt="image" src="https://github.com/user-attachments/assets/836ae379-af7f-4bf0-b9d5-c6cc47e2e72f" />

**2. See CRUD in SQL** <br/>
Here is how these operations commonly map to SQL commands:
| CRUD operation | SQL command |
|----------------|-------------|
| Create	       | `INSERT`    |
| Read	         | `SELECT`    |
| Update	       | `UPDATE`    |
| Delete	       | `DELETE`    |

For example, adding a student:
```sql
INSERT INTO Students (RollNo, Name)
VALUES (101, 'Ravi');
```
Reading student records:
```sql
SELECT * FROM Students;
```

Important distinction: In CRUD, Create means creating a data record, not necessarily creating a database table. Creating a table uses SQL's CREATE TABLE statement.

**3. Why are the other options wrong?**
- B. Cache, Read, Update, Delete - Cache is not the C in CRUD.
- C. Copy, Replace, Update, Delete - Copy and Replace are not the standard CRUD operations.
- D. Collect, Read, Use, Discard - These are not the standard database-operation terms.

Which SQL command corresponds to the Update operation in CRUD?
- [ ] `INSERT`
- [ ] `SELECT`
- [x] `UPDATE`
- [ ] `DELETE`

Correct! UPDATE modifies existing records.

---

Q.5 Which principle ensures that only essential information is visible to the outside world?
- [ ] A. Polymorphism
- [ ] B. Information hiding
- [ ] C. Encapsulation
- [x] D. Abstraction

Correct answer: D. Abstraction

**1. Understand the concept step by step** <br/>
**Abstraction** means exposing the important features of an object while hiding unnecessary implementation details.

Think about driving a car:
```
What you use
- Steering wheel, accelerator and brake.

What you don't need to manage directly
- Internal engine mechanisms and fuel-injection details.

You can drive the car without knowing every detail of how its engine works.
This illustrates abstraction.
```
In programming, a user might call a method such as `car.start()` without needing to know all the internal steps used to start the engine.

**2. Differentiate the four options** <br/>
These concepts are related, but they are not identical.
| Concept	                | Main idea	                          | Simple example                               |
|-------------------------|-------------------------------------|----------------------------------------------|
| **Polymorphism**	      | One interface, different behaviors	| `draw()` works differently for a circle and a rectangle |
| **Information hiding**	| Prevent direct access to internal details	| A private variable cannot be accessed directly from outside a class |
| **Encapsulation**	      | Bundle data and methods together and control access	| A BankAccount class manages its balance through methods |
| **Abstraction**	        | Show essential features and hide implementation complexity | Drive a car without understanding its engine internals |

**Exam tip**: When the question emphasizes essential features or hiding implementation complexity, choose Abstraction. When it emphasizes restricting access to internal data, think Information hiding or Encapsulation, depending on the wording.

You use an ATM to withdraw money without knowing how the bank processes the transaction internally. Which OOP principle does this best illustrate?
- [ ] Polymorphism
- [x] Abstraction
- [ ] Inheritance
- [ ] Method overloading

Correct! You use the essential ATM functions without needing to know the internal processing.


---

**1. What is an Ethernet network?** <br/>
Ethernet is a widely used technology for connecting devices in a Local Area Network (LAN), such as computers in a school, office, or computer lab.

<img width="976" height="327" alt="image" src="https://github.com/user-attachments/assets/ebd47fa9-5404-45e8-a862-b8eef4cc7af1" />

For example, computers in a school lab can use Ethernet to communicate with one another, access shared resources, and connect to the internet through a network device.

**2. Important Ethernet facts for the exam**
- **Network type**: Commonly used in LANs.
- **IEEE standard**: IEEE 802.3.
- **Common medium**: Twisted-pair copper cables and fibre-optic cables.
- **Addressing**: Ethernet frames use MAC addresses for local network delivery.
- **Device commonly used**: An Ethernet switch connects devices within a LAN.
- **Data unit**: Ethernet transmits data in frames.

**3. How does Ethernet differ from the other options?**
| Option	                  | What it refers to                                                    |
|---------------------------|----------------------------------------------------------------------|
| A. **Ethernet networks**	    | LAN technology standardized by IEEE 802.3                            |
| B. **Token Ring networks**	  | A LAN technology that uses a token-passing access method             |
| C. **ATM networks**	          | Asynchronous Transfer Mode, a networking technology using fixed-size cells |
| D. **Point-to-Point networks**|	A direct link between two endpoints; a general connection arrangement rather than a specific LAN technology like Ethernet |


Exam memory tip: Remember **Ethernet = IEEE 802.3, while Token Ring = IEEE 802.5**.

---

Q.7 Stealing someone's intellectual work and representing it as your own is known as ………… .
- [ ] A. Fraud
- [ ] B. Identity Theft
- [ ] C. Online Stealing
- [x] D. Plagiarism

Correct answer: D. Plagiarism

**1. Understand the concept step by step** <br/>
Plagiarism means using another person's original work or ideas and presenting them as your own without proper acknowledgment.

Examples include:
- Copying someone's assignment and submitting it under your name.
- Copying paragraphs from a website into your project without citing the source.
- Using someone else's research or writing and claiming that you created it.

**2. Why are the other options incorrect?**
| Option	                | Meaning	                                                  | Why it is incorrect here |
|-------------------------|-----------------------------------------------------------|--------------------------|
| A. **Fraud**	          | Deliberate deception, often for unlawful gain	Too general;| the specific act described is plagiarism. |
| B. **Identity Theft**	  | Using another person's identifying information without authorization | Concerns someone's identity, not specifically copying their work. |
| C. **Online Stealing**	| A general, nonstandard description	| Not the established term for presenting another person's intellectual work as your own. |
| D. **Plagiarism**	      | Presenting another person's work or ideas as your own without proper credit	| Correct answer. |

**3. Exam memory tip**
- **Plagiarism** -> copying intellectual work without proper credit.
- **Identity theft** -> misusing another person's identity.
- **Fraud** -> deception for an improper or unlawful purpose.


A student copies an article from the internet and submits it as their own assignment without mentioning the author. What is this called?
- [ ] Identity theft
- [x] Plagiarism
- [ ] Data encryption
- [ ] Authentication
      
Correct! Copying someone else's work without proper credit is plagiarism.

---

Q.8 Even with two-factor authentication, users may still be vulnerable to _____________ attacks.
- [ ] A. Scripting
- [ ] B. Cross attack
- [x] C. Man-in-the-middle
- [ ] D. Radiant

Correct answer: C. Man-in-the-middle

**1. Understand the concept step by step** <br/>
First, let's understand two-factor authentication (2FA).

Two-factor authentication requires two different forms of verification to sign in. For example:
1. Something you know - your password.
2. Something you have - a one-time code from an authenticator app.
Even with 2FA, an attacker may use a man-in-the-middle (MITM) attack to intercept or relay communication between the user and the legitimate service.

<img width="591" height="316" alt="image" src="https://github.com/user-attachments/assets/8615ab28-c0dc-4786-8d66-8c593224cf04" />


Important: **2FA still significantly improves security**. However, some forms of 2FA, such as codes entered into a phishing site, can be relayed by an attacker. Phishing-resistant authentication, such as passkeys, offers stronger protection against this type of attack.


**2. Why are the other options incorrect?**
- A. **Scripting** - Too broad; scripting can be involved in different attacks, but it is not the best answer here.
- B. **Cross attack** - Not a standard, specific attack name in this context.
- C. **Man-in-the-middle** - Correct. An attacker can intercept or relay communication, potentially compromising a login session.
- D. **Radiant** - Not a recognized attack type in this context.

**3. Exam memory tip** <br/>
**MITM = Man in the Middle**. An attacker positions themselves between two communicating parties to intercept or manipulate communication.

What does MITM stand for?
- [ ] Multiple Internet Transmission Method
- [x] Man-in-the-middle
- [ ] Managed Internal Threat Monitoring
- [ ] Multi-Input Transfer Mechanism

Correct! MITM stands for Man-in-the-middle.

---

Que. 9 The ability of a class to provide different implementations of a method based on the input parameters?
- [x] A. Overloading
- [ ] B. Polymorphism
- [ ] C. Inheritance
- [ ] D. Encapsulation

Correct answer: A. Overloading

**1. Understand method overloading step by step** <br/>
Method overloading means defining multiple methods with the same name but different parameter lists.

For example, in Java:
```java
class Calculator {
    int add(int a, int b) {
        return a + b;
    }

    int add(int a, int b, int c) {
        return a + b + c;
    }
}
```
Both methods are named `add`, but they accept different numbers of parameters.
```java
add(2, 3);       // Calls the first method: 5
add(2, 3, 4);    // Calls the second method: 9
```
The compiler selects the appropriate method based on the arguments supplied.

**2. Exam memory tip**
- Same method name + different parameters -> **Overloading**
- Subclass provides its own implementation of an inherited method -> **Overriding**

Which example demonstrates method overloading?
- [x] `print(int x)` and `print(String x)` in the same class
- [ ] A child class inherits a field from its parent
- [ ] A class makes a variable private
- [ ] A class creates an object

Correct! Both methods have the same name but different parameter types.


---

Q.10 Which of the following refers to creating products tailored to individual customers?
- [x] A. Customization
- [ ] B. Adaptation
- [ ] C. Direct material
- [ ] D. Auction

Correct answer: A. Customization

**1. Understand the concept step by step** <br/>
Customization means modifying or designing a product or service according to an individual customer's needs, preferences, or requirements.

For example, imagine you're buying a laptop online.
```
A customer chooses:
- RAM: 16 GB
- Storage: 1 TB
- Color: Silver
The customer selects the specifications they prefer instead of accepting only one fixed configuration. This illustrates customization.
```
Other examples include personalized T-shirts, customized phone cases, and made-to-order furniture.

**2. Why are the other options incorrect?**
| Option	              | Meaning	                                                    | Why it isn't correct |
|-----------------------|-------------------------------------------------------------|----------------------|
| A. **Customization**	| Tailoring a product to an individual customer's preferences	| Correct answer. |
| B. **Adaptation**	    | Adjusting something to suit a new condition or environment	| Broader than individual product personalization. |
| C. **Direct material** | Material that becomes part of a manufactured product	| A production-cost term, not the process described. |
| D. **Auction**	       | A process in which buyers bid for an item	| Describes a selling method, not product customization. |

**5. Exam memory tip: Customization = customer-specific product**.

Don't confuse it with mass production, where many identical products are manufactured, or mass customization, where products are produced at scale while still allowing individual choices.

A company allows customers to print their own names and select designs on phone covers. What is this an example of?
- [ ] Auction
- [x] Customization
- [ ] Direct material
- [ ] Data encryption

Correct! Customers personalize the product to their preferences.

---

Q.11 The length of an IPv6 address is:
- [ ] A. 32 bits
- [ ] B. 64 bits
- [x] C. 128 bits
- [ ] D. 256 bits

Correct answer: C. 128 bits

An IPv6 address is 128 bits long. This is the standard address length defined for Internet Protocol version 6.

**1. Understand the concept step by step** <br/>

Step 1: **What is an IP address?** <br/>
An Internet Protocol (IP) address identifies a network interface so devices can communicate across networks.

There are two important versions:
| Feature	       | IPv4	                             | IPv6                                   |
|----------------|-----------------------------------|----------------------------------------|
| Address length | 32 bits	                         | 128 bits                               |
| Format	       | Decimal numbers separated by dots | Hexadecimal groups separated by colons |
| Example	       | `192.168.1.1`                     | `2001:db8::1`                          |

Step 2: **Why does IPv6 use 128 bits?** <br/>
IPv6 was designed to provide a much larger address space than IPv4.
- IPv4 provides `2^32` possible bit patterns.
- IPv6 provides `2^128` possible bit patterns.
That means IPv6 can support an enormously larger number of addresses.

Step 3: **How is an IPv6 address organized?** <br/>
A full IPv6 address has eight groups of hexadecimal digits. Each group represents 16 bits.

`8 x 16 = 128 bits`

For example: `2001:0db8:0000:0000:0000:0000:0000:0001` <br/>
The address can be shortened to `2001:db8::1` by using IPv6's zero-compression rules.

**2. Exam memory tip**
- **IPv4 = 32 bits**
- **IPv6 = 128 bits**

How many bits are in an IPv4 address?
- [ ] 16 bits
- [x] 32 bits
- [ ] 64 bits
- [ ] 128 bits

Correct! IPv4 uses 32 bits, while IPv6 uses 128 bits.

---

Q.12 A platform where individuals or groups regularly publish written content, typically in a reverse chronological order is known as:
- [ ] A. News Group
- [x] B. Blog
- [ ] C. Chat Group
- [ ] D. Social Networking

Correct answer: B. Blog

A blog is a website or online platform where an individual or group publishes articles, opinions, tutorials, or other written content.

The clue in this question is "written content, typically in a reverse chronological order."


**1. Understand "reverse chronological order"** <br/>
- **Chronological order** means arranging events from oldest to newest.
- **Reverse chronological** order means arranging them from newest to oldest.

For example, suppose a computer science blog publishes these posts:


<img width="562" height="247" alt="image" src="https://github.com/user-attachments/assets/e214aef7-03fe-459c-97ef-2ac515b5a935" />


**2. Why are the other options incorrect?**
| Option	                  | Meaning                                                       |
|---------------------------|---------------------------------------------------------------|
| A. **News Group**	        | An online discussion forum or group organized around a topic  |
| B. **Blog**	              | A platform for publishing articles and written posts - correct|
| C. **Chat Group**	        | A group for exchanging messages and conversations             |
| D. **Social Networking**	| A platform for connecting and interacting with people         |

> A social networking site can also contain blog posts, but Blog is the most specific answer to this question.


**3. Exam memory tip, Remember these clues:**
- Articles or posts, newest first -> **Blog**
- Real-time messaging -> **Chat group**
- Connecting with people -> **Social networking**


A teacher regularly publishes computer programming tutorials on a website, with the latest tutorial displayed at the top. What is this website most likely called?
- [x] Blog
- [ ] Chat group
- [ ] News group
- [ ] Operating system

Correct! A blog publishes posts or articles, often with the newest first.

---

Q.13 A text file `song.txt` contains the following contents in it: `Life goes on as it never ends`
What will be the output of the following code snippet?
```py
f1 = open("song.txt", "r")
s1 = f1.read(5)
s2 = f1.readline(4)
s3 = f1.read(3)
print(s1, s3, sep="#")
```
- [ ] A. goes # on
- [ ] B. Life #goes # on
- [x] C. Life # on
- [ ] D. Error

Correct answer: C. Life # on

Let's trace the code carefully. The key is that each read operation continues from the file's current position.

**1. Step-by-step execution** 
```
Initially, the file contains:

Life goes on as it never ends

Step 1: s1 = f1.read(5)

The read(5) method reads the next 5 characters.

s1 = "Life "

Notice that the fifth character is a space after Life.
------------------------------------------------------

Step 2: s2 = f1.readline(4)

The file pointer has moved past those first five characters.
readline(4) now reads up to four characters from the current position.

s2 = "goes"

The file pointer is now just before the space following goes.
--------------------------------------------------------------

Step 3: s3 = f1.read(3)

The next three characters are a space, o, and n.

s3 = " on"
-------------------------------------------------------------
Step 4: print(s1, s3, sep="#")

The print() function prints s1 and s3, placing # between them.
- s1 contains "Life " - with a trailing space.
- s3 contains " on"   - with a leading space.
-------------------------------------------------------------
Therefore, the output is: "Life # on"
```
1. `read(5)` -> `"Life "`
2. `readline(4)` -> `"goes"`
3. `read(3)` -> `" on"`

Exam memory tips
- `read(n)` reads up to n characters.
- `readline(n)` reads up to n characters from the current position, stopping earlier if a newline is encountered.
- Reading advances the file pointer.
- Only variables included in `print()` are displayed.

If we changed the last line to print(s2), what would be printed?
- [ ] `Life` 
- [x] `goes`
- [ ] `on`
- [ ] The entire file

Correct! s2 contains the four characters 'goes'.

---

Q14. Who used the term “IoT” first?
- [ ] A. Steve Jobs
- [ ] B. Bill Simpson
- [x] C. Kevin Aston
- [ ] D. None of these

Correct answer: C. Kevin Ashton. He coined the term Internet of Things (IoT) in 1999 while working on a presentation related to supply-chain management and RFID technology.

**Understand the concept** <br/>
**IoT (Internet of Things)** means physical objects connected to the internet that can collect, send, or receive data.

Examples:
- A smartwatch tracking your steps.
- A smart thermostat adjusting room temperature.
- Sensors monitoring soil moisture on a farm.


- **Steve Jobs** — known for co-founding Apple, not for coining IoT.

**Exam tip: Remember Kevin Ashton -> Internet of Things (IoT) -> 1999.**

Which technology is commonly used in IoT devices to identify objects wirelessly?
- [x] A. RFID
- [ ] B. HTML
- [ ] C. SMTP
- [ ] D. SQL

**RFID stands for Radio-Frequency Identification**. It uses radio waves to identify and track objects wirelessly.

Example: RFID tags are used in library books, access cards, and inventory tracking.

Exam tip: RFID is commonly associated with IoT because it helps devices identify and track physical objects.

---

Q15. Languages commonly supported by Dreamweaver for web development?
- [ ] A. Python and Ruby
- [x] B. HTML and CSS
- [ ] C. C++ and Java
- [ ] D. PHP and MySQL

**Adobe Dreamweaver** is a web development tool used to create and edit websites.
- **HTML (HyperText Markup Language)**: Defines the structure of a webpage, such as headings, paragraphs, images, and links.
- **CSS (Cascading Style Sheets)**: Controls the appearance of a webpage, including colors, fonts, spacing, and layout.

```html
<h1>Hello Students!</h1>
```

```css
h1 {
  color: blue;
}
```

HTML creates the heading; CSS makes its text blue.

Why the other options are incorrect: 
- Python and Ruby are not the primary languages this question targets;
- C++ and Java are not standard webpage structure/styling languages;
- PHP and MySQL are commonly used for server-side programming and databases, respectively.

---

Q16. What is the purpose of a constructor in OOP?
- [ ] A. To destroy objects
- [ ] B. To create instances of abstract classes
- [x] C. To initialize object properties
- [ ] D. To define abstract methods

**A constructor is a special method that runs when an object is created**. <br/>
Its main purpose is to initialize the object's properties so the object starts with the required values.

Example in Java
```java
class Student {
    String name;

    Student(String studentName) {
        name = studentName;
    }
}

Student s1 = new Student("Rahul");
```

Why the other options are incorrect

- A. To destroy objects - destruction or cleanup is handled differently depending on the language; a constructor creates/initializes rather than destroys.
- B. To create instances of abstract classes - abstract classes generally cannot be instantiated directly.
- D. To define abstract methods - abstract classes may declare abstract methods, but that is not the purpose of a constructor.

Exam tip: 

**Constructor = object initialization**. <br/>
In Java, a constructor has the same name as its class and has no return type.

---

Q.17 What is the main advantage of using abstract classes over interfaces
- [ ] A. Abstract classes can have multiple inheritance, unlike interfaces
- [ ] B. Interfaces can have constructors, while abstract classes cannot
- [x] C. Abstract classes can provide default implementations of methods
- [ ] D. Interfaces allow for private access modifiers, unlike abstract classes

Correct answer: Option C because an abstract class can contain both implemented methods and abstract methods that subclasses must implement.

**Understand the concept from the basics** <br/>

Let's understand the difference between an abstract class and an interface using Java.

**1. What is an abstract class?**
> An abstract class is a class that cannot be instantiated directly.
> It can provide common functionality to its subclasses.

```java
abstract class Animal {
    void eat() {
        System.out.println("Eating...");
    }

    abstract void sound();
}
```
Notice two methods:
- `eat()` has a body, so it already provides an implementation.
- `sound()` has no body, so a concrete subclass must implement it.

Now, a subclass can reuse the existing `eat()` method:
```
class Dog extends Animal {
    void sound() {
        System.out.println("Barking");
    }
}
```

When a `Dog` object calls `eat()`, it uses the implementation inherited from Animal. 
The `Dog` class only needs to implement `sound()`.

This is the key idea: an abstract class can provide shared, ready-to-use method implementations while leaving some behavior for subclasses to define.

**2. What is an interface?**
> An interface defines a contract that implementing classes agree to follow.
```java
interface Animal {
    void sound();
}
```
A class implementing this interface must provide the required `sound()` implementation:
```java
class Dog implements Animal {
    public void sound() {
        System.out.println("Barking");
    }
}
```

Important Java nuance: modern Java interfaces can also have default methods with implementations. So Option C describes a capability of abstract classes, but it is not an exclusive advantage over every modern interface.


**3. Why are the other options incorrect?**

| Option	                | Explanation       |
|-------------------------|-------------------|
| A. **Multiple inheritance** |	Incorrect. Java classes cannot extend multiple classes. A class can, however, implement multiple interfaces. |
| B. **Interfaces have constructors**	| Incorrect. Interfaces do not have constructors. Abstract classes can have constructors, which run when a subclass is instantiated.
| C. **Default implementations in abstract classes**	| Correct for the intended exam answer. Abstract classes can provide concrete methods that subclasses reuse. |
| D. **Interfaces allow private access modifiers, unlike abstract classes**	| Incorrect. Abstract classes support private members. Modern Java interfaces can also have private methods, subject to Java's interface rules. |


**4. Exam memory tip**
- **Abstract class**: shared state, constructors, and implemented methods.
- **Interface**: a contract that classes implement; a class can implement multiple interfaces.
- **Multiple class inheritance**: not supported in Java.
- **Modern Java**: interfaces can have default and static methods, and private methods since Java 9.


Suppose three classes - `Dog`, `Cat`, and `Cow` - all need the same implemented `eat()` method, but each must provide its own `sound()` method.

Which is a suitable design?
- [x] A. An abstract class with an implemented `eat()` method and an abstract `sound()` method
- [ ] B. A constructor that destroys objects
- [ ] C. Three unrelated classes with no shared functionality
- [ ] D. An interface with a constructor

Correct! Option A.

An abstract class is a suitable choice because it lets related classes share common functionality while implementing their own specific behavior.

In our example:
- `Animal` provides the common `eat()` method.
- `Dog`, `Cat`, and `Cow` inherit that method.
- Each class implements its own `sound()` method.

Remember for the exam: **An abstract class can contain both `concrete methods` (methods with a body) and `abstract methods` (methods without a body).**

---

Q. 18 Which networking devices is used to regenerate and transmit the weakened signal ahead?
- [ ] A. Hub
- [ ] B. Ethernet Card
- [x] C. Repeater
- [ ] D. Modem

Correct answer: C. Repeater

**1. Understand the concept from the basics**

A **repeater** is a networking device that receives a weakened signal and regenerates it so that the signal can travel farther.

Imagine sending a message across a long distance:
1. A signal travels through a network cable.
2. As it travels, the signal can weaken.
3. A repeater receives the signal.
4. It regenerates the signal and sends it onward.

This helps extend the distance over which a network signal can travel.

**Real-world example** <br/>
Suppose a network cable needs to cover a distance beyond its supported range. A repeater can help extend the connection by regenerating the signal.

Important distinction: A traditional repeater regenerates signals; it does not decide where packets should be routed.

**2. Why are the other options incorrect?**
| Option	             | Purpose                                                                            |
|----------------------|------------------------------------------------------------------------------------|
| A. **Hub**	         | Connects multiple devices in a LAN and forwards incoming data to its other ports.  |
| B. **Ethernet Card** | A network interface card that allows a computer to connect to an Ethernet network. |
| C. **Repeater**	     | Regenerates a weakened signal to extend its transmission distance. Correct.        |
| D. **Modem**	       | a modem modulates and demodulates signals for communication.                       |


**3. Exam memory tip** <br/>
Remember these associations:
- **Repeater** -> Regenerates a signal.
- **Hub** -> Connects devices in a LAN.
- **Switch** -> Forwards frames based on MAC addresses.
- **Router** -> Forwards packets between networks.
- **NIC/Ethernet card** -> Connects a device to a network.


A computer can connect to an Ethernet network using which hardware component?
- [ ] A. Repeater
- [x] B. Ethernet card (NIC)
- [ ] C. Hub
- [ ] D. Router

Correct! Option B: Ethernet card (NIC).

A **Network Interface Card (NIC)** is the hardware component that enables a computer to connect to a network. <br/>
An **Ethernet card** is a type of NIC used for wired Ethernet connections.

Remember the difference
- **NIC / Ethernet card**: Connects a computer to a network.
- **Repeater**: Regenerates a weakened signal.
- **Hub**: Connects multiple devices in a LAN.
- **Router**: Connects different networks and forwards packets between them.

Exam tip: If the question mentions regenerating a weakened signal, choose Repeater. If it asks which hardware enables a computer to connect to Ethernet, choose NIC / Ethernet card.

---

The maximum length (in bytes) of an IPv4 datagram is:
- [ ] A. 32
- [ ] B. 256
- [ ] C. 1024
- [x] D. 65535

Correct answer: D. 65535 bytes

The maximum total length of an IPv4 datagram is 65,535 bytes. This includes both the IPv4 header and the data (payload).

**1. What is an IPv4 datagram?** <br/>
IPv4 is a network-layer protocol used to deliver packets across networks. <br/>
An IPv4 datagram has two main parts:

<img width="995" height="237" alt="image" src="https://github.com/user-attachments/assets/7cc2ab9d-840d-4b37-897e-9afd00afd9c0" />


The IPv4 header contains a Total Length field that specifies the length of the entire datagram, including the header and payload.

**2. Why is the maximum 65,535 bytes?** <br/>
The Total Length field is 16 bits wide.

A 16-bit unsigned field can represent values from: **`0 to 2^16-1`** <br/>
Therefore: `2^16-1 = 65,536-1 = 65,535` <br/>
That is the maximum IPv4 datagram length.

Important: The minimum IPv4 header is 20 bytes, so with that header size, the maximum payload is `65,535 - 20 = 65,515` bytes. A longer header reduces the maximum payload further.

**3. Exam memory tip**

Remember this formula:
- **IPv4 Total Length field = 16 bits**
- **Maximum value = 2^16-1**
- **Maximum datagram length = 65,535 bytes**

Don't confuse this with the IPv4 address length, which is 32 bits.


An IPv4 datagram has a 20-byte header and a total length of 1,500 bytes. How many bytes are payload?
- [ ] A. 20 bytes
- [x] B. 1,480 bytes
- [ ] C. 1,500 bytes
- [ ] D. 1,520 bytes

**`Payload = Total Length - Header Length`**

Remember: Total length includes both the header and payload. Subtract the header to find the payload.

---

Ginni has created a table, SCORES in MySQL to store runs scored by players in a cricket match. The table contains the following records:
| PLAYER	| SCORE |
|---------|-------|
| Ranveer	| 50    |
| Sukesh	| 35    |
| Mirza	  | 10    |
| John	  | 51    |
| Murugan	| 70    |

Which of the following statements will give 10 as output?
- [ ] A. `SELECT MAX(Score) FROM Scores`;
- [x] B. `SELECT MIN(Score) FROM Scores`;
- [ ] C. `SELECT SUM(Score) FROM Scores`;
- [ ] D. `SELECT AVG(Score) FROM Scores`;

Correct answer: B. `SELECT MIN(Score) FROM Scores`

SQL provides **aggregate functions** to perform calculations on a group of rows and return a result.

Let's understand all four functions using the scores in the question.

**`MIN()` - Minimum value**
```sql
SELECT MIN(Score) FROM Scores;
-- Returns the smallest score: 10.
```

**`MAX()` - Maximum value**
```sql
SELECT MAX(Score) FROM Scores;
-- Returns the largest score: 70.
```

**`SUM()` - Total value**
```sql
SELECT SUM(Score) FROM Scores;
-- Adds all the scores: 50 + 35 + 10 + 51 + 70 = 216
```

**`AVG()` - Average value**
```sql
SELECT AVG(Score) FROM Scores;
-- return average 216/5 = 43.2
```

**`COUNT()`- count the records(rows)**
```sql
SELECT count(player) FROM Scores;
-- Return total rows in the table = 5
```

Important exam point: These functions operate on a column's values. For ordinary numeric columns, `MIN()` and `MAX()` return the lowest and highest non-NULL values, respectively.


Suppose a table named Students contains these marks: `45, 80, 65, 90, 20` <br/>
Which query returns the second-highest mark?
```
The marks are: 45, 80, 65, 90, 20
Arrange them in descending order: 90, 80, 65, 45, 20
- Highest mark = 90
- Second-highest mark = 80

Step by step
1. The inner MAX(Marks) returns 90.
2. WHERE Marks < 90 excludes the highest mark.
3. The outer MAX(Marks) returns the largest remaining mark, 80.
Output: 80
```
How can we find the second-highest mark in SQL?
```sql
SELECT MAX(Marks) FROM Students WHERE Marks < (SELECT MAX(Marks) FROM Students);
```
This method returns the second-highest distinct mark. If the highest mark occurs more than once, it excludes that value entirely.

---

Q. 21 Which data type is used to implement Queue data structure in Python?
- [ ] A. Sets
- [ ] B. Dictionary
- [ ] C. Tuple
- [ ] D. List

Correct answer: D. List

A Python list can be used to implement a queue because it supports adding and removing elements. However, a tuple is immutable, so it cannot be modified after creation in the usual way needed for a queue.

**What is a queue?** <br/>
A queue is a linear data structure that follows `FIFO - First In, First Out`.

Think of people standing in a line at a ticket counter:
- The first person to join the line gets served first.
- A new person joins at the back.
- The person at the front leaves first.

<img width="987" height="212" alt="image" src="https://github.com/user-attachments/assets/5c5f8d97-a9ec-4bc7-b90e-ff67a585b5e0" />


A simple implementation using a list is:
```py
queue = []

queue.append(10)
queue.append(20)
queue.append(30)

print(queue.pop(0))  # 10
```
- `append()` adds an element to the end of the list.
- `pop(0)` removes and returns the element at index 0, the front of the queue.

A Python list can implement a queue, but `collections.deque` is generally better for efficient removal from the front.


**Why are the other options incorrect?**
| Option	Explanation
| A. **Sets**	      | Sets are unordered collections of unique elements; they are not suitable for maintaining a FIFO sequence. |
| B. **Dictionary**	| Dictionaries store key-value pairs. They can be adapted for queue-like behavior, but they are not the intended answer here.|
| C. **Tuple**	    | Tuples are immutable, so adding and removing elements is not supported directly. | 
| D. **List**	      |  Lists support appending elements and removing the front element. |


**Exam memory tip**
- **Queue** -> FIFO (First In, First Out)
- **Stack** -> LIFO (Last In, First Out)
- **Python list** -> can implement a queue.
- **Python deque** -> preferred for efficient queue operations.


Which data structure follows LIFO (Last In, First Out)?
- [ ] A. Queue
- [x] B. Stack
- [ ] C. Tree
- [ ] D. Graph

Correct! Option B: Stack.

A stack follows LIFO — Last In, First Out.

Think of a stack of plates: the last plate you place on top is the first one you remove.

Example:
```py
stack = []

stack.append(10)
stack.append(20)
stack.append(30)

print(stack.pop())  # 30
```

---

Q. 22 In an ideal microcomputer, where is the Arithmetic Logic Unit (ALU) located?
- [x] A. CPU
- [ ] B. Memory
- [ ] C. Input devices
- [ ] D. Output devices

Correct answer: A. CPU

The **Arithmetic Logic Unit (ALU) is a component of the Central Processing Unit (CPU)**. <br/>
It performs two main types of operations: <br/>
**1. Arithmetic operations** <br/>
Mathematical calculations such as `addition`, `subtraction`, `multiplication`, and `division`. <br/>
Example: `10 + 5 = 15`

**2. Logical operations** <br/>
Operations such as `AND`, `OR`, `NOT`, and comparisons. <br/>
Example: `Is 10 > 5 ? Yes`.

<img width="811" height="681" alt="image" src="https://github.com/user-attachments/assets/fab40971-6567-47a9-94d1-e73092e8929b" />


> **The ALU is a part of the CPU**. <br/>
The CPU also contains registers and other components.

> Think of the **CPU as the computer's brain** and the **ALU as its calculator**. <br/>
The **CPU coordinates processing, while the ALU performs arithmetic and logical operations**.

| Option	           | Explanation                           |
|--------------------|---------------------------------------|
| **Memory**	       | Memory stores data and instructions. The ALU processes data; it is not located in memory. |
| **Input devices**	 | Devices such as keyboards and mice send data or commands to the computer. They do not contain the CPU's ALU. |
| **Output devices** |	Devices such as monitors and printers present the results of processing. They do not contain the CPU's ALU. |

**Exam memory tip**
> **ALU = Arithmetic + Logic = part of the CPU**.

Remember the roles:
- **ALU**: Performs calculations and logical operations.
- **CU (Control Unit)**: Directs and coordinates computer operations.
- **Memory**: Stores data and instructions.


Which component of the CPU is primarily responsible for controlling and coordinating the execution of instructions?
- [ ] A. Arithmetic Logic Unit (ALU)
- [x] B. Control Unit (CU)
- [ ] C. RAM
- [ ] D. Hard disk

Correct! Option B - Control Unit (CU)

The Control Unit (CU) is responsible for controlling and coordinating the execution of instructions inside the CPU.

Think of a computer as a team:
- **Control Unit (CU)**: The manager who tells each component what to do.
- **Arithmetic Logic Unit (ALU)**: The calculator that performs mathematical and logical operations.
- **Memory**: Stores data and instructions.

Example
Suppose the computer needs to calculate `5 + 3`.
1. The Control Unit coordinates the steps needed to execute the instruction.
2. The ALU performs the addition.
3. The result, `8`, can be stored in a register or memory, as required.


| Option	         | Why it is incorrect                                   |
|------------------|-------------------------------------------------------|
| A. **ALU**       | Performs arithmetic and logical operations, rather than primarily coordinating instruction execution. |
| B. **CU**        | Controls and coordinates instruction execution.        |
| C. **RAM**	     | Temporarily stores data and programs currently in use. |
| D. **Hard disk** | Provides long-term storage for files and programs.     |


Exam memory tip **CU = Control; ALU = Calculate**.
- **CU**: Directs operations.
- **ALU**: Calculates and compares.
- **RAM**: Temporarily stores data.
- **Hard disk**: Stores data long-term.

---

Q23. What consists of the identification of risks or threats, the implementation of security measures, and the monitoring of those measures for effectiveness?
- [ ] A. Risk assessment
- [ ] B. Security
- [x] C. Risk Management
- [ ] D. None of the above

Correct!  C. Risk Management is the best answer. because the question includes identifying risks, implementing security measures, and monitoring their effectiveness.

Risk management is the overall process of identifying risks, evaluating them, deciding how to handle them, and monitoring the effectiveness of the actions taken.

Imagine a school wants to protect its computer lab from cyberattacks.

**Step 1: Identify risks** <br/>
Find possible threats, such as viruses, stolen passwords, or unauthorized access.

**Step 2: Assess risks** <br/>
Evaluate how likely each threat is and how much damage it could cause.

**Step 3: Implement security measures** <br/>
Install antivirus software, use strong passwords, and restrict access.

**Step 4: Monitor and review** <br/>
Check whether the security measures are working and improve them if necessary.

All four steps fit within the broader process of risk management.

| Option	                | Meaning	                                      | Why it is incorrect here         |
|-------------------------|-----------------------------------------------|----------------------------------|
| A. **Risk assessment**	| Evaluates the likelihood and impact of risks. | It is only one part of risk management, not the entire process described. |
| B. **Security**	        | Protects systems, data, and resources from threats.	| It describes the protective objective or state, rather than the complete process of identifying, treating, and monitoring risks. |
| C. **Risk Management**	Identifies, assesses, treats, and monitors risks. |	Correct. It covers the full process described in the question. |

Exam memory tip, Remember this distinction:
- **Risk assessment** = How likely is the risk, and how serious is it?
- **Risk management** = Identify + assess + treat + monitor risks.

For example, finding that weak passwords are dangerous is part of risk assessment. Introducing stronger password rules and checking whether they work are part of the broader risk-management process.

A company identifies that employees may click on phishing emails, evaluates the threat, introduces security training, and regularly checks whether phishing incidents decrease. <br/>
Which process does this best describe?
- [ ] A. Risk assessment only
- [x] B. Risk management
- [ ] C. Data storage
- [ ] D. Input processing

Correct! B. Risk management

**Risk assessment** focuses on identifying and evaluating risks, including how likely they are and how much damage they could cause.

Assessing the possibility of employees clicking phishing emails is part of risk assessment. <br/>
However, the company also:
1. Identifies the phishing threat.
2. Evaluates the risk.
3. Introduces security training to reduce the risk.
4. Monitors whether phishing incidents decrease.
   
The entire process is risk management, because it includes taking action and monitoring the results, not just evaluating the risk.

| Risk assessment	                | Risk management                                      |
|---------------------------------|------------------------------------------------------|
| Identifies and evaluates risks.	| Covers the overall process of handling risks.        |
| Estimates likelihood and impact.| Includes assessment, risk treatment, and monitoring. |
| One part of risk management.	  | The broader process.                                 |

Exam memory tip
> Assessment = Evaluate. <br/>
> Management = Evaluate + Act + Monitor.

---

Q24. Which attributes is not a valid attribute of the tag in HTML ?
- [ ] A. text
- [ ] B. background
- [ ] C. bgcolor
- [x] D. width

If the intended tag is `body`, `text`, `background`, and `bgcolor` have all been used in older HTML, while `width` is not a standard body attribute. 

**What are HTML attributes?** <br/>
HTML attributes provide additional information about an HTML element. 

For example:
```html
<img src="flower.jpg" width="200" alt="A flower">
```
Here:
- `src` specifies the image source.
- `width` specifies the image width.
- `alt` provides alternative text.


| Option	        | Meaning and usage                      |
|-----------------|----------------------------------------|
| A. `text`	      | Not a standard global HTML attribute. It has been used as an attribute on certain older HTML elements, such as body. |
| B. `background`	| Used on older HTML elements, such as body, to specify a background image. It is obsolete in modern HTML. |
| C. `bgcolor`	  | Used on older elements to specify a background color. It is obsolete in modern HTML. |
| D. `width`	    | A valid attribute on elements such as `img`, `canvas`, and `iframe`.                 |

**Exam memory tip**
- HTML attributes depend on the element.
- `width` is valid on some elements, but not all.
- `background` and `bgcolor` are obsolete HTML attributes; modern pages should use CSS for backgrounds.
- Always identify the HTML tag before deciding whether an attribute is valid.

Which is the recommended modern way to set a page's background color?
- [ ] A. Use the text attribute
- [ ] B. Use the bgcolor attribute
- [x] C. Use the CSS background-color property
- [ ] D. Use the width attribute

Correct! Option C - Use the CSS `background-color` property

CSS (Cascading Style Sheets) controls the appearance and styling of HTML elements. <br/>
The `background-color` property sets an element's background color.
```html
<!DOCTYPE html>
<html>
   <head>
       <style>
           body {
              background-color: lightblue;
           }
       </style>
   </head>
<body>
   <h1> Hello, Students! </h1>
</body>
</html>
```
Here, `background-color: lightblue;` makes the page background light blue.

Exam memory tip, **HTML = structure; CSS = styling**.
- `background-color` -> sets background color.
- `color` -> sets text color.
- `width` -> sets width.

---

Q25. SQL applies conditions on the groups through ______ clause after groups have been formed.
- [ ] A. `WHERE`
- [x] B. `HAVING`
- [ ] C. `NEW`
- [ ] D. `ALL`

Correct! Option B - `HAVING`

What does `GROUP BY` do?
Suppose we have this Employees table:
| Employee | Department	| Salary |
|----------|------------|--------|
| Ravi	   | IT	        | 40,000 |
| Priya	   | HR	        | 30,000 |
| Amit	   | IT	        | 50,000 |
| Neha	   | HR	        | 35,000 |
| Kiran	   | Sales	    | 25,000 |

We want to calculate the total salary for each department.
```sql
SELECT Department, SUM(Salary)
FROM Employees
GROUP BY Department;
```
Result
| Department | Total Salary |
|------------|--------------|
| IT	       | 90,000       |
| HR	       | 65,000       |
| Sales	     | 25,000       |

`GROUP BY` combines rows with the same department so aggregate functions, such as `SUM()`, can calculate a result for each group.

What if we want only departments whose total salary exceeds ₹50,000?
```sql
SELECT Department, SUM(Salary) AS TotalSalary
FROM Employees
GROUP BY Department
HAVING SUM(Salary) > 50000;
```
| Department | Total Salary |
|------------|--------------|
| IT	       | 90,000       |
| HR	       | 65,000       |

Sales is excluded because its total salary is only ₹25,000.

Why `HAVING`? <br/>
Because the condition is applied to the groups after they have been formed.

Then what does `WHERE` do? <br/>
`WHERE` filters individual rows before grouping.

```sql
SELECT Department, SUM(Salary) AS TotalSalary
FROM Employees
WHERE Salary > 30000
GROUP BY Department;
```

**`WHERE` vs `HAVING`**
| Feature	             | `WHERE`	                  | `HAVING`                     |
|----------------------|----------------------------|------------------------------|
| Filters	             | Individual rows	          | Groups                       |
| Applied conceptually | Before grouping	          | After grouping               |
| Commonly used with	 | Ordinary column conditions	| Aggregate conditions         |
| Example	             | `WHERE Salary > 30000`	    | `HAVING SUM(Salary) > 50000` |

5. Exam memory tip, Remember:
- `WHERE` -> Rows
- `HAVING` -> Groups

A useful **SQL execution-order** shortcut is: `FROM -> WHERE -> GROUP BY -> HAVING -> SELECT -> ORDER BY`

This is the conceptual processing order, not necessarily the order in which a database physically executes every operation.

Consider the following query:
```sql
SELECT Department, COUNT(*)
FROM Employees
GROUP BY Department
HAVING COUNT(*) > 2;
```
What does `HAVING COUNT(*) > 2` do?
- [ ] A. Selects employees whose individual salary is greater than 2
- [x] B. Shows only departments containing more than 2 employees
- [ ] C. Limits the result to 2 departments
- [ ] D. Counts only 2 employees in each department

Correct! Option B - Shows only departments containing more than 2 employees

1. `FROM Employees` - Reads the employee records.
2. `GROUP BY Department` - Groups employees belonging to the same department.
3. `COUNT(*)` - Counts the employees in each department.
4. `HAVING COUNT(*) > 2` - Keeps only departments with more than two employees.

| Department | Number of employees |
|------------|---------------------|
| IT 	       | 4                   |
| HR	       | 2                   |
| Sales	     | 3                   |
| Finance	   | 1                   |

After applying `HAVING COUNT(*) > 2`, the result is:

| Department | Number of employees |
|------------|---------------------|
| IT 	       | 4                   |
| Sales	     | 3                   |

HR and Finance are excluded because they have two and one employees, respectively.

Exam memory tip: **`GROUP BY` creates groups; `HAVING` filters those groups**.

---

Q26. Given binary numbers `A = 101010` and `B = 111111`, what is the result of `(A AND B) OR (A XOR B)`?
- [x] A. 111111
- [ ] B. 101111
- [ ] C. 111010
- [ ] D. 101010

**Understand the three bitwise operators** <br/>
Each binary digit is a bit: either `0` or `1`.
| A bit	| B bit	| AND (&)	| XOR (^)	| OR (l) |
|-------|-------|---------|---------|--------|
| 0	    | 0	    | 0	      | 0	      | 0      |
| 0	    | 1	    | 0	      | 1	      | 1      |
| 1	    | 0	    | 0	      | 1	      | 1      |
| 1	    | 1	    | 1	      | 0	      | 1      |

Remember:
- `AND`: Result is 1 only when both bits are 1.
- `XOR`: Result is 1 when the bits are different.
- `OR`: Result is 1 when at least one bit is 1.

Solve it step by step
```
Given:
A = 101010
B = 111111

Step 1: Calculate A AND B

A       = 101010
B       = 111111
          ------
A AND B = 101010

Since every bit in B is 1, AND keeps each bit of A unchanged.
----------------------------------
Step 2: Calculate A XOR B
XOR gives 1 when the two bits are different.

A       = 101010
B       = 111111
          ------
A XOR B = 010101

Every bit in B is 1, so XOR flips each bit of A: 1 becomes 0, and 0 becomes 1.
-----------------------------------
Step 3: Calculate (A AND B) OR (A XOR B)

               A AND B = 101010
               A XOR B = 010101
                         ------
(A AND B) OR (A XOR B) = 111111
```

---

Q 27. DFA exist is a ________
- [x] A. Regular Language
- [ ] B. Non-Regular Language
- [ ] C. Any language
- [ ] D. Cannot be said

Correct! Option A - Regular Language is the best answer based on the visible wording and the standard **theory of finite automata**.

**DFA** stands for **Deterministic Finite Automaton**. <br/> 
In formal language theory, a language that can be recognized by a DFA is a regular language.

It is a mathematical model used to recognize patterns in strings.

A language is called regular if some finite automaton, such as a DFA, can recognize it.

For example, consider the language of binary strings that end in `1`:
- `101` -> Accepted
- `111` -> Accepted
- `100` -> Rejected
- `110` -> Rejected

A DFA can recognize this language by keeping track of whether the most recently read bit is `1`.

**Visualize how a DFA works**

<img width="987" height="551" alt="image" src="https://github.com/user-attachments/assets/b7972cc3-f05d-4407-a7f0-e9e23446f60f" />

The DFA has a finite number of states and follows defined transitions for each input symbol. This is why it can recognize this regular language.


Exam memory tip, **DFA -> Regular Language**.
- **DFA**: Deterministic Finite Automaton
- **NFA**: Nondeterministic Finite Automaton
- Both DFA and NFA recognize exactly the class of regular languages.

---

**Q28. Website vs. Web Page**

What is the difference between a website and a web page?
- [x] A. A website is a collection of web pages, while a web page is a single document that is displayed on the web.
- [ ] B. A website is a software program, while a web page is a hardware device.
- [ ] C. A website is a physical object, while a web page is a logical object.
- [ ] D. All of the above.


**Website vs. Web Page**
- **Website**: A collection of related web pages available under a common domain name.
- **Web page**: A single document displayed in a web browser.

**2. Imagine a school website**.

<img width="995" height="597" alt="image" src="https://github.com/user-attachments/assets/d56dcec6-df4d-4b65-8c4a-5dc436171d7d" />


Think of a book:
- A website is like the entire book.
- A web page is like one page of that book.
A website can contain many web pages, and each page can have its own content and URL.


**3. Exam memory tip** <br/>
Remember this simple rule: **Website = Collection. Web page = Single document**.

For example, `youtube.com` is a website, while an individual `YouTube video's page` is a web page.

A school website contains Home, About Us, Courses, and Contact Us pages. How many web pages are mentioned?
- [ ] A. One
- [ ] B. Three
- [x] C. Four
- [ ] D. Five

The school website contains these four web pages:
1. Home
2. About Us
3. Courses
4. Contact Us

Each is an individual web page, and together they form a website.
- Website = Collection of web pages.
- Web page = A single document displayed on the web.

---

**Q29. Turing Machine**

The "Turing Machine" showed that you could use a/an _____ system to program any algorithmic task.
- [x] A. Binary
- [ ] B. Electro-chemical
- [ ] C. Recursive
- [ ] D. Semantic

**What is a Turing Machine?** <br/>
A Turing Machine is a theoretical model of computation introduced by Alan Turing. 

It consists of:
- An infinite tape divided into cells for storing symbols.
- A read/write head that reads and writes symbols.
- A set of rules that determine what to do next.

<img width="767" height="367" alt="image" src="https://github.com/user-attachments/assets/8ca1c6ab-fb38-4b4f-aa63-6a4f4e4c0ef4" />

It helps us understand what problems can be solved by an algorithm.

**What does "recursive" mean here?** <br/>
In computability theory, a recursive function is a function that can be computed by an algorithm that eventually halts for every valid input.

Turing Machines and recursive functions are closely related: they characterize the same class of computable functions.

For example, adding two natural numbers can be performed by an algorithm, so it is computable.

Important distinction: A Turing Machine does not prove that every conceivable task can be programmed. It models the computation of algorithmically computable tasks.


| Option	                | Explanation      |
|-------------------------|------------------|
| A. **Binary**	          | Binary uses the symbols `0` and `1`. Computers commonly use binary, but the theoretical result about Turing Machines is not specifically that every algorithm requires a binary system. |
| B. **Electro-chemical**	| This describes a physical implementation approach, not the central theoretical result of a Turing Machine. |
| C. **Recursive**	      | Likely intended answer. Recursive functions are equivalent in computational power to Turing Machines. |
| D. **Semantic**	        | Semantics concerns the meaning of symbols or programs; it is not the expected term for this result. |

**Exam memory tip**
- **Alan Turing** -> Turing Machine
- **Turing Machine** -> Model of computation
- **Recursive functions** -> Computable functions
- **Binary** -> Representation using `0` and `1`


Which of the following is a theoretical model used to study what can be computed by an algorithm?
- [x] A. Turing Machine
- [ ] B. HTML page
- [ ] C. Database table
- [ ] D. Network cable

> **A Turing Machine is a theoretical model used to study what problems can be solved by algorithms.**

A Turing Machine has three basic components:
- **Tape**: Stores symbols and data.
- **Read/write head**: Reads and writes symbols on the tape.
- **Control unit**: Follows rules to determine the next operation.

For example, an algorithm for adding two numbers can be represented using a computational model such as a Turing Machine.

Remember for the exam
- Turing Machine -> Model of computation.
- Alan Turing -> Introduced the concept.
- Recursive functions -> Closely related to computable functions.
- Binary -> Uses `0` and `1`.

---

**Q30. Exception in Programming**

The condition that occurs during program execution that disrupts the normal flow of instructions?
- [ ] A. Abstraction
- [ ] B. Inheritance
- [x] C. Exception
- [ ] D. Encapsulation

**1. What is an exception?** <br/>
An exception is an event or condition that occurs during program execution and disrupts the normal flow of instructions.

For example, consider this Python program:
```py
a = 10
b = 0

result = a / b

print(result)
print("Program finished")
```
When Python tries to divide `10` by `0`, it raises a `ZeroDivisionError`.
```
a = 10 executes successfully.
b = 0 executes successfully.
a / b raises an exception.
print("Program finished") is not executed in this example.
```
We can handle this exception using `try` and `except`:
```py
try:
    result = 10 / 0
except ZeroDivisionError:
    print("Cannot divide by zero")

print("Program finished")

# output: 
# Cannot divide by zero
# Program finished
```
The exception is handled, allowing the program to continue.

| Option	          | Meaning	                                  | Why it is incorrect                              |
|-------------------|-------------------------------------------|--------------------------------------------------|
| **Abstraction**	  | Hiding unnecessary implementation details	| It is an OOP concept, not the condition described.|
| **Inheritance**	  | One class acquiring properties and methods from another class	| It supports code reuse and class relationships; it is not an exception. |
| **Exception**	    | An event or condition disrupting normal program execution	| Correct answer. |
| **Encapsulation**	| Bundling data and methods together and controlling access	| It is an OOP concept, not the condition described. |

4. Exam memory tip, Remember these four terms:
- **Abstraction** -> Hide complexity.
- **Inheritance** -> Reuse or extend a class.
- **Exception** -> An abnormal event during execution.
- **Encapsulation** -> Bundle data and methods together.

| Option	          | Meaning                                                      |
|-------------------|--------------------------------------------------------------|
| TypeError	        | An operation is applied to an incompatible type.             |
| ZeroDivisionError	| Division or modulo operation uses zero as the divisor.       |
| NameError	        | A name is used that Python cannot find in the current scope. |
| SyntaxError	      | The code violates Python's syntax rules.                     |

Exam memory tip
- **Divide by zero** -> ZeroDivisionError
- **Wrong type of operation** -> TypeError
- **Undefined name** -> NameError
- **Invalid syntax** -> SyntaxError
  
---

**Q31. Meaning of Data**

The term "Data" refers to:
- [ ] A. The electronic representation of the information (or data)
- [ ] B. Basic information
- [ ] C. Raw Facts and figures
- [x] D. Both A and C

**1. What is data?** <br/>
Data refers to raw facts and figures that can be collected, stored, and processed by a computer.

Examples:
- `25` - a number
- `Naman` - a name
- `85, 90, 78` - exam marks
- `24/10/2027` — a date
By themselves, these values are data. When organized and interpreted, they can provide useful information.

**Understand data vs. information**
```
Data
85, 90, 78

Raw exam marks
--------------------
Information
"The student's average mark is 84.33."

The data has been processed to provide meaning.
```

A teacher records these marks: 70, 85, 90. Before calculating the average, what do these numbers represent?
- [ ] A. Processed information
- [x] B. Raw data
- [ ] C. A computer program
- [ ] D. An output device

Understand the difference
- **Data**: `70, 85, 90` - the individual marks.
- **Processing**: Calculate the average: `(70 + 85 + 90)/ 3`.
- **Information**: The average mark is approximately `81.67`.

**Exam memory tip**
> Raw facts and figures = Data.

> Processed data that conveys meaning = Information.

---

**Q32. First Web Browser**

Which among the following was the first web browser?
- [ ] A. Internet Explorer
- [x] B. Mosaic
- [ ] C. Google Chrome
- [ ] D. Opera


**1. History of Web Browser**

The important historical detail is that the first web browser was WorldWideWeb, created by Tim Berners-Lee in 1990 at CERN. It was later renamed Nexus.

**`WorldWideWeb (1990)`**
- First web browser
- Created by Tim Berners-Lee.
- It could browse and edit web pages.

**`Mosaic (1993)`**
- Popular early graphical browser
- Helped make the web easier to use and more popular

**`Internet Explorer (1995)`**
- Released several years after the first browser.

**`Opera`**	
- Opera appeared in the mid-1990s, after the first browser.

**`Chrome`**
- Chrome was released in 2008.

<img width="962" height="601" alt="image" src="https://github.com/user-attachments/assets/21926c34-77e0-4fcd-9ba0-f301612ceff0" />


Who created the first web browser, WorldWideWeb, in 1990?
- [ ] A. Bill Gates
- [x] B. Tim Berners-Lee
- [ ] C. Marc Andreessen
- [ ] D. Steve Jobs

Tim Berners-Lee created the first web browser, called WorldWideWeb, in 1990 while working at CERN.

Remember these important facts:
- 1990: WorldWideWeb - first web browser.
- 1993: Mosaic - an influential early graphical browser.
- 1995: Internet Explorer - released by Microsoft.
- 2008: Google Chrome - released by Google.

---

Q33. Which Search Algorithm Requiring the Least Memory?
- [ ] A. Optimal Search
- [x] B. Linear Search
- [ ] C. DFS
- [ ] D. BFS

| Algorithm	         | Typical memory consideration                          |
|--------------------|-------------------------------------------------------|
| **Linear Search**	 | `O(1)` auxiliary space in an iterative implementation |
| **DFS**	           | Often less memory than BFS in broad trees             |
| **BFS**	           | Can use substantial memory for the frontier           |
| **Optimal Search** | Depends on which algorithm "optimal search" refers to |

**1. Understand memory usage in search algorithms**

**A. Optimal Search** 
- "Optimal search" is not one specific algorithm with a fixed memory requirement. 
- In AI, optimal usually means that an algorithm finds a solution with the lowest cost. 
- For example, Uniform-Cost Search is optimal under suitable conditions, but it can require substantial memory.

**B. Linear Search**
- Linear search examines elements one by one in a list or array.
- Example: Find `7` in `[2, 4, 7, 9]`.
- It checks `2`, then `4`, then `7`.
- It uses `O(1)` auxiliary space when implemented iteratively.

**C. DFS: Depth-First Search**
- DFS explores one branch deeply before backtracking.
- DFS often uses less memory than BFS in a broad search tree because it stores the current path and some unexplored branches. However, its memory usage depends on the search representation and implementation.

<img width="547" height="397" alt="image" src="https://github.com/user-attachments/assets/618dab4e-11b8-40a0-a416-737527857d6e" />

**D. BFS: Breadth-First Search**
- BFS explores all nearby nodes before moving to deeper levels.
- It typically stores a large frontier of nodes, so it can use much more memory than DFS.


**Exam memory tip**
- **DFS** -> Go deep first; often memory-efficient compared with BFS.
- **BFS** -> Explore level by level; often memory-intensive.
- **Linear Search** -> Check items one by one; iterative version uses `O(1)` auxiliary space.
- **Optimal** -> Refers to solution quality, not automatically to low memory usage.

In a broad search tree, which algorithm generally requires more memory because it stores many nodes at the current frontier?
- [ ] A. DFS
- [x] B. BFS
- [ ] C. Linear Search
- [ ] D. None of the above

Correct! Option B. BFS (Breadth-First Search)

**Why is BFS more memory-intensive?**
- BFS explores a search tree level by level. <br/>
  It stores the nodes waiting to be explored in a queue.

For example, imagine a tree where every node has several children. <br/>
BFS must keep many nodes from the current level in memory before moving to the next level.  <br/>
This can require substantial memory.

DFS, on the other hand, explores one branch deeply before backtracking, so it often uses less memory in a broad search tree.


**DFS vs BFS**
| Feature	                          | DFS	                 | BFS                  |
|-----------------------------------|----------------------|----------------------|
| Full form	                        | Depth-First Search	 | Breadth-First Search |
| Exploration	                      | Deep into one branch |	Level by level      |
| Main data structure	              | Stack	               | Queue                |
| Typical memory use in broad trees	| Lower	               | Higher               |


Exam memory tip: 
- **BFS** uses a **`Queue`**; **DFS** uses a **`Stack`**.
- BFS often requires more memory than DFS when searching broad trees.

---

**Q34. Memory-Mapped I/O in a Microcontroller**

What is the primary role of the memory-mapped I/O technique in a microcontroller?
- [ ] A. It increases the speed of program execution
- [ ] B. It provides additional memory space for data storage
- [x] C. It allows external devices to access the microcontroller's memory
- [ ] D. It eliminates the need for I/O operations

Correct! Option C

**1. What is memory-mapped I/O?** <br/>
Memory-mapped I/O (Input/Output) is a technique in which hardware device registers are assigned addresses within the processor's memory address space.

This allows the CPU to communicate with peripherals by reading from or writing to specific addresses, much like it accesses memory.

Examples of peripherals include:
- Keyboard
- Timers
- Sensors
- Serial communication controllers

**2. How does it work?** <br/>
Imagine a microcontroller controlling an LED.

<img width="945" height="507" alt="image" src="https://github.com/user-attachments/assets/d658cc29-7aae-4500-a55b-eca5e01e2e8d" />

For example, writing a value to a particular device register can turn an LED on or off. <br/>
Reading a device register can provide sensor data.

The device registers are not ordinary RAM storage; accessing them triggers device-specific operations.


**3. Exam memory tip**

> **Memory-mapped I/O = Peripheral registers assigned memory addresses**.

This lets the CPU use ordinary memory-read and memory-write instructions to communicate with devices.


In memory-mapped I/O, where are peripheral device registers mapped?
- [ ] A. Only in the CPU's cache
- [x] B. Within the memory address space
- [ ] C. Only on the hard disk
- [ ] D. Outside the computer's address system

Correct! Option B. - Within memory address space.

In memory-mapped I/O, the registers of peripheral devices are assigned specific addresses within the microcontroller's memory address space.

This allows the CPU to communicate with devices using ordinary memory read and write instructions.

Example: A microcontroller controls an LED. A particular memory address is assigned to the LED's control register. The CPU writes a value to that address to turn the LED on or off.

---

| Operating Systems |
|-------------------|


Q.35 Context switching in an operating system refers to the process of:
- [ ] A. Switching between user and kernel modes
- [x] B. Switching between processes to allow multitasking
- [ ] C. Switching between different file systems
- [ ] D. Switching between different operating systems

Correct! Option B - Switching between processes to allow multitasking.

**1. What is context switching?**
An operating system (OS) allows multiple processes to share the CPU. <br/>
When the CPU stops working on one process and starts or resumes another, it performs a context switch.

The **`context`** is the information needed to resume a process, such as its **CPU register values, program counter, and other execution state**.

<img width="996" height="317" alt="image" src="https://github.com/user-attachments/assets/8b3f95ba-a296-4096-b80e-24f928668a30" />

**Example**: <br/>
You're listening to music while typing a document. The operating system switches CPU execution between processes so they can make progress. On a single CPU core, they take turns executing; this creates the impression that multiple tasks are running simultaneously.

**2. Exam memory tip**

Remember these distinctions:
- **Context switching**: Switching execution between `processes` or `threads`.
- **Mode switching**: Switching between `user mode` and `kernel mode`.
- **Multitasking**: Managing execution of multiple tasks over time.


Which information must the operating system preserve so that a paused process can resume correctly?
- [ ] A. Only the process's name
- [x] B. The process's execution state, including CPU registers and program counter
- [ ] C. Only the files stored on the hard disk
- [ ] D. Only the computer's IP address

Correct! Option B - The process's execution state, including CPU registers and program counter.

During a `context switch`, the operating system saves the current process's execution state so it can resume later from where it stopped.
- **CPU registers**: Hold values used during execution.
- **Program counter (PC)**: Keeps track of the next instruction to execute.
- **Process state**: Records whether the process is running, ready, or waiting.

Exam memory tip: 
> **Context switching = save the current state + restore the next process's state**.

---

**Question 36 - Digital Electronics**

The operating voltage range for TTL logic family?
- [ ] A. 1.8 V to 3.3 V
- [ ] B. 3.3 V to 5.0 V
- [x] C. 5.0 V to 12 V
- [ ] D. -5.0 V to 5.0 V


**TTL logic** <br/>
TTL stands for **Transistor-Transistor Logic**, a digital logic family traditionally associated with a nominal `5 V` power supply.

**Exam memory tip** <br/>
- TTL -> traditionally `5 V`. 
- Don't assume that a range extending to `12 V` is valid just because it includes 5 V.

What does TTL stand for?
- [x] A. Transistor-Transistor Logic
- [ ] B. Transfer Timing Logic
- [ ] C. Transistor Transfer Language
- [ ] D. Terminal Transmission Logic

Correct! Option A. Transistor-Transistor Logic

TTL is a digital logic technology traditionally associated with a **`5 V` supply voltage**.

- TTL: Transistor-Transistor Logic
- Traditional supply voltage: `5 V`
- Used in: Digital logic circuits

Exam memory tip: TTL -> Transistor-Transistor Logic → 5 V.

---

**Computer Networks**

Q.37 Communication over mobile phone is an example of which type of communication mode?
- [ ] A. Simplex
- [ ] B. Half-Duplex
- [x] C. Full-Duplex
- [ ] D. Double-Duplex


**1. What is communication mode?** <br/>
Communication modes describe the direction in which information travels between two devices or people.

**A. Simplex**
- Communication occurs in only one direction.
- Example: `Traditional radio broadcasting` - the station transmits to listeners.

<img width="402" height="287" alt="image" src="https://github.com/user-attachments/assets/90cdcdc7-08e3-45db-9960-503318e452eb" />

**B. Half-Duplex**
- Both sides can communicate, but not simultaneously.
- Example: `Walkie-talkies`.

<img width="456" height="257" alt="image" src="https://github.com/user-attachments/assets/8e8c2a5c-697d-4f41-97b4-aca988574128" />

**C. Full-Duplex**
- Both sides can send and receive information at the same time.
- Example: A normal `mobile phone call`.

<img width="920" height="760" alt="image" src="https://github.com/user-attachments/assets/3d9cde1d-d793-4a8c-ac6d-39346dbc1c74" />


> ~~Double-Duplex~~: This is not the standard communication-mode term.

**2. Why is a mobile phone call full-duplex?** <br/>
Imagine you're speaking with a friend on the phone. <br/>
You can hear your friend while speaking, and your friend can hear you at the same time.

That simultaneous, two-way communication is `full-duplex`.

| Mode	          | Direction	             | Example         |
|-----------------|------------------------|-----------------|
| **Simplex**	    | One-way only	         | Radio broadcast |
| **Half-duplex** | Two-way, one at a time | Walkie-talkie   |
| **Full-duplex**	| Two-way simultaneously | Phone call      |

Two people use walkie-talkies. One person must press a button and speak, then release it so the other person can respond. <br/>
Which communication mode is this?
- [ ] A. Simplex
- [x] B. Half-Duplex
- [ ] C. Full-Duplex
- [ ] D. Double-Duplex

---

**Artificial Intelligence**

Q.38 The advantage of using an expert system development tool is ___________?
- [ ] A. Imposed structure
- [ ] B. Knowledge engineering assistance
- [ ] C. Rapid prototyping
- [x] D. All of the mentioned

Correct! Option D - All of the mentioned.

**1. Expert system development tools** <br/>
An expert system is an AI program that uses stored knowledge and rules to solve problems in a specific domain, similar to how a human expert would approach them.

For example, a medical expert system might use rules and medical knowledge to help identify possible diseases based on symptoms.

**2. Simple example** <br/>
Suppose you're building an expert system to identify plant diseases.
- **Imposed structure**: The tool organizes rules and knowledge in a defined format.
- **Knowledge engineering assistance**: It helps you encode an expert's knowledge, such as symptoms and disease rules.
- **Rapid prototyping**: You can quickly build a basic version and test it with sample symptoms.
These features can make development more organized and efficient.

Which component of an expert system stores facts and rules about a particular domain?
- [ ] A. User interface
- [x] B. Knowledge base
- [ ] C. Keyboard
- [ ] D. Operating system

Correct! Option B - Knowledge base.

The **knowledge base** stores the facts, rules, and domain-specific knowledge that an expert system uses to solve problems.

For example, a plant-disease expert system might contain this rule:
> IF a plant has yellow leaves AND wilting, THEN check for possible root problems.

The system uses its knowledge base to help reach a conclusion.

- **Knowledge base**:  `what the system knows`; Stores facts and rules.
- **Inference engine**: `how the system`; Applies rules to available facts to draw conclusions.
- **User interface**: Allows users to interact with the system.

---

**Python Programming**

Q.39 Following given below and then choose the correct output from the given options
```py
def Change(N):
    N = N + 10
    print(N, end='$$ ')

N = 15
Change(N)  # 25$$ 
print(N)   # 15

"""
The variable N outside the function has the value 15.
"""
```
- [x] A. 25$$15
- [ ] B. 15$$25
- [ ] C. 25$$25
- [ ] D. 2525$$

> **Reassigning a local variable inside a function does not reassign the outside variable.**

What will this code print?
```py
def update(x):
    x = x + 5
    print(x)

a = 10
update(a)  # 15
print(a)   # 10
```

---

Q.40 _________________ is two dimensional data structure in Python with row index and column index.
- [x] A. DataFrame
- [ ] B. List
- [ ] C. Tuple
- [ ] D. Series

Correct! Option A. - DataFrame.

**1. What is a DataFrame?** <br/>
A DataFrame is a two-dimensional, tabular data structure in the Python pandas library. <br/>
It organizes data into rows and columns, with `row` and `column` labels.

For example, imagine storing student marks:

**Student Marks DataFrame**
| Index	| Name  | Marks |
|-------|-------|-------|
| 0	    | Neha  | 85    |
| 1	    | Rahul | 92    |
| 2	    | Priya	| 78    |

Rows have indexes; columns have labels such as Name and Marks.

We can create a DataFrame like this:
```py
import pandas as pd

data = {
    "Name": ["Neha", "Rahul", "Priya"],
    "Marks": [85, 92, 78]
}

df = pd.DataFrame(data)
print(df)
```

| Option	      | Explanation                                       |
|---------------|---------------------------------------------------|
| **DataFrame**	| A two-dimensional structure with rows and columns.|
| **List**	    | A list stores an ordered collection of items. Nested lists can represent rows and columns, but a list itself does not provide the DataFrame's labeled tabular structure. |
| **Tuple**	    | A tuple is an ordered, immutable collection. It is not the standard pandas two-dimensional tabular structure. |      
| **Series**	  | A pandas Series is a one-dimensional labeled array. |

**2. Exam memory tip**, Remember the difference:
- **Series** -> One-dimensional
- **DataFrame** -> Two-dimensional
- **Tuple** -> Ordered, immutable collection
- **List** -> Ordered, mutable collection


In pandas, which data structure is one-dimensional and contains labeled data?
- [ ] A. DataFrame
- [x] B. Series
- [ ] C. Dictionary
- [ ] D. Matrix

Correct! Option B. - Series

A **pandas Series** is a one-dimensional labeled data structure. <br/>
It stores values with an associated index.

Example:
```py
import pandas as pd

marks = pd.Series([85, 92, 78])
print(marks)

# OUTPUT
"""
0    85
1    92
2    78

Here, 0, 1, and 2 are the index labels, and 85, 92, and 78 are the values.
"""
```

**Quick revision**
| Structure	| Dimension	| Example use                        |
|-----------|-----------|------------------------------------|
| Series	  | 1D	      | Marks in one subject               |
| DataFrame	| 2D	      | Student names and marks in a table |

---

Q.41 What is the output of the following expression?
```py
Sports = "Paralympic Games"
print(Sports.split("m"))
```
- [ ] A. `[ ' Paraly ' , 'm' , 'pic Ga', 'm', ' es']`
- [ ] B. `('Paraly', 'm', 'pic Games')`
- [ ] C. `('Paraly', 'pic Ga', 'es')`
- [x] D. `[ 'Paraly', 'pic Ga', 'es']`

Python `splits` the string wherever the lowercase letter "m" occurs. <br/>
It removes the separator from the resulting pieces.

Exam memory tip
- `string.split("m")` -> splits at lowercase m.
- The separator is removed.
- `split()` returns a list.
- Python is case-sensitive: `.split()` works; `.Split()` does not.

What is the output of this code?
```py
word = "banana"
print(word.split("a"))
```
- [x] A. `['b', 'n', 'n']`
- [ ] B. `['b', 'n', 'n', '']`
- [ ] C. `['ba', 'na', 'na']`
- [ ] D. `['banana']`
  
---

**Question 42 - Theory of Computation**


---

**Computer Fundamentals**

Q.43 A photograph is an analog image and a ___ can convert it into a digital image.
- [ ] A. Printer
- [x] B. Scanner
- [ ] C. Webcam
- [ ] D. Camera

Correct: Option B. Scanner

A **photograph** is an analog image when it exists as a physical printed picture.

A **scanner** converts that printed photograph into a digital image that can be stored on a computer.

<img width="997" height="382" alt="image" src="https://github.com/user-attachments/assets/17742915-4b44-48b5-b440-0f3b55792aa5" />

A scanner captures the image and converts it into digital data, allowing you to save it as a file such as `JPEG` or `PNG`.

| Device	    | Why it is?                                                                           |
|-------------|--------------------------------------------------------------------------------------|
| **Printer**	| Produces a physical copy from digital content.                                       |
| **Scanner** | Converts a printed photograph into a digital file.                                   |
| **Webcam**	| Captures live images or video, usually of people or surroundings.                    |
| **Camera**	| Captures photographs directly, rather than scanning an existing printed photograph.  |

Exam memory tip: **Scanner = paper to digital; Printer = digital to paper**.

Which device is commonly used to convert a handwritten page into a digital image on a computer?
- [ ] A. Printer
- [x] B. Scanner
- [ ] C. Speaker
- [ ] D. Projector

Correct! Option B. Scanner

A scanner converts a handwritten page or printed document into a digital image that can be stored on a computer.

Remember:
- **Scanner**: Paper -> Digital
- **Printer**: Digital -> Paper

---

Q 44. Complexity Theory - NP(Nondeterministic Polynomial Time)

Question: A problem is said to be in NP if:
- [ ] A. Its solution can be verified in polynomial time
- [x] B. It can be solved using a non-deterministic algorithm
- [ ] C. It is not solvable
- [ ] D. It has exponential complexity


**What is NP?** <br/>
NP stands for **Nondeterministic Polynomial** Time.

In computational complexity, NP is the class of decision problems for which a proposed solution can be verified in polynomial time.

Think of it this way: <br/>
Suppose someone gives you a completed Sudoku puzzle. Checking whether the solution follows the rules is relatively easy compared with solving the puzzle from scratch.
- **Finding a solution**: May require substantial work.
- **Verifying a proposed solution**: Can be done efficiently.
That is the central idea behind the verification characterization of NP.


Exam memory tip
- **P**: Solutions can be found in polynomial time by a deterministic algorithm.
- **NP**: Solutions can be verified in polynomial time.
- **NP-hard**: At least as hard as every problem in NP.
- **NP-complete**: Both in NP and NP-hard.


Which of the following is the best description of P in computational complexity?
- [ ] A. Problems that cannot be solved by computers
- [x] B. Problems solvable in polynomial time by a deterministic algorithm
- [ ] C. Problems that always require exponential time
- [ ] D. Problems whose solutions cannot be verified

Correct! Otion B. Problems solvable in polynomial time by a deterministic algorithm.

Class P contains decision problems that can be solved in polynomial time using a deterministic algorithm.

For example, checking whether a number appears in a sorted array using binary search takes `O(log n)` time, which is polynomial time.

Remember for the exam:
- **P**: Efficiently solvable.
- **NP**: Proposed solutions are efficiently verifiable.
  
---

**Q45. Computer Networks - Email Protocols**

Which protocol is used to send e-mails is _________?
- [ ] A. HTTP
- [ ] B. POP
- [x] C. SMTP
- [ ] D. FTP

**What is SMTP?** <br>
SMTP stands for **Simple Mail Transfer Protocol**.

It is used to send outgoing emails from an email client to a mail server and to transfer emails between mail servers.

For example, when you compose an email in Gmail and click Send, SMTP is involved in sending that message.

<img width="966" height="467" alt="image" src="https://github.com/user-attachments/assets/92528b76-3b6e-425b-af7e-8fab3fb2d1db" />

|       | Full form/purpose	            | Why                                                          |
|-------|-------------------------------|--------------------------------------------------------------|
| HTTP	| Hypertext                     | Transfer Protocol	Transfers web resources, such as webpages. |
| POP	  | Post Office Protocol          | Retrieves or downloads emails from a mail server.            |
| SMTP	| Simple Mail Transfer Protocol | Used to send emails.                                         |
| FTP	  | File Transfer Protocol	      | Transfers files between computers.                           |

Exam memory tip, Remember this simple distinction:
- **SMTP** -> Send email
- **POP3** -> Retrieve/download email
- **HTTP/HTTPS** -> Access web resources
- **FTP** -> Transfer files

Which protocol is commonly used to retrieve emails from a mail server?
- [ ] A. SMTP
- [x] B. POP3
- [ ] C. FTP
- [ ] D. HTTP

Correct! Option B. POP3.

- **SMTP** sends outgoing emails.
- **POP3** retrieves emails from a mail server, often by downloading them to your device.

For example, when you send an email, SMTP helps send it. When your email application downloads messages from a mail server using POP3, POP3 handles retrieval.

---

**Q46. Object-Oriented Programming - Method Overloading**

Question: In OOP, what is method overloading?
- [ ] A. Creating multiple constructors
- [ ] B. Using multiple inheritance
- [x] C. Defining multiple methods with the same name but different parameters
- [ ] D. Inheriting multiple methods from a parent class

**1. What is method overloading?** <br/>
Method overloading is an OOP concept in which multiple methods have the same name but different parameter lists.

The methods can differ in their:
- Number of parameters
- Types of parameters
- Order of parameter types

For example, imagine a calculator that adds numbers.
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
Here, all three methods are named `add`, but their parameters differ.
- `add(2, 3)` `returns 5`.
- `add(2, 3, 4)` `returns 9`.
- `add(2.5, 3.5)` `returns 6.0`.
The compiler selects the appropriate method based on the arguments. <br/>
This is called **compile-time polymorphism** in Java.

- Creating multiple constructors: 	This is related to constructor overloading, a specific kind of overloading, but it does not define method overloading generally.

- Using multiple inheritance:	This refers to inheriting from multiple parent classes, not defining methods with the same name and different parameters.

- Inheriting multiple methods from a parent class: This describes inheritance, not method overloading.

Exam memory tip
- **Overloading**: Same name, different parameters.
- **Overriding**: A subclass provides a new implementation of an inherited method with a compatible signature.

> Remember: Overloading = different parameter lists.

Which example demonstrates method overloading in Java?
- [ ] A. Two methods named `show()` with identical parameters but different return types only.
- [x] B. Two methods named `display(int x)` and `display(String x)`.
- [ ] C. A subclass inherits a method without changing it.
- [ ] D. A class creates an object using `new`.

Correct! B. Two methods named `display(int x)` and `display(String x)`

Both methods have the same name, `display()`, but accept different parameter types
```java
void display(int x) {
    System.out.println(x);
}

void display(String x) {
    System.out.println(x);
}
```
The compiler can distinguish them based on the argument supplied.
- `display(10)` calls the integer version.
- `display("Hello")` calls the string version.
That is **method overloading**.

---

**Q47. Cryptography**

Question: Private Key cryptography is also known as ____________ cryptography.
- [ ] A. Private key
- [ ] B. Public key
- [x] C. Symmetric key
- [ ] D. Asymmetric key

Correct answer: C. Symmetric key

**1. What is private-key cryptography?** <br/>
**Private-key cryptography** is another name for **symmetric-key cryptography**.

In symmetric encryption, the sender and receiver use the same secret key to encrypt and decrypt information.

<img width="881" height="725" alt="image" src="https://github.com/user-attachments/assets/375af78b-87b3-4e09-bcc6-b5856cfe8a5b" />

Examples of symmetric encryption algorithms include `AES` and `DES`.


**2. Symmetric(Private) vs. asymmetric(Public) cryptography**

| Feature	                  | Symmetric key	        | Asymmetric key                                      |
|---------------------------|-----------------------|-----------------------------------------------------|
| Keys used	                | One shared secret key	| Public and private key pair                         |
| Encryption and decryption	| Same key	            | Different keys, depending on the operation          |
| Key                       | sharing	Secret key must be shared securely | Public key can be shared openly|
| Examples	                | AES, DES	            | RSA, ECC                                            |

Exam memory tip: 
- **Symmetric = same key**
- **Asymmetric = two related keys**.

Alice encrypts a message using a secret key and shares that key securely with Bob. Bob uses the same key to decrypt the message. Which type of cryptography is this?
- [ ] A. Asymmetric cryptography
- [x] B. Symmetric cryptography
- [ ] C. Hashing
- [ ] D. Digital signatures

Correct! Option B. Symmetric cryptography.

- **Symmetric**: Same shared secret key.

- **Asymmetric**: Public key and private key pair.

- **Hashing**: Produces a hash value; it is not ordinary reversible encryption.

- **Digital signatures**: Help verify authenticity and integrity.

---

**Q48. Software Maintenance**

Question: Process model focuses on fixing defects as they are identified?
- [ ] A. Waterfall Model
- [x] B. Corrective Maintenance
- [ ] C. Perfective Maintenance
- [ ] D. Adaptive Maintenance

Correct! Option B. Corrective Maintenance

**1. What is corrective maintenance?** <br/>
**Corrective maintenance** means _modifying software to fix defects, bugs, or errors discovered after the software_ has been delivered or put into use.

Example <br/>
Imagine a school management system where the fee calculator incorrectly adds ₹500 instead of ₹5,000.

A developer identifies the bug and fixes the calculation. This is corrective maintenance.

| Term                       | Meaning	                                                     | Example          |
|----------------------------|---------------------------------------------------------------|------------------|
| **Waterfall Model**        | A sequential software development model with distinct phases. | Requirements -> Design -> Coding -> Testing |
| **Corrective Maintenance** | Fixes existing defects or bugs.	| Fixing an incorrect fee calculation. |
| **Perfective Maintenance** | Improves performance, usability, or functionality.	 | Making a report load faster.|
| **Adaptive Maintenance**	 | Modifies software to work in a changed environment. | Updating software to support a new operating system. |

**3. Exam memory tip**
Remember the three major types of software maintenance:
- **Corrective** = Correct a bug
- **Perfective** = Improve the software
- **Adaptive** = Adapt to changes in the environment

One useful distinction: c**orrective maintenance addresses defects**, while **perfective maintenance improves software that is already functioning**.

A company updates its software so that it works correctly with a newly released version of Windows. Which type of maintenance is this?
- [ ] A. Corrective maintenance
- [ ] B. Perfective maintenance
- [x] C. Adaptive maintenance
- [ ] D. Preventive maintenance

Correct! Option C. Adaptive maintenance.

The software is being modified to work with a new version of Windows, which is a change in its operating environment.

Quick revision:
- **Corrective**: Fix a bug.
- **Perfective**: Improve performance or add enhancements.
- **Adaptive**: Adjust to a changed environment.
- **Preventive**: Reduce the likelihood of future problems.

> Exam memory tip: **New environment -> Adaptive maintenance**.

---

**Q49. HTML Attributes**

Question: Which of the following attributes is not a valid attribute of the tag in HTML?
- [ ] A. face
- [ ] B. type
- [ ] C. size
- [x] D. colour

**1. Understanding HTML attributes** <br/>
**HTML attributes** provide additional information about an HTML element. 

For example:
```html
<font face="Arial">Hello</font>
<input type="text">
<input size="20">
```

- `face` was a valid attribute of the older `<font>` tag.
- `type` is a valid attribute of elements such as `<input>`.
- `size` is valid for elements such as `<input>` and `<select>`.
- `colour` is not a standard HTML attribute. Color is usually specified through CSS, for example, `color: red;`. Not a standard HTML attribute; CSS uses the property `color`

Which of the following is a valid CSS property for changing text color?
- [ ] A. `font-color`
- [ ] B. `text-colour`
- [x] C. `color`
- [ ] D. `text-style-color`

Correct! Option C. `color`

In CSS, the `color` property changes the color of text.
Example:
```html
p {
    color: red;
}
```
This makes the paragraph text red.

Remember the distinction:
- `color` -> CSS property for text color.
- `background-color` -> CSS property for background color.
- `colour` -> Not the standard CSS property spelling.

Exam memory tip: CSS uses American spelling: `color`, not `colour`.

---

**Question 50: Image Processing**

Q50. Which of the following is the first and foremost step in Image Processing?
- [x] B. Segmentation
- [ ] C. Image enhancement
- [ ] D. Image restoration

Correct! A. Image acquisition

**Image Processing** <br/>
`Image processing` means using a computer to perform operations on an image **to improve it, extract useful information, or analyze its contents**.

The first step is generally image acquisition - obtaining the image and converting it into a digital form that a computer can process.

For example, imagine you want a computer to identify cats in photographs.

**Step 1: Image acquisition** <br/>
Capture the photograph using a camera or scanner.

**Step 2: Image enhancement** <br/>
Improve brightness, contrast, or image quality if needed.

**Step 3: Image segmentation** <br/>
Separate the cat from the background.

**Image restoration** may also be performed to reduce blur, noise, or other image degradation. 

The exact order of later operations depends on the application, but acquisition is the starting point in the standard introductory workflow.

<img width="976" height="472" alt="image" src="https://github.com/user-attachments/assets/2c7dbca4-487f-435c-ab55-0436ea07089f" />

| Term                  | Meaning	                                             | Why                            |
|-----------------------|------------------------------------------------------|--------------------------------|
| **Segmentation**	    | Dividing an image into meaningful regions or objects | Usually performed after the image has been acquired. |
| **Image enhancement**	| Improving the visual quality of an image	| Requires an image to work on first. |
| **Image restoration**	| Recovering an image degraded by blur, noise, or distortion | Also operates on an already acquired image. |

**Exam memory tip, Remember this distinction:**
- **Acquisition** = Get the image.
- **Enhancement** = Improve the image.
- **Restoration** = Recover degraded image quality.
- **Segmentation** = Separate objects or regions.

A computer receives a photograph and needs to separate a person from the background. Which image-processing operation is most directly responsible?
- [ ] A. Image acquisition
- [ ] B. Image restoration
- [x] C. Image segmentation
- [ ] D. Image compression

Correct! C. Image segmentation

**Image segmentation** divides an image into meaningful regions or objects. 
For example, it can separate a person from the background in a photograph.
- **Image acquisition**: Captures or obtains the image.
- **Image restoration**: Reduces degradation such as blur or noise.
- **Image segmentation**: Separates the person from the background.
- **Image compression**: Reduces the amount of storage needed for an image.

Exam memory tip: **Segmentation = separating objects or regions**.

---

Q51. Full form of TCP in TCP/IP?
- [x] A. Transmission Control Protocol
- [ ] B. Transmission Central Protocol
- [ ] C. Transfer Control Protocol
- [ ] D. Transport Central Protocol

Correct! A. Transmission Control Protocol

**1. Understand TCP/IP** <br/>
TCP stands for **Transmission Control Protocol**.

TCP/IP is a collection of communication protocols that computers use to communicate over networks, including the internet.

Think of sending a message from your computer to another computer. TCP helps ensure that data arrives reliably and in the correct order.

For example, when a message is divided into multiple pieces during transmission, TCP helps the receiving computer reassemble those pieces in the correct order and detect missing data so it can be retransmitted when necessary.

**2. Important exam concepts**
- **TCP**: Transmission Control Protocol - reliable, connection-oriented communication.

- **IP**: Internet Protocol - addressing and routing packets between networks.

- **UDP**: User Datagram Protocol - connectionless communication with lower overhead, but without TCP's built-in delivery guarantees.

Which statement about TCP is correct?
- [ ] A. TCP is used only to assign IP addresses.
- [x] B. TCP provides reliable, ordered delivery of data.
- [ ] C. TCP is a programming language.
- [ ] D. TCP is used only for transferring files.

Correct! B. TCP provides reliable, ordered delivery of data.

TCP tracks transmitted data, detects missing segments, supports retransmission, and reassembles data in the correct order at the receiving end.
- **IP addressing** is associated with the Internet Protocol, not TCP alone.
- **TCP** is a communication protocol, not a programming language.
- **TCP** supports many applications, including web browsing, email, and file transfers; it isn't limited to file transfers.

> Exam memory tip: **TCP = reliable delivery;** **IP = addressing and routing**.

---

Question 52: **Operating Systems**

Q52. The kernel operates in a privileged mode, also known as:
- [ ] A. User mode
- [ ] B. Debug mode
- [x] C. Supervisor mode
- [ ] D. Interrupt mode

Correct! C. Supervisor mode

**1. Kernel** <br/>
The `kernel` is the core part of an operating system. <br/>
It manages hardware resources, memory, processes, and communication between software and hardware.

To protect the computer, operating systems commonly use two privilege levels:
- **`User mode`**: Applications run with restricted permissions.
- **`Kernel mode/Supervisor mode`**: The operating system kernel can execute privileged operations, such as controlling hardware and managing memory.
  
For example, when a music player needs to read a file from storage, it requests the operating system to perform the operation. The kernel handles the request using its privileged access.

<img width="982" height="352" alt="image" src="https://github.com/user-attachments/assets/e9529390-7359-4ecb-a034-e13dfbafce37" />


| Term                | Explanation                                                                                |
|---------------------|--------------------------------------------------------------------------------------------|
| **User mode**	      | Restricted mode intended for ordinary applications.                                        |
| **Debug mode**	    | A mode or facility used for debugging; not the standard name for kernel's privileged mode. |
| **Supervisor mode**	| A common name for the privileged execution mode i.e. Kernel mode.                          |
| **Interrupt mode**	| Not the standard name for the kernel's privileged mode. Interrupts are events that may cause the CPU to transfer control to a handler. |


> Exam memory tip: **Kernel = privileged access; applications = restricted access**.

What is the primary purpose of user mode in an operating system?
- [ ] A. To allow every application unrestricted hardware access
- [x] B. To protect the system by restricting application privileges
- [ ] C. To replace the operating system kernel
- [ ] D. To disable memory management

Correct! B. To protect the system by restricting application privileges.

User mode limits what ordinary applications can do directly. When an application needs a privileged operation, such as accessing hardware, it requests the operating system kernel to perform it.

- Unrestricted hardware access would compromise system security.
- restricted privileges help protect the operating system and other applications.
- User mode does not replace the kernel.
- Memory management remains an important operating-system responsibility.

---

Question 53 - Inode in a Unix-like File System

Q.53 The "inode" in a Unix-like file system is used to:
- [ ] A. Store the contents of the file
- [ ] B. Store the file's name and location
- [x] C. Store the attributes and metadata of the file
- [ ] D. Store the directory structure of the file system

**1. What an inode is?** <br/>
In a Unix-like operating system, an `inode` is a data structure that stores information about a file, rather than the file's actual contents.

An inode typically stores:
- File type and permissions
- Owner and group IDs
- File size
- Timestamps
- Pointers or references to the blocks containing the file's data

For example, imagine a file called `notes.txt`.
| Information    	            | Where it is generally stored |
|-----------------------------|------------------------------|
| File name: `notes.txt`      |	Directory entry              |
| File size: 2 KB	            | Inode metadata               |
| File permissions            | Inode metadata               |
| Actual text inside the file	| Data blocks                  |

Important distinction: 
> The directory entry associates the filename with an inode number. The inode itself generally does not store the filename.

- The actual contents are stored in data blocks, not directly inside the inode.
- The filename is stored in a directory entry. The inode identifies metadata and references to data blocks.
- **Store the attributes and metadata** This includes permissions, ownership, size, and timestamps.
- Directories contain entries mapping names to inode numbers. The overall directory structure is not the inode's primary purpose.

**Exam memory tip, Remember this distinction:**
- **Inode** -> Information about the file
- **Directory entry** -> Filename and inode number
- **Data blocks** -> Actual file contents

A file has the name `report.pdf`, a size of `5 MB`, and read-only permissions. Which information is typically stored in its inode?
- [ ] A. Only the filename
- [ ] B. The PDF's actual contents
- [x] C. The file size and permissions
- [ ] D. The entire directory tree

Correct! C. The file size and permissions.

The inode stores metadata such as file size, permissions, ownership, and timestamps. 

The actual PDF contents are stored in data blocks, while the filename is generally stored in a directory entry.

> Remember: **Inode = file information, not file contents**.

---

Question 54 - File Operations in an Operating System

Operations in an operating system include:
- [ ] A. Allocating memory to files
- [ ] B. Assigning file names to processes
- [ ] C. Loading files into CPU registers
- [x] D. Reading, writing, and modifying file content

**1. Concept: File operations in an operating system** <br/>
An operating system (OS) manages files and provides operations that let programs and users work with them.

Common file operations include:
- `Read`: Retrieve data from a file.
- `Write`: Store data in a file.
- `Create`: Make a new file.
- `Delete`: Remove a file.
- `Modify`: Change existing file content.

For example, when you open a text file, type a new sentence, and save it, the operating system helps perform these file operations.

**CRUD** for four fundamental data operations:
- **C - Create**
- **R - Read**
- **U - Update**
- **D - Delete**
These are also widely used in databases and applications.

Which operating system operation retrieves existing data from a file without changing its contents?
- [ ] A. Write
- [x] B. Read
- [ ] C. Delete
- [ ] D. Rename

Correct! B. Read

The read operation retrieves existing data from a file without changing its contents.
- **Read**: Retrieves data.
- **Write**: Stores or changes data.
- **Delete**: Removes a file.
- **Rename**: Changes a file's name.

> Remember: **Read = get data; Write = save data**.

---

Question 55 - HTTP

The term HTTP stands for:
- [ ] A. Hyper Terminal Tracing Program
- [ ] B. Hypertext Tracing Program
- [x] C. Hypertext Transfer Protocol
- [ ] D. Hypertext Tracing Protocol

Correct! Option C. - Hypertext Transfer Protocol.

`HTTP` stands for Hypertext Transfer Protocol. <br/>
It is a protocol used for communication between a web browser (client) and a web server.

For example, when you open a website in your browser, HTTP defines how the browser requests web resources and how the server responds.

- **`HTTP`** - transfers web resources such as HTML pages.
- **`HTTPS`** - HTTP secured using encryption, typically through TLS.

Which protocol is the secure version of HTTP?
- [ ] A. FTP
- [x] B. HTTPS
- [ ] C. SMTP
- [ ] D. POP3

Correct! Option B - HTTPS.

**HTTPS** <br/>
- HTTPS stands for Hypertext Transfer Protocol Secure. 
- It is the secure version of HTTP and uses TLS encryption to protect data exchanged between your browser and a website.

For example, when you enter your password on a website using HTTPS, encryption helps protect it while it travels across the network.

| Protocol	| Main purpose                               |
|-----------|--------------------------------------------|
| HTTP	    | Transfers web resources                    |
| HTTPS	    | Transfers web resources securely using TLS |
| FTP	      | Transfers files                            |
| SMTP	    | Sends emails                               |
| POP3	    | Retrieves emails                           |

---

Question 56 - Secure Remote Login

Which of the following protocols is used for secure remote login?
- [ ] A. FTP
- [ ] B. HTTPS
- [ ] C. TELNET
- [ ] D. HTTP
- [x] E. SSH


**SSH = Secure Shell**
- When you want to log in to another computer over a network and control it remotely, `SSH` is the standard protocol.
- It encrypts the communication between your computer and the remote computer.

| Protocol   | Main purpose                                    |
| **FTP**	   | Transfers files                                 |
| **HTTPS**	 | Secure communication with websites              |
| **TELNET** | Remote login, but without encryption by default |
| **HTTP**	 | Transfers web resources                         |


- **SSH** -> Secure remote login
- **TELNET** -> Unencrypted remote login
- **HTTPS** -> Secure web browsing
- **FTP** -> File transfer

Which protocol is specifically designed for secure remote access to another computer's command line?
- [ ] A. HTTP
- [x] B. SSH
- [ ] C. FTP
- [ ] D. TELNET

Correct! Option B - SSH (Secure Shell).

**SSH** <br/>
**SSH (Secure Shell)** is a network protocol that lets you securely access and control a remote computer through a command-line interface.

For example, if you connect to a remote Linux server to run commands, you commonly use SSH:
```
ssh username@server_ip
```

> **SSH encrypts the communication, helping protect login credentials and data from interception.**

> **SSH = Secure Shell = Secure remote login**

| Protocol	| Main purpose	            | Security                 |
|-----------|---------------------------|--------------------------|
| SSH	      | Secure remote login	      | Encrypted                |
| TELNET	  | Remote login	            | Unencrypted by default   |
| HTTPS	    | Secure web communication	| Encrypted using TLS      |
| FTP	      | File transfer	            | Not encrypted by default |

---

Question 57 - Software Development Life Cycle

Which software life cycle model is based on iterative prototyping?
- [ ] A. Waterfall Model
- [ ] B. Spiral Model
- [ ] C. Agile Model
- [x] D. Prototype Model

**1. Understand the Prototype Model**

A prototype is an early, working or illustrative version of software created to understand what users need.

Imagine you're building a school website:
1. Create a basic sample website.
2. Show it to teachers and students.
3. Collect their feedback.
4. Improve the design and features.
5. Repeat until the requirements are clear.

<img width="897" height="422" alt="image" src="https://github.com/user-attachments/assets/2dc7918e-5396-4eea-b2de-fa692b4d004f" />

| Model	        | Key idea                                                         |
|---------------|------------------------------------------------------------------|
| **Waterfall**	| Sequential phases, generally completed one after another         |
| **Spiral**	  | Repeated development cycles with a strong focus on risk analysis |
| **Agile**	    | Iterative, incremental development with frequent feedback        |
| **Prototype**	| Build and refine an early version to clarify requirements        |

Exam memory tip:
- **Prototype** -> Build a sample and get feedback.
- **Spiral** -> Focus on risk analysis in repeated cycles.
- **Waterfall** -> Follow sequential phases.
- **Agile** -> Deliver software incrementally.

A software team builds a sample application screen, shows it to the client, and repeatedly changes it based on feedback before developing the final system. Which model does this best describe?
- [ ] A. Waterfall Model
- [x] B. Prototype Model
- [ ] C. Spiral Model
- [ ] D. V-Model

Correct! Option B. - Prototype Model.

The Prototype Model involves creating an early version of the software, collecting feedback from users, and improving the prototype until the requirements are understood.

Example: A team creates a sample school website, shows it to teachers, changes the layout based on their feedback, and repeats the process before developing the final website.

> **If the question emphasizes building a sample, showing it to users, and refining it, think Prototype Model**.

---

**Question 58 - Secure Software Development**

What is the primary purpose of Software Requirements Specification (SRS) documents?
- [ ] A. To list the programming languages used
- [ ] B. To describe the user interface design
- [x] C. To define the software’s functional and non-functional requirements
- [ ] D. To specify the hardware components required

Correct! C. - To define the software’s functional and non-functional requirements.

**1. What is an SRS document?**

- SRS stands for **Software Requirements Specification**.

- It is a document that describes what a software system must do and the conditions under which it must operate.

Think of it as a blueprint for software development. Before developers build an application, they need to understand what the client expects.

Example: **School Management System** <br/>
Suppose you're developing a school management system.
| Requirement type	          | Example                                          |
|-----------------------------|--------------------------------------------------|
| Functional requirement	    | Teachers can enter students' marks.              |
| Functional requirement	    | Students can view their results.                 |
| Non-functional requirement	| Results should load within two seconds.          |
| Non-functional requirement	| Only authorized users can access student records.|

`Functional requirements` describe **what the system does**. <br/>
`Non-functional requirements` describe **qualities or constraints, such as performance, security, and reliability**.

> **SRS = What the software must do and how well it must do it.**


A school application must allow students to check their marks and load each result page within two seconds. <br/>
Which option correctly identifies these requirements?
- [ ] A. Both are functional requirements.
- [ ] B. Both are non-functional requirements.
- [x] C. Checking marks is functional; the two-second limit is non-functional.
- [ ] D. Checking marks is non-functional; the two-second limit is functional.

Correct! C.
- Checking marks is a functional requirement because it describes an action the application must perform.
- Loading results within two seconds is a non-functional requirement because it specifies a performance standard the application must meet.

| Functional	                   | Non-functional                                     |
|--------------------------------|----------------------------------------------------|
| What the system does	         | How well the system works                          |
| Students can log in. 	         | Login completes within two seconds.                |
| Teachers can enter marks.	     | The system supports 1,000 concurrent users.        |
| Students can download results. | Student data is protected from unauthorized access.|

Ask yourself:
> **"What does it do?” -> Functional**. 

> **"How well or under what constraints does it work?" -> Non-functional**.

---

**Question 59 — Object-Oriented Programming (OOP)**

What is encapsulation in OOP?
- [ ] A. The ability to inherit properties from multiple classes
- [ ] B. The process of creating objects
- [x] C. The bundling of data and methods that operate on the data
- [ ] D. The use of abstract classes only

Correct! Option C. - The bundling of data and methods that operate on the data

**1. What is encapsulation?** <br/>

**Encapsulation** is an OOP concept that combines data (variables) and the methods (functions) that work on that data into a single unit, usually a class.  <br/>
It also helps control access to an object's internal data.

Think of a bank account. You can deposit or withdraw money, but you shouldn't be able to change the balance directly without following the bank's rules.

Example in Java
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
```
Let's understand the important parts:
- `balance` stores the account's data.
- `private` restricts direct access to `balance` from outside the class.
- `deposit()` provides a controlled way to modify the balance.
- `getBalance()` allows the balance to be read.
This Encapsulation protects the data from invalid changes.


| Term                                      | Concept	    | Explanation                             |
|-------------------------------------------|-------------|-----------------------------------------|
| Inherit properties from multiple classes	| **Inheritance**	| Inheritance allows a class to acquire features from another class. |
| Process of creating objects	              | **Object creation**	| Creating an instance of a class is called instantiation. |
| Bundling data and methods	                | **Encapsulation** | It combines data and related methods while controlling access.
| Use of abstract classes only	            | **Abstraction**	 | Abstraction focuses on exposing essential features while hiding implementation details. <br/> It doesn't require abstract classes exclusively. |

Remember these four OOP concepts:
- **Encapsulation** -> Bundle and protect data.
- **Inheritance** -> Reuse features from another class.
- **Polymorphism** -> One interface, different behaviors.
- **Abstraction** -> Hide implementation details.

In the Java example above, why is `balance` declared private?
- [ ] A. To allow every class to change it directly
- [x] B. To prevent direct access from outside the class
- [ ] C. To make the variable constant forever
- [ ] D. To create multiple objects automatically

Correct! B. To prevent direct access from outside the class.

In Java, the private access modifier restricts access to a field or method from outside the class where it is declared.
```java
class BankAccount {
    private double balance = 1000;

    public double getBalance() {
        return balance;
    }
}
```
- `balance` cannot be accessed directly from an unrelated external class.
- `getBalance()` provides a controlled way to read the balance.
- A `deposit` or `withdrawal` method can validate changes before updating the balance.

Important: `private` does not make a variable constant. Its value can still change through methods inside the class.

| Keyword	     | Meaning                                      |
|--------------|----------------------------------------------|
| `private`	   | Accessible within the declaring class        |
| `public`	   | Accessible wherever other access rules permit|
| `protected`	 | Accessible within the package and by subclasses, subject to Java's access rules|

> **Encapsulation = bundle data and methods + control access to internal data**

---

Q.58 — Program Analysis Tools

Question: Program Analysis Tools are used for:
- [ ] A. Designing software architecture
- [ ] B. Measuring software reliability
- [ ] C. Automatically generating test cases
- [x] D. Analysing code for errors and performance bottlenecks

Correct! Option D. Analysing code for errors and performance bottlenecks.

**1. What are Program Analysis Tools?** <br/>
**Program analysis** tools help developers examine source code to identify potential errors, understand program behaviour, and find performance problems.

Think of them as inspectors for your code. They help you find problems before those problems affect users.

For example, consider this Python code:
```py
def calculate_total(price, quantity):
    total = price * quantity
    return total

print(calculate_total(100, 5))  # 500
```
A program analysis tool can inspect the code to help identify potential bugs, suspicious patterns, or inefficient operations.

Two important types
1. **Static analysis**:
- Examines code without executing it.
- It can detect some errors, unused variables, and coding-standard violations.
```py
x = 10
y = "hello"
print(x + y)
```
  
2. **Dynamic analysis**:
- Examines a program while it runs.
- It can help identify runtime errors, memory problems, and performance bottlenecks.
```py
x = 10
y = 0
print(x / y)
```

A **performance bottleneck** is a part of a program that slows down the entire application.

**Remember**:
- **Program analysis** -> Inspect code for problems.
- **Testing** -> Execute or check software to find failures.
- **Test-case generation** -> Create inputs to test software.
- **Software architecture** -> Plan the system's structure.

Which tool category is primarily used to identify coding errors without executing the program?
- [x] A. Static analysis tools
- [ ] B. Performance monitoring tools
- [ ] C. Test execution tools
- [ ] D. Code-generation tools

Correct! Static analysis tools. 

**Static analysis** examines source code without running the program. It can identify potential problems before execution.

| Term                         | Explanation                                                                      |
|------------------------------|----------------------------------------------------------------------------------|
| Static analysis tools	       | Inspect code without executing it.                                               |
| Performance monitoring tools | Usually measure execution time, resource usage, and other runtime behaviour.     |
| Test execution tools	       | Run tests to check whether the software behaves as expected.                     |
| Code-generation tools	       | Automatically produce source code from specifications, templates, or other inputs.|


Remember for the exam
- **Static analysis** -> Examine code without running it.
- **Dynamic analysis** -> Examine behaviour while the program runs.
- **Performance monitoring** -> Measure speed and resource usage.
- **Code generation** -> Produce code automatically.

---

**Q.59 — Method Signature in OOP**

Question: In OOP, what does the term "method signature" refer to?
- [ ] A. The name of the method
- [ ] B. The return type of the method
- [ ] C. The parameters of the method
- [x] D. The combination of method name and parameter types

Correct! D. The combination of method name and parameter types.

**1. What is a method signature?** <br/>
A method signature identifies a method using its name and the parameters that define how it can be called.

Consider this Java example:
```java
void display(int number) {
    System.out.println(number);
}

void display(String name) {
    System.out.println(name);
}
```
Both methods have the same name, `display`, but different parameter types:
- `display(int)` accepts an integer.
- `display(String)` accepts a string.
Their signatures distinguish the two methods, allowing **method overloading**.

In Java, a method signature includes the method name and parameter types. <br/>
The `return type` alone is not part of the signature, and you cannot overload methods merely by changing their return types. <br/>
Other programming languages may define signatures differently.

Remember:
> **Method signature = method name + parameter list**

Example: `calculate(int, int)` and `calculate(double, double)` have different signatures in Java.

Can two Java methods have the same name and identical parameter types but different return types only?
- [ ] A. Yes, always
- [x] B. No, Java does not allow this as method overloading
- [ ] C. Yes, if both methods are public
- [ ] D. Yes, if one method returns an integer

Correct! B. **No, Java does not allow this as method overloading**.

In Java, We cannot define two methods in the same class with the same name and identical parameter types just by changing their return types.
```java
class Calculator {
    int add(int a, int b) {
        return a + b;
    }

    double add(int a, int b) {
        return a + b;
    }
}
```
**compilation error** because both methods have the same name `add` and the same parameter types `(int, int)`. <br/> 
Changing the return type from int to double does not make them different method signatures.

However, this is valid method overloading:
```java
class Calculator {
    int add(int a, int b) {
        return a + b;
    }

    int add(int a, int b, int c) {
        return a + b + c;
    }
}
```
Here, the parameter lists differ: one method takes two integers, and the other takes three.

| Change between methods	  | Valid overloading? |
|---------------------------|--------------------|
| Different parameter count	| Yes                |
| Different parameter types	| Yes                |
| Different parameter order	| Yes, if the resulting parameter types differ by position |
| Different return type only|	No                 |

> Memory tip: **Method overloading depends on the parameter list, not the return type alone.**

---

**Q.60 — Software Testing**

Which of the following involves testing individual components or units of code?
- [ ] A. Integration Testing
- [ ] B. System Testing
- [x] C. Unit Testing
- [ ] D. Acceptance Testing

Correct! C. Unit Testing

**1. Unit Testing** <br/>
Unit testing is the process of testing individual, small parts of a program, such as a function, method, or class, to verify that each works correctly.

Imagine we are developing a school management application with these functions:
- `calculateTotal()` - calculates total marks.
- `calculatePercentage()` - calculates percentage.
- `checkResult()` - determines whether a student passed.
Before testing the entire application, we test each function separately.

<img width="980" height="322" alt="image" src="https://github.com/user-attachments/assets/34c0afe5-b299-4b92-b00f-cb16b1849e30" />


For example, if `calculateTotal(40, 50)` should return `90`, a unit test checks whether the actual result matches the expected result.

**Different Terms**

|  Term                   | Meaning	                                          | Example                     |
|-------------------------|---------------------------------------------------|-----------------------------|
| **Integration Testing**	| Tests whether multiple components work together.	| Checking whether marks calculation connects correctly to result generation.
| **System Testing**	    | Tests the complete, integrated application.	| Testing the entire school management application. |
| **Unit Testing**	      | Tests an individual component or unit of code.	| Testing `calculateTotal()` by itself.|
| **Acceptance Testing**	| Checks whether the software meets user or business requirements. | A school verifies that the application meets its needs before accepting it. |


**Remember the testing sequence:**
> **Unit -> Integration -> System -> Acceptance**

- **Unit**: One component.
- **Integration**: Components working together.
- **System**: The complete application.
- **Acceptance**: Does it meet the user's requirements?
This is a common conceptual sequence for exams, although actual development workflows may vary.

A developer tests whether the login module and the database module communicate correctly with each other. Which type of testing is being performed?
- [ ] A. Unit Testing
- [x] B. Integration Testing
- [ ] C. Acceptance Testing
- [ ] D. System Testing

Correct! Integration Testing

The developer tests whether the login module and database module communicate correctly with each other. <br/>
The key phrase is with each other.
- The login module is one component.
- The database module is another component.
- Testing their interaction checks whether the two components work together correctly.
That is **Integration Testing**.

<img width="1000" height="352" alt="image" src="https://github.com/user-attachments/assets/64a8fdc7-88d4-4e41-9a64-d2529ed54198" />

**Memory tip**
- **One component** -> Unit testing
- **Components together** -> Integration testing
- **Whole application** -> System testing
- **User requirements** -> Acceptance testing

A developer tests the calculatePercentage() function by itself to confirm that it returns the correct percentage. <br/>
Which testing type is this?
- [ ] A. Integration Testing
- [ ] B. System Testing
- [x] C. Unit Testing
- [ ] D. Acceptance Testing

Correct! C. Unit Testing  

A unit test checks whether this individual function produces the expected result.

---



---



---





---
</details>
<!----------------------------->


<details>
  <summary> <b> PYQs 2024 </b> </summary>

<br/>

| Questions 1–5: Digital media, Boolean algebra, and graphs |
|-----------------------------------------------------------|

---

Q1. Audio compression can be used for _____
- [ ] (A) Voice and data
- [ ] (B) Video and voice
- [x] (C) Speech or music
- [ ] (D) Picture and colors

Correct answer: (C) Speech or music

Concept: Audio compression reduces the amount of data needed to store or transmit sound.
- Lossless compression preserves the original audio exactly.
- Lossy compression removes some less perceptible audio information to reduce file size.

Examples include FLAC (lossless) and MP3 (lossy). Image compression, by contrast, is used for pictures.

---

Q2. _____ is basically a form of pictorial presentation.
- [ ] (A) Photography
- [ ] (B) Animations
- [x] (C) Drawing
- [ ] (D) Creativity

Best answer: (C) Drawing

Concept: A drawing represents information visually through lines, shapes, and symbols. <br/>
Photography and animation are also visual media, so the wording is somewhat broad, but drawing is the most likely intended answer.

---

Q3. Consider two binary numbers A = 110001 and B = 001100. What is the result of (A AND B) OR (NOT A AND NOT B)?
- [ ] (A) 000000
- [ ] (B) 110001
- [ ] (C) 001100
- [ ] (D) 111101

Correct calculation: 000010 — none of the listed options.

Let's solve it bit by bit. For this question, use six-bit binary numbers and six-bit complements.
```
A                 = 110001
B                 = 001100
A AND B           = 000000

NOT A             = 001110
NOT B             = 110011
NOT A AND NOT B   = 000010

Final OR result   = 000010
```

Concepts to remember:
- `AND`: The output bit is 1 only when both input bits are 1.
- `OR`: The output bit is 1 when at least one input bit is 1.
- `NOT`: Flips each bit, with the number of bits fixed by the representation.

The expression is equivalent to bitwise XNOR: it produces 1 wherever the corresponding bits of A and B are equal. The provided options appear to contain an error.

---

Q4. What is the minimized expression for the Boolean function F(A,B,C,D)=Sigma(0,1,2,4,5,6,10,12,13) using the K-map method?


One minimized sum-of-products expression is: `F = A'C' + BC' + A'D' + B'CD'`

Here, a prime (`′`) means `NOT`. For example, `A'` means `NOT A`.

Concept: **Karnaugh map (K-map)**

A K-map groups adjacent cells containing 1s in groups of 1, 2, 4, 8, and so on. Larger groups generally produce simpler Boolean expressions.

For this function, the groups can be represented as:
| Grouped minterms	| Simplified term |
|-------------------|-----------------|
| 0, 1, 4, 5	      | A'C'            |
| 4, 5, 12, 13	    | BC'             |
| 0, 2, 4, 6	      | A'D'            |
| 2, 10	            | B'CD'           |

These groups cover all the given minterms. Some minterms can appear in more than one group, which is allowed in K-map simplification.

---

Q5. The minimum number of edges in a spanning tree of a connected graph with `n` vertices is:
- [ ] (A) `n`
- [x] (B) `n-1`
- [ ] (C) `n+1`
- [ ] (D) `n(n-1)/2`
  
Correct answer: (B) `n-1`

Concept: A spanning tree connects every vertex of a connected graph without forming any cycle.

For example, if a graph has 5 vertices, a spanning tree needs exactly `5 - 1 = 4` edges.

Remember:
- A tree with `n` vertices has `n-1` edges.
- Adding an edge to a tree creates a cycle.
- Removing an edge from a tree disconnects it.

---

Q6. In pointer implementation of linked lists, which operation can be performed in constant time `O(1)` when inserting or deleting nodes?
- [x] (A) Inserting at the beginning
- [ ] (B) Inserting at the end
- [ ] (C) Inserting at a specific position
- [ ] (D) Deleting a specific node

Correct answer: (A) Inserting at the beginning

Concept: Inserting at the beginning of a singly linked list takes constant time because only a small number of pointers need to be changed.
```
Before: HEAD → 20 → 30 → NULL

Insert 10:

After:  HEAD → 10 → 20 → 30 → NULL
```

The number of existing nodes does not affect the number of pointer changes.

Exam caution: Inserting at the end can also be `O(1)` if a tail pointer is maintained. Deleting a specific node depends on whether the required node and its predecessor are already available.

---

Q7. For a 2-D array represented in row-major order, the index formula to access the element at row i and column j, using base address B, is:
- [x] (A) `Index = B + (i x n + j)`
- [ ] (B) `Index = B + (j x n + i)`
- [ ] (C) `Index = B + (i + j)`
- [ ] (D) `Index = B + (i x m + j)`

Best answer: (A), assuming n is the number of columns and indices are zero-based.

Concept: Row-major order stores an entire row contiguously before moving to the next row.

For an array with n columns, the element `offset = i x n+j`

If B is a byte address and each element occupies w bytes, the full address formula is: `Address = B + (i x n+j) x w`

The question's formula omits the element-size factor, so it is really an element-index formula unless each element occupies one address unit.

---

Q8. In general, a file is basically a collection of all related _____.
- [ ] (A) Rows and columns
- [ ] (B) Database
- [ ] (C) Fields
- [x] (D) Records

Correct answer: (D) Records

Concept: In the traditional file-processing model:
- Field: One item of information, such as a student's name.
- Record: A collection of related fields about one entity, such as one student's details.
- File: A collection of related records.
- Database: An organized collection of related data, often stored in multiple tables or files.

---

Q9. Which of the following refers to the number of attributes in a relation?
- [ ] (A) Row
- [x] (B) Degree
- [ ] (C) Column
- [ ] (D) All of the above

Correct answer: (B) Degree

Concept in relational databases:
- Degree: Number of attributes (columns) in a relation.
- Cardinality: Number of tuples (rows) in a relation.

For example, a Student table with RollNo, Name, and Class has degree 3. If it contains 40 student records, its cardinality is 40.

---

Q10. Process-to-process communication involves communication between:
- [ ] (A) Different network layers
- [ ] (B) Different devices on the same network
- [ ] (C) Devices using different protocols
- [x] (D) Processes on different devices

Correct answer: (D) Processes on different devices

Concept: Process-to-process communication means data is exchanged between application processes running on communicating hosts. At the transport layer, TCP and UDP use port numbers to identify the relevant application processes.

For example, a browser process communicates with a web server process. The devices do not necessarily have to be on the same local network.

---

Q11. The term HTTP stands for:
- [ ] (A) Hyper Terminal Tracing Program
- [ ] (B) Hypertext Tracing Program
- [x] (C) Hypertext Transfer Protocol
- [ ] (D) Hypertext Tracing Protocol

Correct answer: (C) Hypertext Transfer Protocol

Concept: HTTP is an application-layer protocol used for communication between web clients and servers.

For example, when a browser requests a webpage, it can send an HTTP request and receive an HTTP response.

Remember these common protocols:
| Protocol	| Full form and primary use                       |
|-----------|-------------------------------------------------|
| HTTP	    | Hypertext Transfer Protocol — web communication |
| HTTPS	    | HTTP Secure — HTTP protected using TLS          |
| FTP	      | File Transfer Protocol — file transfer          |
| SMTP	    | Simple Mail Transfer Protocol — sending email   |
| DNS	      | Domain Name System — resolves domain names      |
| DHCP	    | Dynamic Host Configuration Protocol — assigns network configuration |

---

Q12. Which software life cycle model is based on iterative prototyping?
- [ ] (A) Waterfall model
- [ ] (B) Spiral model
- [ ] (C) Agile model
- [x] (D) Prototype model

Best answer: (D) Prototype model

Concept: The Prototype Model develops an early working version of the software so that users can evaluate it and provide feedback. Developers refine the prototype repeatedly until the requirements are better understood.

Example:
1. Build a basic school website.
2. Show it to teachers.
3. Collect feedback about the timetable and student section.
4. Improve the design and functionality.
5. Develop the final system.
Exam distinction: The Spiral Model also uses repeated cycles and can include prototyping, but its defining feature is risk-driven development. Since the question specifically emphasizes iterative prototyping, the Prototype Model is the most direct answer.

---

Q13. ISO 9000 and SEI CMM are both frameworks related to:
- [ ] (A) Software testing
- [ ] (B) Software documentation
- [x] (C) Software quality assurance and process improvement
- [ ] (D) Software design principles

Correct answer: (C) Software quality assurance and process improvement

Concept:
- ISO 9000 family: Standards related to quality management systems.
- SEI CMM: Capability Maturity Model, developed to assess and improve an organization's software-development processes.

The key idea is that consistent, well-managed processes can improve the quality and reliability of software.

---

Q14. What is the term for defining multiple methods in a class with the same name but different parameters?
- [ ] (A) Overriding
- [x] (B) Overloading
- [ ] (C) Inheriting
- [ ] (D) Inheritance

Correct answer: (B) Overloading

Concept: Method overloading means using the same method name with different parameter lists.

Example in Java:
```java
int add(int a, int b) {
    return a + b;
}

int add(int a, int b, int c) {
    return a + b + c;
}
```
Both methods are named `add`, but they accept different numbers of arguments.

Compare:
- Overloading: Same name, different parameter lists.
- Overriding: A subclass provides its own implementation of an inherited method.
- Inheritance: A class acquires or extends properties and behavior from another class.
In Java, changing only the return type is not sufficient to overload a method.

---

Q15. The language accepted by Pushdown Automata is:
- [ ] (A) Recursive language
- [x] (B) Context-free language
- [ ] (C) Linearly bounded language
- [ ] (D) All of the mentioned

Correct answer: (B) Context-free language

Concept: A Pushdown Automaton (PDA) is like a finite automaton with an additional memory structure called a stack.

The stack helps it recognize patterns such as matching numbers of opening and closing parentheses.

For example:
```
 L = { a^n b^n | n>=0}
```
This language contains strings such as ab, aabb, and aaabbb. <br/>
A PDA can recognize it by pushing a symbol for each a and popping one for each b.

Exam fact: A nondeterministic PDA recognizes context-free languages. A deterministic PDA recognizes the smaller class of deterministic context-free languages.

---

Q16. Which of the following is the best example of a semantic network?
- [x] (A) WordNet
- [ ] (B) Human food chain
- [ ] (C) MYCIN
- [ ] (D) Autonomous car driver

Correct answer: (A) WordNet

Concept: A semantic network represents concepts and the relationships between them as a graph.

For example:
- Dog is a animal.
- Dog has a tail.
- Animal is a living thing.

WordNet is a lexical database that organizes words into groups of synonyms and connects them through semantic relationships.

MYCIN, in contrast, is a well-known rule-based medical expert system.

---

Q17. Which of the following is not a characteristic of expert systems?
- [ ] (A) Understandable
- [ ] (B) Highly responsive
- [x] (C) Unreliable
- [ ] (D) High performance

Correct answer: (C) Unreliable

Concept: An expert system uses a knowledge base and an inference mechanism to solve problems in a specialized domain.

Its desirable characteristics include:
- Reliable and consistent advice.
- Good performance within its defined domain.
- Explanation of conclusions, where supported.
- Fast responses for suitable problems.

Being unreliable is a weakness, not a desirable characteristic.

---

Q18. Unclassified email is called:
- [ ] (A) Extra mail
- [x] (B) Spam
- [ ] (C) Junk mail
- [ ] (D) None of the above

Best answer: (B) Spam

Concept: Spam is unsolicited or unwanted electronic messaging, especially bulk email.

Important wording note: The phrase “unclassified email” is imprecise. Both spam and junk mail are commonly used for unwanted email, so options B and C overlap. In typical computer-awareness questions, spam is the expected term.

---

Q19. Which of the following is the abbreviation of JPEG?
- [x] (A) Joint Photographic Experts Group
- [ ] (B) Joint Photographs Expansion Group
- [ ] (C) Joint Photographic Expanded Group
- [ ] (D) Joint Photographic Expansion Group

Correct answer: (A) Joint Photographic Experts Group

Concept: JPEG is associated with a widely used image-compression standard, especially for photographs.
- JPEG commonly uses lossy compression.
- It can greatly reduce image file size.
- Repeated saving with lossy compression may reduce image quality.

Remember: PNG is another common image format and generally uses lossless compression.

---

Q20. When adding two positive binary numbers using the 2's complement method, if the result has a carry-out from the most significant bit (MSB), what should be done?
- [x] (A) Ignore the carry
- [ ] (B) Add the carry to the least significant bit (LSB)
- [ ] (C) Add the carry to the sign bit
- [ ] (D) Subtract the carry from the MSB

Correct answer: (A) Ignore the carry

Concept: In fixed-width 2's complement arithmetic, the carry-out beyond the most significant bit is discarded. Overflow is a separate issue and must be checked independently.

For example, using four bits:
```
  0011   (+3)
+ 0010   (+2)
------
  0101   (+5)
```

This example has no carry-out. In fixed-width addition, any carry beyond the four-bit result is discarded.

Exam distinction: Discarding carry-out does not mean signed overflow can never happen. For example, adding two positive signed numbers can produce a negative-looking bit pattern if the mathematical result exceeds the representable range.


---

Q21. In the All-Pairs Shortest Paths algorithm, what does the term “transitive property” refer to?
- [ ] (A) The property of having a cycle path
- [ ] (B) The property of having all vertices connected to each other
- [x] (C) The property of being able to reach one vertex from another
- [ ] (D) The property of a path being shorter than another path

Best available answer: (C), but the wording is imprecise.

Concept: In the context of shortest-path algorithms, the key idea is that a route from vertex \(i\) to vertex \(j\) may be improved by passing through an intermediate vertex \(k\).

The Floyd–Warshall update is:
```
d[i][j] = min(d[i][j], d[i][k] + d[k][j])
```

It compares the current path with a route that goes through `k`.

Strictly speaking, this is the shortest-path relaxation principle, not a precise definition of the transitive property. Option C is the closest available choice.

---

Q22. In a Binary Search Tree (BST), deleting a node with one child involves:
- [ ] (A) Removing the node and replacing it with its left child
- [ ] (B) Removing the node and replacing it with its right child
- [ ] (C) Removing the node and replacing it with its parent
- [ ] (D) Removing the node and leaving the subtree unaltered

Correct concept: Replace the node with its only child.

Options A and B are both incomplete: either can be correct depending on which child the node has. Therefore, the question does not have one universally correct option as written.

Example:
```
Before:          After deleting 20:

    20                  30
      \
       30
```

If the node has only a left child, promote the left child. If it has only a right child, promote the right child. This preserves the BST ordering property.

---

Q23. Counting Sort is particularly efficient for sorting arrays where the range of elements is:
- [ ] (A) Very large
- [x] (B) Very small
- [ ] (C) Constant
- [ ] (D) Sorted

Correct answer: (B) Very small

Concept: Counting Sort counts how many times each value occurs, then uses those counts to reconstruct the sorted sequence.

Its typical time complexity is: `O(n+k)` where: `n` is the number of elements, `k` is the size of the value range.

Example: 
```
Sorting [2, 1, 2, 0, 1] is efficient because the values range only from 0 to 2.
```
If the range is extremely large compared with the number of elements, Counting Sort may waste considerable time and memory.


---

Q24. What is the primary function of SNMP (Simple Network Management Protocol)?
- [ ] (A) File transfer
- [ ] (B) Remote terminal access
- [x] (C) Network management and monitoring
- [ ] (D) Web browsing

Correct answer: (C) Network management and monitoring

Concept: SNMP is used to monitor and manage network devices such as routers, switches, and servers.

A network administrator may use it to collect information about:
- Interface traffic.
- Device availability.
- Error counts.
- Performance and resource usage.


Quick revision of the related protocols:
| Protocol	| Main purpose                      |
|-----------|-----------------------------------|
| SNMP	    | Network monitoring and management |
| FTP	      | File transfer                     |
| SSH	      | Secure remote access              |
| HTTP	    | Web communication                 |

---

Q25. Frame design in the Data Link Layer includes:
- [ ] (A) Deciding the routing path for data packets
- [x] (B) Defining the structure of data frames
- [ ] (C) Assigning IP addresses to devices
- [ ] (D) Setting the data transmission rate

Correct answer: (B) Defining the structure of data frames

Concept: The Data Link Layer organizes bits into frames so devices on the same link can exchange data.

A frame may contain:
- Header information, such as source and destination MAC addresses.
- Payload, which carries the data.
- Trailer information, such as an error-detection value.

Remember the distinction:
- Data Link Layer: Frames and MAC addressing.
- Network Layer: Packets and IP addressing.
- Transport Layer: Segments, ports, and end-to-end transport.

Routing paths are generally selected at the Network Layer, not during frame design.

---

Q26. TCP regulates end-to-end packet flow using:
- [ ] (A) Source quench messages
- [x] (B) A window size advertisement
- [ ] (C) Fixed-size segments
- [ ] (D) Binary exponential backoff

Correct answer: (B) A window size advertisement

Concept: TCP uses a sliding-window mechanism to control how much data a sender can transmit before receiving acknowledgements.

The receiver advertises a receive window indicating how much additional data it can accept. This is called flow control.

Do not confuse it with congestion control:
- Flow control: Prevents overwhelming the receiver.
- Congestion control: Helps prevent overloading the network.

Source Quench is obsolete, and binary exponential backoff is associated with Ethernet contention and related protocols rather than TCP's receive-window mechanism.

---

Q27. What is the primary purpose of a Software Requirements Specification (SRS) document?
- [ ] (A) To list the programming languages used
- [ ] (B) To describe the user-interface design
- [x] (C) To define the software’s functional and non-functional requirements
- [ ] (D) To specify the hardware components required

Correct answer: (C) To define the software’s functional and non-functional requirements

Concept: An SRS explains what a software system must do and the constraints under which it must operate.
- Functional requirement: A student can view examination results.
- Non-functional requirement: The results page should load within a specified time under defined conditions.

An SRS may mention interfaces or hardware constraints, but its primary purpose is to specify requirements rather than prescribe every implementation detail.

---

Q28. What is encapsulation in OOP?
- [ ] (A) The ability to inherit properties from multiple classes
- [ ] (B) The process of creating objects
- [x] (C) The bundling of data and methods that operate on the data
- [ ] (D) The use of abstract classes only

Correct answer: (C) The bundling of data and methods that operate on the data

Concept: Encapsulation combines data and the methods that work on that data within a class. Access controls can also restrict how the internal state is modified.

Example in Java:
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
```

Here, balance is private, and the class provides controlled ways to access or change it.

Remember the four common OOP concepts:
- Encapsulation — bundling and controlled access.
- Abstraction — exposing essential features while hiding implementation details.
- Inheritance — deriving a class from another class.
- Polymorphism — one interface or method name supporting different behavior.

---

Q29. What is the purpose of CSS media queries?
- [ ] (A) To add multimedia content to a webpage
- [ ] (B) To create animations
- [x] (C) To apply different styles based on the device’s characteristics
- [ ] (D) To define color schemes for a website

Correct answer: (C) To apply different styles based on the device’s characteristics

Concept: Media queries let you apply CSS conditionally based on screen width, orientation, and other device or display characteristics.

Example:
```css
/* Default styles */
.container {
    width: 80%;
}

/* Styles for narrower screens */
@media (max-width: 600px) {
    .container {
        width: 100%;
    }
}
```
On screens up to 600 pixels wide, the container uses the full width.

This is an important technique in responsive web design, helping webpages adapt to phones, tablets, and desktops.

---

Q30. How can you make an asynchronous request to a server in JavaScript?
- [ ] (A) Using the async keyword
- [ ] (B) Using the await keyword
- [x] (C) Using the fetch API or XMLHttpRequest
- [ ] (D) By defining a callback function

Best answer: (C) Using the fetch API or XMLHttpRequest

Concept: `fetch()` is a modern JavaScript API for making network requests. It returns a `Promise`, allowing the program to continue doing other work while waiting for the response.

Example:
```js
async function getData() {
    const response = await fetch(
        "https://example.com/data"
    );

    const data = await response.json();
    console.log(data);
}
```

Understand the difference:
- `fetch()` initiates the network request.
- `async` allows a function to return a Promise.
- `await` pauses execution within an async function until a Promise settles.
- `Callbacks` are another way to handle asynchronous operations.

Options A, B, and D can all be involved in asynchronous programming, but C most directly identifies APIs used to make the request.

---

Q31. What is the purpose of SQL injection attacks?
- [ ] (A) To increase the performance of database queries
- [x] (B) To bypass authentication systems
- [ ] (C) To improve database security
- [ ] (D) To enhance data encryption

Correct answer: (B) To bypass authentication systems

Concept: SQL injection is a security vulnerability in which malicious input changes the meaning of a SQL query.

For example, if an application builds SQL by concatenating untrusted user input, an attacker may alter the query to access data or bypass login checks.

SQL injection can be used to:
- Bypass authentication.
- Read unauthorized data.
- Modify or delete database records.
- In some circumstances, perform other privileged database actions.

Prevention: Use parameterized queries or prepared statements instead of directly concatenating user input into SQL.

---

Q32. A grammar that produces more than one parse tree for the same sentence is called:
- [ ] (A) Contiguous
- [x] (B) Ambiguous
- [ ] (C) Unambiguous
- [ ] (D) Regular

Correct answer: (B) Ambiguous

Concept: A context-free grammar is ambiguous if at least one string in its language has more than one distinct parse tree, or equivalently, more than one leftmost or rightmost derivation.

Example: `a + b * c`
Without suitable precedence rules, an expression grammar might interpret this as either:
- `a + (b * c)`
- `(a + b) * c`

These interpretations produce different parse trees and meanings.

Exam tip: Ambiguity concerns multiple valid syntactic structures for the same string, not merely multiple strings produced by a grammar.

---

Q33. The minimum number of productions required to produce a language consisting of palindrome strings over `Sigma = {a,b}` is:
- [ ] (A) 3
- [ ] (B) 7
- [X] (C) 5
- [ ] (D) 6

Likely intended answer: (C) 5

One standard grammar for all palindromes over {a, b}, including the empty string, is: ` S -> aSa | bSb | a | b | epsilon`

This has five production alternatives:
```
1. S -> aSa
2. S -> bSb
3. S -> a
4. S -> b
5. S -> epsilon
```

Why it works: A palindrome reads the same forwards and backwards. The first two productions add matching symbols to both ends, while the final three allow the derivation to end with a one-character palindrome or the empty string.

Important caveat: The question does not specify whether the empty string is included or how productions are counted. The answer of five follows the conventional grammar above; different conventions can change the count.

---

Q34. Which of the following is true for the language {a^p | p is a prime}?
- [ ] (A) It is regular but not context-free
- [x] (B) It is neither regular nor context-free, but accepted by a Turing machine
- [ ] (C) It is not accepted by a Turing Machine
- [ ] (D) It is context-free but not regular

Correct answer: (B) It is neither regular nor context-free, but accepted by a Turing machine

Concept: This language contains strings whose lengths are prime numbers:
```
aa       length 2  → prime
aaa      length 3  → prime
aaaaa    length 5  → prime
aaaaaaa  length 7  → prime
```

Strings of lengths 4, 6, and 8 are not in the language.

Why is the language not regular? A unary regular language must have an ultimately periodic set of accepted lengths. Prime numbers do not form such a set, so a finite automaton cannot recognize this language.

Why is it not context-free? Every context-free language over a one-symbol alphabet is regular. Since this language is not regular, it cannot be context-free either.

However, a Turing machine can count the input length and test whether that length is prime. Therefore, the language is decidable and is certainly accepted by a Turing machine.

---

Q35. Which products are people most likely to be more uncomfortable buying on the Internet?
- [ ] (A) Books
- [ ] (B) Movie ticket
- [x] (C) Furniture
- [ ] (D) None of the above

Best answer: (C) Furniture

Concept: Furniture is a physical product that buyers may want to inspect in person before purchasing. They may want to check its size, material, comfort, colour, and build quality.

Books and movie tickets are commonly purchased online because buyers generally don't need to inspect the physical product in the same way.

This is a question about consumer behaviour in e-commerce, not a universal rule: modern online furniture shopping is common, but the traditional exam answer is likely furniture.

---

Q36. The study of encryption is called:
- [ ] (A) Encryption
- [x] (B) Cryptography
- [ ] (C) Decryption
- [ ] (D) None of the above

Correct answer: (B) Cryptography

Concept: Cryptography studies techniques for securing information, including encryption, decryption, authentication, and digital signatures.
- Plaintext: Original readable message.
- Encryption: Converts plaintext into ciphertext using an algorithm and key.
- Ciphertext: The transformed message.
- Decryption: Converts ciphertext back into readable plaintext using the appropriate key.

Example:
```
Plaintext → Encryption + Key → Ciphertext
Ciphertext → Decryption + Key → Plaintext
```

Remember: encryption is one part of cryptography; cryptography is the broader field.

---

Q37. SMTP, FTP, and HTTP — full forms and uses

| Protocol	| Full form	                    | Main use                   |
|-----------|-------------------------------|----------------------------|
| SMTP	    | Simple Mail Transfer Protocol	| Sending email              |
| FTP	      | File Transfer Protocol	      | Transferring files         |
| HTTP	    | Hypertext Transfer Protocol	  | Transferring web resources |

Concept to remember:
- SMTP is used to send email, including between mail servers.
- FTP is used to transfer files between a client and server.
- HTTP is used for communication between web clients and servers.

Exam trap: Receiving email is commonly associated with POP3 or IMAP, rather than SMTP.

---

Q38. MIMD Full form: Multiple Instruction, Multiple Data.
- MIMD is a classification of computer architecture in Flynn's taxonomy.

It means multiple processing units can execute different instruction streams on different data at the same time.

Examples include multicore processors and multiprocessor systems running independent tasks.

Flynn's four categories:
| Category	| Instruction streams	| Data streams |
|-----------|---------------------|--------------|
| SISD	    | Single	            | Single       |
| SIMD	    | Single 	            | Multiple     |
| MISD	    | Multiple	          | Single       |
| MIMD	    | Multiple	          | Multiple     |

Remember: SIMD is useful for applying the same operation to many data elements; MIMD allows different operations on different data.

---

Q39. Binary-to-Gray code conversion

Rule: Keep the most significant bit (MSB) unchanged. Each subsequent Gray bit is the XOR of two adjacent binary bits.

```
G0 = B0
Gi = Bi-1 (+) Bi
Here, (+) represents XOR.
```
Example: Convert binary `1011` to Gray code.
| Step	     | Calculation | Gray bit |
|------------|-------------|----------|
| First bit	 | Copy MSB	   | 1        |
| Second bit | 1 (+) 0	   | 1        |
| Third bit	 | 0 (+) 1     | 1        |
| Fourth bit | 1 (+) 1     | 0        |
Answer: `1110` 

Why Gray code matters: Consecutive Gray-code values differ by only one bit, which helps reduce errors during transitions in devices such as rotary encoders.

---

Q40. Merge Sort — worst-case time complexity <br/>
Answer: `O(nlog n)`

Merge Sort divides the array into halves, sorts each half recursively, and merges the sorted halves.

Its recurrence is: `T(n) = 2T(n/2) + O(n)` 

Therefore, its best-, average-, and worst-case time complexities are all `O(nlog n)`.

Space complexity: Standard array-based Merge Sort generally requires `O(n)` additional space.

---

Q41. Abstraction <br/>
Definition: Abstraction means exposing essential features while hiding unnecessary implementation details.

For example, when using an ATM, you select an operation such as withdrawing money without needing to know the internal banking software logic.

In OOP, abstraction can be implemented using abstract classes and interfaces, depending on the programming language.

Distinguish it from encapsulation:
- Abstraction: Hides implementation complexity and presents a simplified interface.
- Encapsulation: Bundles data and methods together and controls access to internal state.

---

Q42. One-to-many (1:M) relationship

A one-to-many relationship means one record in one entity can be associated with multiple records in another entity.

Example:
```
One Department
      |
      | 1:M
      |
Many Employees
```

One department can have many employees, while each employee belongs to one department in this simplified model.

Database implementation: The primary key of the “one” side is usually stored as a foreign key in the table on the “many” side.

Example:
- Department(DepartmentID, DepartmentName)
- Employee(EmployeeID, Name, DepartmentID)
Here, `Employee.DepartmentID` references `Department.DepartmentID`.

---

Q43. RFID — full form <br/>
RFID = Radio Frequency Identification.

RFID uses radio waves to identify or track tagged objects.

A typical system contains:
- Tag: Attached to an object and stores identification information.
- Reader: Communicates with the tag.
- Backend system: Processes the collected information, when used.

Applications include inventory tracking, access cards, toll collection, and supply-chain management.

Exam distinction: RFID does not necessarily require direct visual contact between the reader and the tag.

---

Q44. Pushdown Automata — grammar name  <br/>
Answer: Context-Free Grammar (CFG).

A pushdown automaton (PDA) recognizes context-free languages. Context-free grammars generate context-free languages.

A CFG is formally represented as: 
```
G = (V, Sigma, P, S)
Where:
V = variables or non-terminals.
Sigma = terminals.
P = production rules.
S = start symbol.

For example:
S -> aSb | epsilon

generates strings such as ab, aabb, and aaabbb.
```
Exam trap: A general nondeterministic PDA recognizes all context-free languages. A deterministic PDA recognizes only deterministic context-free languages.

---

Q45–46. BLE — full form <br/>
BLE = Bluetooth Low Energy.

BLE is a wireless communication technology designed for devices that need to communicate while consuming relatively little power.

Common uses include:
- Fitness trackers and smartwatches.
- Beacons and proximity detection.
- Sensors and Internet of Things (IoT) devices.

BLE versus classic Bluetooth: BLE is particularly suited to small, intermittent data exchanges with low energy consumption. It is not simply another name for all Bluetooth communication.

---

Q47. What HTML tag is used for `a` URL link? <br/>
Answer: The anchor tag, <a>.

Example:
```html
<a href="https://example.com">Visit website</a>
```
- `<a>` creates the hyperlink.
- `href` specifies the destination URL.
- `Visit website` is the clickable text.

Remember: `<link>` is generally used to connect external resources such as stylesheets in the document head. For a clickable link in webpage content, use `<a>`.

---

Q48. FAT stands for what? <br/>
**FAT = File Allocation Table**.

FAT is a file-system structure used to track how files occupy storage space.

Common variants include FAT12, FAT16, and FAT32.

The file system maintains information that helps the operating system locate file data on a storage device. FAT32 is commonly associated with removable storage and broad device compatibility.

---

Q49. UDP, DDL, and INSERT INTO

**UDP — User Datagram Protocol**

UDP is a transport-layer protocol that sends datagrams without establishing a connection. It has low overhead but does not guarantee delivery, ordering, or retransmission.

Common applications include real-time voice/video, online gaming, and DNS queries.

**DDL — Data Definition Language**

DDL commands define or modify database structures.

Common examples:
- `CREATE` — creates a table or other database object.
- `ALTER` — changes an existing structure.
- `DROP` — removes a database object.
- `TRUNCATE` — removes all rows from a table while retaining the table structure.

**`INSERT INTO` - SQL command**
```sql
--- INSERT INTO adds new records to a table.

INSERT INTO Student (RollNo, Name)
VALUES (101, 'Amit');
```
This inserts a student record with roll number 101 and name Amit.

Exam distinction: `INSERT` is a DML command in the common classification, not DDL.

---

Q50. Abstract Data Type (ADT) <br/>
An Abstract Data Type defines a data type in terms of its values and permitted operations, without specifying the internal implementation.

For example, a stack ADT supports operations such as:
- `push()` — add an item.
- `pop()` — remove the top item.
- `peek()` — inspect the top item.

A stack can be implemented using an array or a linked list. The ADT describes the behavior; the implementation describes how that behavior is achieved.

---

Q51–52. HTML — full form <br/>
**HTML = HyperText Markup Language.**

HTML defines the structure and meaning of content on a webpage using elements and tags.

Example:
```html
<h1>My School</h1>
<p>Welcome to our website.</p>
```
- `<h1>` represents a top-level heading.
- `<p>` represents a paragraph.

Remember the distinction:
- HTML — structure and content.
- CSS — presentation and styling.
- JavaScript — behavior and interactivity.
 
---
</details>
<!----------------------------->


<details>
  <summary> <b> PYQs 2023 </b> </summary>

<br/>


---
</details>
<!----------------------------->


<details>
  <summary> <b> PYQs 2020 </b> </summary>

<br/>

---
</details>
<!----------------------------->


<details>
  <summary> <b> PYQs 2019 </b> </summary>

<br/>

| Section 1 | General Knowledge and Other Skills |
|-----------|------------------------------------|

**Question 1. Bihari Puraskar, 2019** <br/>

Among the following, whom did the K. K. Foundation announce as the winner of the 28th Bihari Puraskar on May 16, 2019?**
- [x] A. Manisha Kulshreshtha
- [ ] B. Leeladhar Jagudi
- [ ] C. Keerti Parihar
- [ ] D. None of them

Correct answer: A. Manisha Kulshreshtha

The question concerns a literary award named after the Hindi poet Bihari. The Bihari Puraskar is one of the literary awards instituted by the K. K. Birla Foundation.

Concepts to remember
- Bihari Puraskar: A literary award associated with Hindi and Rajasthani literature.
- K. K. Birla Foundation: The organization associated with this award.
- Exam approach: For current-affairs questions, remember the award, winner, year and awarding organization together.

The Bihari Puraskar is primarily associated with which field?
- [ ] A. Sports
- [x] B. Literature
- [ ] C. Medicine
- [ ] D. Space research

Answer: B. Literature

---

**Question 2. 54th Jnanpith Award** <br/>

Original question: The 54th Jnanpith Award was given to which English writer in New Delhi on June 12, 2019?
- [ ] A. Sunil Shrivastava
- [x] B. Amitav Ghosh
- [ ] C. Yuvraj Bhattarai
- [ ] D. Leeladhar Jagudi

Correct answer: (B) Amitav Ghosh

Explanation: Amitav Ghosh is an Indian author who writes in English. He received the 54th Jnanpith Award for his contribution to Indian literature.

Concept to remember: The Jnanpith Award is a major Indian literary award. Amitav Ghosh is particularly associated with English-language literature.

Possible related questions

1. Amitav Ghosh is primarily known as a:
- [ ] (A) Scientist
- [x] (B) Author
- [ ] (C) Sportsperson
- [ ] (D) Economist

Answer: (B) Author

2. When studying literary awards, distinguish the award recipient from the language or literary tradition associated with that recipient.

---

**Question 3. Chief Election Commissioner of India**

Original question: Who was the Chief Election Commissioner of India at the time of the 2019 examination?
- [ ] (A) Ashok Lawasa
- [x] (B) Sunil Arora
- [ ] (C) Sushil Chandra
- [ ] (D) None of them

Correct answer: (B) Sunil Arora

Explanation: Sunil Arora served as India's Chief Election Commissioner from December 2018 to April 2021. Since this is a historical current-affairs question, answer it according to the time specified in the original paper, not the present officeholder.

Concept to remember: The Election Commission of India administers elections to Parliament, state legislatures, and the offices of the President and Vice-President.

Possible related questions

1. Which institution conducts elections to the Lok Sabha?
- [ ] (A) Supreme Court
- [x] (B) Election Commission of India
- [ ] (C) Finance Commission
- [ ] (D) Union Public Service Commission

Answer: (B) Election Commission of India

2. A common variation asks you to distinguish the Election Commission from the UPSC, Finance Commission and other constitutional bodies.

---

**Question 4. Minimum pension for small and marginal farmers**

Original question: The minimum pension provided to farmers attaining the age of 60 years to all small and marginal farmers by the Central Government from May 31, 2019, is:
- [ ] (A) Rs. 2,000 per month
- [x] (B) Rs. 3,000 per month
- [ ] (C) Rs. 4,000 per month
- [ ] (D) None of these

Answer: (B) Rs. 3,000 per month

Explanation: The Pradhan Mantri Kisan Maan-Dhan Yojana is a pension scheme for eligible small and marginal farmers. It provides a monthly pension of ₹3,000 after the eligible beneficiary reaches 60 years of age, subject to the scheme's conditions.

Possible related MCQs

1: At what age does the pension under this scheme begin?

(A) 55 years (B) 58 years (C) 60 years (D) 65 years

Answer: (C) 60 years

2: What is the stated monthly pension?

(A) ₹1,000 (B) ₹2,000 (C) ₹3,000 (D) ₹5,000

Answer: (C) ₹3,000

Exam tip: Remember the pair: 60 years -> ₹3,000 per month.

---

Question 5. Sudirman Cup 2019

Original question: The winner of the World Mixed Team Badminton Championship Sudirman Cup 2019 is:
- [ ] (A) India
- [x] (B) China
- [ ] (C) Japan
- [ ] (D) None of these

Answer: (B) China

Explanation: China won the 2019 Sudirman Cup, an international mixed-team badminton championship.

Possible related MCQs

1. The Sudirman Cup is associated with which sport?
- [ ] (A) Tennis
- [x] (B) Badminton
- [ ] (C) Hockey
- [ ] (D) Table tennis

Answer: (B) Badminton

2: Is the Sudirman Cup an individual or team championship? <br/>
Answer: Team championship.

Exam tip: Sports current affairs can test either the winner or the sport associated with a tournament.

---

**Question 6. Remainder theorem**

Original question: A number, when divided by 52, gives remainder 45. If the same number is divided by 13, the remainder will be:
- [ ] (A) 5
- [x] (B) 6
- [ ] (C) 12
- [ ] (D) 7
Answer: (B) 6

Explanation:
```
Let the number be N.
If dividing by 52 gives remainder 45, then N = 52k + 45
Since 52 = 13 times 4, the term 52k is divisible by 13.
Therefore, the remainder when N is divided by 13 is the remainder of 45 divided by 13:
45 = 13 times 3 + 6
So the answer is 6.
```

Possible related MCQs

1. A number leaves remainder 17 when divided by 24. What remainder does it leave when divided by 8?
```
Since 24 is divisible by 8, calculate 17 mod 8.

Answer: 1
```

2. A number leaves remainder 29 when divided by 36. What remainder does it leave when divided by 12?
```
Answer: 5, because 29 = 12 times 2 + 5 
```

Exam tip: If the original divisor is a multiple of the new divisor, reduce the original remainder modulo the new divisor.

---

**Question 7. Comparing radicals**

Original question: Which of the following is the largest number?
- [x] squareRoot 2
- [ ] cubeRoot 3
- [ ] quadRoot 4
- [ ] hexaRoot 6

Answer: squareRoot 2
| option       | approx val |
|--------------|-------|
| squareRoot 2 | 1.414 |
| cubeRoot 3   | 1.442 |
| quadRoot 4   | 1.414 |
| hexaRoot 6   | 1.348 |


Exam tip: When comparing radicals, estimate their decimal values or raise both positive quantities to a common power.

---

**Question 8. Ratio and LCM**

Original question: The ratio of two numbers is 3 : 4 and their LCM is 120. The sum of the numbers is:
- [x]  (A) 70
- [ ] (B) 35
- [ ] (C) 140
- [ ] (D) 105
      
Answer: (A) 70

Explanation:
```
Let the two numbers be 3x and 4x.
Since 3 and 4 are coprime,
LCM(3x,4x)=12x

Given: 12x = 120 -> x = 10
The numbers are 30 and 40.
30 + 40 = 70
```

Possible related MCQs

1. Two numbers are in the ratio 2 : 5 and their LCM is 70. Find their sum.
```
Their LCM is 10x = 70, so x = 7.
Numbers: 14 and 35.
Answer: 49
```

2. Two numbers are in the ratio 3 : 5 and their HCF is 4. Find their sum.
```
Numbers: 12 and 20.
Answer: 32
```

Exam tip: For a ratio a:b, when a and b are coprime, the LCM of ax and bx is abx.

---


**Question 9. Percentage**

Original question: When 60 is subtracted from 60% of a number, the result is 60. The number is:
- [ ] (A) 120
- [ ] (B) 150
- [ ] (C) 180
- [x] (D) 200

Answer: (D) 200? Let's calculate carefully.
```
Let the number be x
0.60x - 60 = 60
Add 60 to both sides
0.60x = 120
    x = 120 / 0.60    
    x = 200
```

Possible related MCQs

1. When 20 is subtracted from 50% of a number, the result is 30. Find the number.
```
0.5x - 20 = 30
0.5x  =  50
   x  = 50 / 0.5
   x  = 100

Answer = 100
```

2. If 25% of a number is 45, what is the number?
```
  x = 45 / 0.25
  x = 4500 / 25
  x = 180
```

Exam tip: Translate the wording into an equation before calculating. `"60 is subtracted from 60% of a number"` means `0.60x - 60` not `0.60(x-60)`

---

**Q10. Profit and Loss**

Question: If the cost price of 15 books is equal to the selling price of 20 books, what is the loss percentage? <br/>
- [ ] (A) 16%
- [ ] (B) 20%
- [ ] (C) 24%
- [x] (D) 25%

Correct answer: (D) 25%

Explanation:
```
Let the cost price of one book be ₹1.
- Cost price of 15 books = ₹15
- Selling price of 20 books = ₹15
- Selling price of one book = ₹15 ÷ 20 = ₹0.75
- Loss per book = ₹1 − ₹0.75 = ₹0.25
```

```
Loss % = 0.25 / 1 x 100 = 25 %
```

Remember: When the cost price of 15 items equals the selling price of 20 items, the loss is 25%.

---

**Q11. Average**

Question: The average of 20 numbers is 15, and the average of the first five numbers is 12. Find the average of the remaining numbers.
- [x] (A) 16
- [ ] (B) 15
- [ ] (C) 14
- [ ] (D) 13

Correct answer: (A) 16

Explanation:
```
Total of 20 numbers = 20 x 15 = 300
Total of the first five numbers = 5 x 12 = 60
Total of the remaining 15 numbers = 300 - 60 = 240

Required Average = 240 / 15 = 16
```
Remember: Average = Total sum ÷ Number of items.

---

**Q12. Ratio and Proportion**

Question: If A:B = 3:4, B:C = 5:7, and C:D = 8:9, find A:D. <br/>
- [ ] (A) 3:7
- [ ] (B) 7:3
- [ ] (C) 21:10
- [x] (D) 10:21

Correct answer: (D) 10:21

Explanation:
```
Make the common terms equal step by step.
From A:B = 3:4 and B:C = 5:7, make B = 20:
       A:B:C = 15:20:28

Now combine C=28 with C:D=8:9. The LCM of 28 and 8 is 56,
so:  A:B:C:D = 30:40:56:63
Therefore  A:D = 30:63 = 10:21
```

---

**Q13. Mensuration - Rectangle and Square**

Question: The perimeter of a rectangle is 160 metres, and the difference between its two sides is 48 metres. Find the side of a square whose area equals the area of this rectangle.
- [x] (A) 32 m
- [ ] (B) 8 m
- [ ] (C) 4 m
- [ ] (D) 16 m

Correct answer: (A) 32 m

Explanation:
```
Let the rectangle's length be l and breadth be b.
           2(l + b) = 160 ->  l + b = 80
Given l - b = 48.
Solving these equations: l = 64, b = 16
Rectangle's area: l x b = 64 x 16 = 1024 m^2

If the square has the same area, its side is: sqrtRoot(1024) = 32m
```
Remember: Square area = side².

---


**Q14. Speed, Time and Distance**

Question: A man walking at a speed of 5 km/hour crosses a bridge in 15 minutes. What is the length of the bridge?
- [ ] (A) 600 m
- [ ] (B) 750 m
- [ ] (C) 1000 m
- [x] (D) 1250 m

Correct answer: (D) 1250 m
```
Explanation:

Convert 15 minutes into hours:  15 / 60 = 0.25 hours
Distance = Speed × Time
          = 5 x 0.25 = 1.25 km
                     = 1250 m
```
Exam tip: Convert hours to minutes or kilometres to metres before selecting your answer.

---

**Q15. Trigonometry**

Question: If A is an acute angle and cot A+cosec A=3, find sin A.
- [ ] (A) 1
- [ ] (B) 4/5
- [x] (C) 3/5
- [ ]  (D) 0

Correct answer: (C) 3/5

Explanation:
```
Use the identity: cosecA + cotA= (1 + cosA) / sinA

Given: (1 + cos A)/ sinA = 3
So, (1 + cosA) = 3 sin A
The acute angle solution is cos A = 4/5 and sin A = 3/5.
Checking: 4/5 + 1 = 3 x 3/5
Both sides equal 9/5.
Therefore, sin A = 3/5.
```

---


**Q16. Blood Relations**

Question: Pointing towards Garima, Rakesh said, "His father is the only son of my father." How is Rakesh related to Garima?
- [ ] (A) Brother
- [x] (B) Father
- [ ] (C) Uncle
- [ ] (D) None of them

Correct answer: (B) Father

Explanation:
- "The only son of my father" refers to Rakesh himself, assuming he is the only son.
- The statement says Garima's father is Rakesh.
Therefore, Rakesh is Garima's father.


---

Q17. Direction Sense
Question: Samir walks 15 metres west from his house, turns left and walks 20 metres, then turns east and walks 25 metres. Finally, he turns left and walks 20 metres. How far is he from his house?
- [ ] (A) 5 m
- [x] (B) 10 m
- [ ] (C) 40 m
- [ ] (D) 80 m

Correct answer: (B) 10 m

Explanation:

Track his movements:
- West: 15 m
- Left from west means south: 20 m
- East: 25 m
- Left from east means north: 20 m
The south and north movements cancel each other. Horizontally, he walks 15 m west and 25 m east.

```
25 - 15 = 10
```

---

**Q18. Coding-Decoding**

Question: In a certain coding language, DEEP is written as 60 and RABIT as 100. How will HAIR be written?
- [ ] (A) 27
- [x] (B) 72
- [ ] (C) 90
- [ ] (D) 160

Correct answer: (B) 72

Explanation:

The pattern is twice the sum of the letters' alphabetical positions.


```
For DEEP:
D(4) + E(5) + E(5) + P(16) = 30
30 x 2 = 60

For RABIT:
R(18) + A(1) + B(2) + I(9) + T(20) = 50
50 x 2 = 100

Apply the same rule to HAIR:
H(8) + A(1) + I(9) + R(18) = 36
36 x 2 = 72
```

---

**Q19. Mathematical Operator Substitution**

Question: If the symbols are reassigned as specified in the paper, solve: ` 8 / 4 x 2 - 4 + 2 = ?`
- [ ] (A) 2
- [ ] (B) 28
- [x] (C) 32
- [ ]  (D) 36

Correct answer: (C) 32

Explanation: According to the operator substitutions in the question:
- `/` means multiplication
- `x` means subtraction
- `-` means addition
- `+` means division

```
8 / 4 x 2 - 4 + 2 = ?
Replace the operators:
8 x 4 - 2 + 4 / 2
Apply BODMAS:
32 - 2 + 2
```

Exam tip: Always replace the operators first, then apply the order of operations.

---

**Q20. Number Pattern**

Question: Find the missing number in the figure containing 8, 27, 64, 125, 216 and a missing value.
- [ ] (A) 4
- [ ] (B) 305
- [x] (C) 343
- [ ] (D) 729

Correct answer: (C) 343

Explanation: These are consecutive cubes:
```
2^3 = 8
3^3 = 27
4^3 = 64
5^3 = 125
6^3 = 216
7^3 = 343
```

Remember: Recognising square and cube number patterns is useful in reasoning questions.

---

**Q21. Letter Series**

Question: Which option completes the series?

JAK, KBL, LCM, MDN, ?
- [ ] (A) OEP
- [x] (B) NEO
- [ ] (C) MEN
- [ ] (D) PFQ

Correct answer: (B) NEO

Explanation: Examine each letter position separately:
- First letters:  J, K, L, M, --> N
- Second letters: A, B, C, D, --> E
- Third letters:  K, L, M, N, --> O
Each letter advances by one position in the alphabet.

Answer: NEO.

---

**Q22. Number Series**

Question: Find the next number: `16, 23, 31, 40, 50, 61, ?`
- [x] (A) 73
- [ ] (B) 77
- [ ] (C) 83
- [ ] (D) 81

Correct answer: (A) 73

Explanation: Calculate the differences:
```
Numbers	     Difference
16 -> 23	      +7
23 -> 31      	+8
31 -> 40	      +9
40 -> 50	      +10
50 -> 61	      +11
61 -> ?         +12
   61 + 12 = 73
```

---

**Q23. Counting Triangles**

Question: How many triangles are there in the given figure?
- [x] (A) 16
- [ ] (B) 15
- [ ] (C) 9
- [ ] (D) 7

Answer indicated in the paper: (A) 16

Explanation: This is a visual-reasoning question. Count the smallest triangles first, then count the larger triangles formed by combining smaller ones. Be careful not to count the same triangle more than once.

The paper's indicated answer is 16.

---

**Q24. Coding-Decoding — Word Substitution**

Question: If "Sand" is coded as "Brick", "Brick" as "House", "House" as "Temple", and "Temple" as "Palace", where do you worship?
- [x] (A) Palace
- [ ] (B) Temple
- [ ] (C) Brick
- [ ] (D) House

Correct answer: (A) Palace

Explanation: You worship at a temple. According to the given code, Temple is called Palace.

Therefore, the answer is Palace.

Exam tip: Answer according to the given code, not the ordinary meaning of the word.

---

**Q25. Letter Coding**

Question: If LIGHT is coded as JGEFR, how will SHORT be coded?
- [ ] (A) FQMPR
- [x] (B) QFMPR
- [ ] (C) FQMRP
- [ ] (D) QFMRP

Correct answer: (B) QFMPR

Explanation: Each letter in LIGHT is shifted two positions backwards:
- L -> J
- I -> G
- G -> E
- H -> F
- T -> R
Apply the same rule to SHORT:
- S -> Q
- H -> F
- O -> M
- R -> P
- T -> R
So, SHORT becomes QFMPR.

---

**Q26. Indian Constitution**

Question: Who said, "The Principles (Directive Principles) should be made the basis of all the future legislation?"
- [ ]  (A) Pt. Jawaharlal Nehru
- [x] (B) Dr. B. R. Ambedkar
- [ ] (C) Dr. B. N. Rao
- [ ] (D) Dr. Zakir Husain

Answer indicated in the paper: (B) Dr. B. R. Ambedkar

Concept: Directive Principles of State Policy are guidelines for the government, set out in Part IV of the Indian Constitution. They are not directly enforceable by courts.

---

**Q27. Solar System**

Question: Which of the following does not belong to the solar system?
- [ ] (A) Planets
- [ ] (B) Comets
- [ ] (C) Asteroids
- [x] (D) Nebulae

Expected answer: (D) Nebulae

Explanation: Planets, comets, and asteroids are all members of our solar system. A nebula is a cloud of gas and dust in space, generally associated with interstellar space rather than being a standard solar-system body.

---

**Q28. Plant Adaptations**

Question: Plants that grow in saline soil are known as what?
- [ ] (A) Xerophytes
- [ ] (B) Hydrophytes
- [ ] (C) Succulents
- [x] (D) Halophytes

Correct answer: (D) Halophytes

Explanation:
- Xerophytes: Adapted to dry environments.
- Hydrophytes: Adapted to aquatic environments.
- Succulents: Store water in fleshy tissues.
- Halophytes: Tolerate high salt concentrations.

Example: mangrove plants.

---

**Q29. Light and Prisms**

Question: Which colour of light undergoes the least deviation while passing through a prism?
- [x] (A) Red
- [ ] (B) Green
- [ ] (C) Yellow
- [ ] (D) Blue

Correct answer: (A) Red

Explanation: In ordinary glass, red light has a longer wavelength and refracts less than blue or violet light. Therefore, red deviates the least.

Remember: Red = least deviation; violet = greatest deviation.

---

**Q30. Astronomy**

Question: The world's largest telescope is in which country?
- [ ] (A) India
- [ ]  (B) Japan
- [x]  (C) China
- [ ]  (D) United States of America

Answer expected for the 2019 paper: (C) China

Explanation: China operates FAST, the Five-hundred-meter Aperture Spherical Telescope, a giant single-dish radio telescope. The phrase "largest telescope" can depend on the type of telescope and the measurement used.

---

**Q31. Environment**

Question: World Environment Day is celebrated on which date?
- [x] (A) 5 June
- [ ] (B) 5 July
- [ ] (C) 5 May
- [ ] (D) 5 March

Correct answer: (A) 5 June

Explanation: World Environment Day is observed annually on 5 June to promote environmental awareness and action.

---

**Q32. Light and Fog**

Question: For which of the following causes can we not see clearly during fog?
- [x] (A) Scattering of light
- [ ] (B) Reflection
- [ ] (C) Internal reflection
- [ ] (D) Refraction

Correct answer: (A) Scattering of light

Explanation: Tiny water droplets in fog scatter light in different directions. This reduces visibility and makes distant objects difficult to see.

---

**Q33. Computer Storage Units**

Question: Which of the following represents a billion characters?
- [ ] (A) Kilobytes
- [x] (B) Gigabytes
- [ ] (C) Terabytes
- [ ] (D) Megabytes

Expected answer: (B) Gigabytes

Explanation: Roughly, one gigabyte corresponds to about one billion bytes in decimal units. Since one character commonly occupies one byte in simple encodings, a gigabyte is approximately a billion characters.

Important: The scan's handwritten mark appears to indicate option C, but that is inconsistent with the usual storage-unit conversion. The wording is approximate, so remember the distinction between decimal and binary units.

---

**Q34. Ancient Indian History**

Question: What was the early capital of Magadh?
- [ ] (A) Vaishali
- [ ] (B) Champa
- [x] (C) Rajgriha (Girivraj)
- [ ] (D) Pataliputra

Correct answer: (C) Rajgriha (Girivraj)

Explanation: Rajagriha, also called Girivraja, was an early capital of the Magadha kingdom. Pataliputra became its capital later.

---

**Q35. Environmentally Friendly Fuel**

Question: Among the following energy fuels, which is the most environmentally friendly?
- [ ] (A) Biogas
- [ ] (B) Ethanol
- [ ] (C) CNG
- [x] (D) Hydrogen

Expected answer: (D) Hydrogen

Explanation: Hydrogen can produce water as its main product when used in a fuel cell, without direct carbon dioxide emissions at the point of use. Its overall environmental impact depends on how the hydrogen is produced.

---

**Q36. World Wetlands Day**

Question: On which day is World Wetlands Day celebrated?
- [ ] (A) 2 March
- [ ] (B) 22 March
- [x] (C) 2 February
- [ ] (D) 22 May

Correct answer: (C) 2 February

Explanation: World Wetlands Day is observed annually on 2 February to raise awareness about the importance of wetlands and their conservation.

---

**Q37. Sports**

Question: The Durand Cup is associated with which sport?
- [ ] (A) Polo
- [x] (B) Football
- [ ] (C) Cricket
- [ ] (D) Hockey

Correct answer: (B) Football

Explanation: The Durand Cup is a major football tournament in India and is among the oldest football competitions in Asia.

---

**Q38. Indian Freedom Movement**

Question: Who said, “Swaraj is my birthright and I shall have it”?
- [ ] (A) Mahatma Gandhi
- [ ] (B) Bhagat Singh
- [ ] (C) Jawaharlal Nehru
- [x] (D) Bal Gangadhar Tilak

Correct answer: (D) Bal Gangadhar Tilak

Explanation: Bal Gangadhar Tilak popularised this famous slogan during India’s struggle for independence. Swaraj means self-rule.

---

**Q39. Indian Constitution**

Question: In the Constitution of India, the Right to Free and Compulsory Elementary Education is included in which section?
- [ ] (A) Human Rights
- [x] (B) Fundamental Rights of citizens
- [ ] (C) Directive Principles of State Policy
- [ ] (D) None of these

Correct answer: (B) Fundamental Rights of citizens

Explanation: Article 21A provides free and compulsory education for children aged 6–14 years as a Fundamental Right.

---

**Q40. Human Biology**

Question: What is the number of chromosomes in the human body?
- [ ] (A) 48
- [x] (B) 46
- [ ] (C) 44
- [ ] (D) 42

Correct answer: (B) 46

Explanation: Most human body cells contain 46 chromosomes, arranged in 23 pairs. Human reproductive cells typically contain 23 chromosomes.

---

**Q41. Indian Parliament**

Question: The Speaker of the Lok Sabha in India is elected by whom?
- [ ] (A) Council of Ministers
- [ ] (B) All Speakers of State Legislative Assemblies
- [x] (C) Members of Lok Sabha
- [ ] (D) Members of Lok Sabha and Rajya Sabha

Correct answer: (C) Members of Lok Sabha

Explanation: The Lok Sabha elects its Speaker from among its own members.

---

**Q42. Geography — Ocean Salinity**

Question: Which of the following is a major source of oceanic salinity?
- [ ] (A) Land
- [x] (B) Rivers
- [ ] (C) Ash from volcanoes
- [ ] (D) Wind

Answer indicated in the paper: (B) Rivers

Explanation: Rivers carry dissolved minerals and salts from rocks and land into the oceans. Over time, these contribute to ocean salinity.

Exam note: Rivers transport dissolved salts, but the broader geological process of weathering and the movement of minerals is important to understanding ocean salinity.

---

**Q43. Important Straits**

Question: Which strait connects the Red Sea and the Indian Ocean?
- [ ] (A) Malacca
- [ ] (B) Bosporus
- [ ] (C) Hormuz
- [x] (D) Bab-el-Mandeb

Correct answer: (D) Bab-el-Mandeb

Explanation: The Bab-el-Mandeb Strait connects the Red Sea with the Gulf of Aden, which opens into the Indian Ocean.
- Malacca: Connects the Andaman Sea region with the South China Sea.
- Bosporus: Connects the Black Sea with the Sea of Marmara.
- Hormuz: Connects the Persian Gulf with the Gulf of Oman.

---

**Q44. Indus Valley Civilization**

Question: Which of the following is a Harappan port?
- [ ] (A) Mahasthangarh
- [ ] (B) Nagapattinam
- [x] (C) Lothal
- [ ] (D) None of these

Correct answer: (C) Lothal

Explanation: Lothal, located in present-day Gujarat, was an important settlement of the Indus Valley Civilization and is well known for its dockyard or port-related structure.

---

**Q45. Indian Constitution**

Question: At present, the Constitution of India comprises:
- [x] (A) 465 Articles, 25 Parts and 12 Schedules
- [ ] (B) 395 Articles, 25 Parts and 8 Schedules
- [ ] (C) 372 Articles, 22 Parts and 12 Schedules
- [ ] (D) None of these

Answer indicated in the paper: (A)

---

**Q46. Solar Cells**

Question: Which of the following is not used in making solar cells?
- [ ] (A) Silicon
- [x] (B) Platinum
- [ ] (C) Gallium
- [ ] (D) Germanium

Expected answer: (B) Platinum

Explanation: Silicon is the most common semiconductor material used in conventional solar cells. Gallium-based and germanium-based materials are also used in certain specialised photovoltaic technologies. Platinum is not a standard solar-cell semiconductor material.

---

**Q47. Right to Equality**

Question: Which Article of the Constitution of India is related to the Right to Equality before law?
- [ ] (A) Article 15
- [x] (B) Article 14
- [ ] (C) Article 16
- [ ] (D) Article 17

Correct answer: (B) Article 14

Explanation: Article 14 guarantees equality before the law and equal protection of the laws.

Quick revision:
- Article 14 — Equality before law
- Article 15 — Prohibition of discrimination
- Article 16 — Equality of opportunity in public employment
- Article 17 — Abolition of untouchability

---

**Q48. Computer Fundamentals**

Question: The brain of any computer is:
- [ ] (A) ALU
- [x] (B) CPU
- [ ] (C) Memory
- [ ] (D) Control Unit (CU)

Correct answer: (B) CPU

Explanation: The Central Processing Unit executes instructions and coordinates computer operations. The ALU performs arithmetic and logical operations, while the Control Unit directs and coordinates execution.

---

**Q49. Sound**

Question: At constant temperature, the speed of sound is maximum in which of the following gases?
- [x] (A) Hydrogen
- [ ] (B) Nitrogen
- [ ] (C) Oxygen
- [ ] (D) Equal in all these gases

Correct answer: (A) Hydrogen

Explanation: At the same temperature, sound travels faster in a gas with a lower molecular mass, assuming comparable conditions. Hydrogen has a much lower molecular mass than nitrogen or oxygen.

---

**Q50. National Emergency**

Question: A National Emergency may be declared by the President of India under which Article?
- [x] (A) Article 352
- [ ] (B) Article 370 
- [ ] (C) Article 371
- [ ] (D) Article 395

Correct answer: (A) Article 352

Explanation: Article 352 of the Indian Constitution deals with the proclamation of a National Emergency.

---

**Q51. UNIVAC**

Question: UNIVAC is:
- [x] (A) Universal Automatic Computer
- [ ] (B) Universal Array Computer
- [ ] (C) Unique Automatic Computer
- [ ] (D) Unvalued Automatic Computer

Correct answer: (A) Universal Automatic Computer

Explanation: UNIVAC stands for Universal Automatic Computer. It was an early commercial computer system.

---

**Q52. Basic Operations of a Computer**

Question: The basic operations performed by a computer are:
- [ ] (A) Arithmetic operation
- [ ] (B) Logical operation
- [ ] (C) Storage and retrieval
- [x] (D) All of these

Correct answer: (D) All of these

Explanation: A computer performs arithmetic and logical operations and stores and retrieves data. Together, these are fundamental computer operations.

---

**Q53. Difference Engine**

Question: Who is the inventor of the Difference Engine?
- [ ] (A) Allen Turing
- [x] (B) Charles Babbage
- [ ] (C) Seymour Cray
- [ ] (D) Augusta Ada Lovelace

Correct answer: (B) Charles Babbage

Explanation: Charles Babbage designed the Difference Engine, a mechanical calculating machine. Ada Lovelace is associated with early work on programming and the Analytical Engine.

---

**Q54. Computer Generations**

Question: Microprocessors as switching devices are associated with which generation of computers?
- [ ] (A) First Generation
- [ ] (B) Second Generation
- [ ] (C) Third Generation
- [x] (D) Fourth Generation

Correct answer: (D) Fourth Generation

Explanation: The fourth generation of computers is characterised by microprocessors built using large-scale and very-large-scale integration (LSI/VLSI) technology.

Quick revision of computer generations:
| Generation	| Main technology           |
|-------------|---------------------------|
| First	      | Vacuum tubes              |
| Second	    | Transistors               |
| Third	      | Integrated circuits (ICs) |
| Fourth	    | Microprocessors           |

---

**Q55. DOS**

Question: DOS stands for:
- [x] (A) Disk Operating System
- [ ] (B) Disk Operating Session
- [ ] (C) Digital Operating System
- [ ] (D) Digital Open System

Correct answer: (A) Disk Operating System

Explanation: DOS is an operating system used to manage files, disks, and computer operations. MS-DOS is a well-known example.

---

**Q56. Character Encoding — EBCDIC**

Question: ASCII and EBCDIC are popular character-coding systems. What does EBCDIC stand for?
- [x] (A) Extended Binary Coded Decimal Interchange Code
- [ ] (B) Extended Bit Code Decimal Interchange Code
- [ ] (C) Extended Bit Case Decimal Interchange Code
- [ ] (D) Extended Binary Case Decimal Interchange Code

Correct answer: (A) Extended Binary Coded Decimal Interchange Code

Explanation: EBCDIC is an 8-bit character encoding developed by IBM. It is associated particularly with IBM mainframe systems.

Quick revision:
- **`ASCII`**: American Standard Code for Information Interchange.
- **`EBCDIC`**: Extended Binary Coded Decimal Interchange Code.

---

**Q57. Father of the Computer**

Question: Who is the father of the computer?
- [ ] (A) Alan Turing
- [ ] (B) Seymour Cray
- [ ] (C) Augusta Ada Lovelace
- [x] (D) Charles Babbage

Correct answer: (D) Charles Babbage

Explanation: Charles Babbage is widely known as the father of the computer for his designs of mechanical computing machines, including the Difference Engine and Analytical Engine.

---

**Q58. Magnetic Disk Storage Capacity**

Question: The storage capacity of a magnetic disk depends on:
- [ ] (A) Tracks per inch of surface
- [ ] (B) Bits per inch of tracks
- [ ] (C) Disk pack and disk surface
- [x] (D) All of these

Correct answer: (D) All of these

Explanation: Disk capacity depends on how densely data can be recorded and how many recording surfaces and tracks are available.

Remember: More tracks and higher recording density generally mean greater storage capacity.

---

**Q59. Main Memory**

Question: The two kinds of main memory are:
- [ ] (A) Primary and Secondary
- [ ] (B) Random and Sequential
- [x] (C) ROM and RAM
- [ ] (D) All of these

Correct answer expected by the paper: (C) ROM and RAM

Explanation: In the terminology used by this question, main memory is divided into RAM and ROM.
- RAM: Read/write working memory; typically volatile.
- ROM: Non-volatile memory used to store persistent instructions or firmware.

Note that "primary and secondary" refers to a broader distinction between storage categories, rather than the two types intended here.

---

**Q60. Buffer**

Question: A storage area used to store data to compensate for differences in the speeds at which different units can handle data is called:
- [ ] (A) Memory
- [x] (B) Buffer
- [ ] (C) Accumulator
- [ ] (D) Address

Correct answer: (B) Buffer

Explanation: A buffer temporarily holds data while it moves between devices or processes operating at different speeds.

Example: A printer buffer holds print data while the printer processes it.

---

**Q61. Characteristics of a Computer**

Question: A computer is free from tiresomeness and boredom. We call this:
- [ ] (A) Accuracy
- [ ] (B) Reliability
- [x] (C) Diligence
- [ ] (D) Versatility

Correct answer: (C) Diligence

Explanation: Diligence means a computer can repeatedly perform tasks without becoming tired or bored.

Keep these terms distinct:
- Accuracy: Produces correct results when given correct data and instructions.
- Reliability: Performs consistently.
- Diligence: Does not tire or lose concentration.
- Versatility: Can perform different types of tasks.

---

**Q62. Computer Generations — Integrated Circuits**

Question: Integrated Circuits (ICs) are related to which generation of computers?
- [ ] (A) First generation
- [ ] (B) Second generation
- [x] (C) Third generation
- [ ] (D) Fourth generation

Correct answer: (C) Third generation

Explanation: Third-generation computers used integrated circuits, replacing many individual transistors with compact circuits containing multiple electronic components.

---

**Q63. CD-ROM**

Question: CD-ROM is a:
- [ ] (A) Semiconductor memory
- [ ] (B) Memory register
- [ ] (C) Magnetic memory
- [x] (D) None of these

Correct answer: (D) None of these

Explanation: A CD-ROM is an optical storage medium. It stores data that is read using a laser, rather than using semiconductor memory or magnetic recording.

---

**Q64. Hybrid Computer**

Question: A hybrid computer:
- [ ] (A) Resembles a digital computer
- [ ] (B) Resembles an analogue computer
- [x] (C) Combines features of both digital and analogue computers
- [ ] (D) None of these

Correct answer: (C) Combines features of both digital and analogue computers

Explanation: Hybrid computers combine analogue processing, which can handle continuous signals, with digital processing, which handles discrete data.

Example: Certain specialised medical monitoring and industrial control systems use hybrid-computing principles.

---

**Q65. EBCDIC and Computer Types**

Question: Which type of computer uses the 8-bit code called EBCDIC?
- [ ] (A) Minicomputers
- [ ] (B) Microcomputers
- [x] (C) Mainframe computers 
- [ ] (D) Supercomputer

Correct answer: (C) Mainframe computers

Explanation: EBCDIC is historically associated with IBM mainframe computer systems.

---

**Q66. Arithmetic Logic Unit (ALU)**

Question: The ALU of a computer responds to commands coming from the:
- [ ] (A) Primary memory
- [x] (B) Control section
- [ ] (C) External memory
- [ ] (D) Cache memory

Correct answer: (B) Control section

Explanation: The Control Unit directs the execution of instructions and coordinates operations. The ALU carries out arithmetic calculations and logical comparisons as directed.

---

**Q67. First-Generation Computers**

Question: The chief component of first-generation computers was:
- [ ] (A) Transistors
- [x] (B) Vacuum tubes and valves
- [ ] (C) Integrated circuits
- [ ] (D) None of these

Correct answer: (B) Vacuum tubes and valves

Explanation: First-generation computers relied on vacuum tubes for electronic switching and processing. They were generally large, power-hungry, and produced considerable heat.

---

**Quick revision**
| Topic	                 | Key fact                                       |
|------------------------|------------------------------------------------|
| DOS	                   | Disk Operating System                          |
| EBCDIC	               | Extended Binary Coded Decimal Interchange Code |
| Father of the computer | Charles Babbage                                |
| Buffer	               | Bridges differences in data-transfer speeds    |
| Diligence	             | Computer does not tire or get bored            |
| Third generation	     | Integrated circuits (IC)                       |
| CD-ROM	               | Optical storage                                |
| Hybrid computer	       | Analogue + digital                             |
| First generation	     | Vacuum tubes                                   |

---

**Q68. Computer Network**

Question: A combination of hardware and software that facilitates the sharing of information between computing devices is called:
- [x] (A) Network
- [ ] (B) Peripheral
- [ ] (C) Expansion board
- [ ] (D) Digital device

Correct answer: (A) Network

Explanation: A computer network connects devices so they can exchange information and share resources such as files, printers, and internet access.

---

**Q69. Byte**

Question: 1 Byte = ?
- [x] (A) 8 bits
- [ ] (B) 4 bits
- [ ] (C) 2 bits
- [ ] (D) 9 bits

Correct answer: (A) 8 bits

Explanation: One byte contains eight bits. `1 Byte = 8 bits`

A bit is a binary digit, either 0 or 1.

---

**Q70. Integrated Circuits**

Question: Which of the following ICs were used in the third generation of computers?
- [ ] (A) SSI
- [ ] (B) MSI
- [ ] (C) LSI
- [x] (D) Both (A) and (B)

Correct answer: (D) Both (A) and (B)

Explanation: Third-generation computers used integrated circuits, including small-scale integration (SSI) and medium-scale integration (MSI).
- SSI: Small-Scale Integration
- MSI: Medium-Scale Integration
- LSI: Large-Scale Integration

---

**Q71. Data Structure**

Question: The term Data Structure refers to ______ and the interrelationship between them.
- [x] (A) Organization of data
- [ ] (B) Programming standard
- [ ] (C) Coding
- [ ] (D) Program design

Correct answer: (A) Organization of data

Explanation: A data structure organises data and defines how data items relate to one another.

Examples include arrays, linked lists, stacks, queues, trees, and graphs.

---

**Q72. Types of Data**

Question: In data structure, data may be of ______ types.
- [ ] (A) 1
- [ ] (B) 2
- [ ] (C) 3
- [x] (D) 4

Answer indicated in the paper: (D) 4

Important note: The question does not specify a classification scheme. Data types can be classified in different ways depending on the programming language or textbook, so the number four should be treated as the paper's expected answer rather than a universal rule.

---

**Q73. Global Variables**

Question: Variables that can be accessed by all modules of a program are called:
- [x] (A) Global
- [ ] (B) Auto
- [ ] (C) Static
- [ ] (D) Local

Correct answer: (A) Global

Explanation: A global variable is declared outside individual functions or local scopes and can be accessed from multiple parts of a program, subject to the language's scope rules.

By contrast, a local variable is accessible only within its defined scope.

---

**Q74. Implementing Stack, Queue and Linked List**

Question: Stack, Queue and Linked List can be implemented using:
- [ ] (A) Numeric variable
- [ ] (B) String variable
- [ ] (C) Logical function
- [x] (D) Array

Correct answer: (D) Array

Explanation: Arrays can be used to implement stacks and queues, and they can also be used to represent linked-list-like structures using index links. In typical implementations, linked lists instead use nodes connected through pointers or references.

Remember: Stacks and queues can be implemented using either arrays or linked lists.

---

**Q75. Hyperlinks**

Question: Hyperlinks can be created between a Word document and:
- [ ] (A) Another Word document
- [ ] (B) A webpage on the World Wide Web
- [ ] (C) A webpage on a company intranet
- [x] (D) All of these
Correct answer: (D) All of these

Explanation: A hyperlink can connect a Word document to another document, an internet webpage, or an intranet resource.

---

**Q76. Inserting Clip Art**

Question: You can insert Clip Art from:
- [ ] (A) Insert → Pictures → Clip Art
- [x] (B) The Clip Art icon on the Drawing toolbar
- [ ] (C) All of these
- [ ] (D) None of these

Answer indicated in the paper: (B) The Clip Art icon on the Drawing toolbar

Explanation: The question refers to older versions of Microsoft Word, where Clip Art could be inserted through the Drawing toolbar. Menus and features differ in modern versions of Word.

---

**Q77. Document Versioning**

Question: Which of the following cannot be done with document versioning?
- [x] (A) Modifying a version
- [ ] (B) Deleting a version
- [ ] (C) Opening a version
- [ ] (D) None of these

Answer indicated in the paper: (A) Modifying a version

Explanation: In traditional document-versioning features, saved versions can be opened or deleted, while an existing saved version may not be directly editable as a separate version. The precise behaviour depends on the software and version being used.

---

**Q78. Dragging Selected Text**

Question: When you drag selected text, you can:
- [ ] (A) Delete text
- [ ] (B) Link text
- [ ] (C) Copy text
- [x] (D) Move text

Correct answer: (D) Move text

Explanation: In typical Word drag-and-drop editing, dragging selected text to another location moves it there. Special modifier keys or settings can change the behaviour to copying.

---

**Q79. Searching in a Word Document**

Question: You can search in a Word document for:
- [ ] (A) Formatting
- [ ] (B) Special characters
- [ ] (C) Phrases
- [x] (D) All of these
Correct answer: (D) All of these

Explanation: Word's Find and advanced Find features support searching for text, phrases, and certain special characters or formatting attributes.

---

**Q80. Adding a Date to a Document**

Question: You can add a date to a document by:
- [ ] (A) Inserting a text date
- [ ] (B) Inserting a date field that updates automatically
- [ ] (C) Typing the date manually
- [x] (D) All of these

Correct answer: (D) All of these

Explanation: You can type a date directly, insert a date as ordinary text, or insert a date field that can update automatically.

For example, a date field is useful when a document should display the current date when updated or printed.

---

| Keyboard Shortcuts, Data Structures and OOP |
|---------------------------------------------|

---

**Q81. End Key**

Question: The End key is used to:
- [x] (A) Move the cursor to the end of the line
- [ ] (B) Move the cursor to the end of the document
- [ ] (C) Move the cursor to the end of the paragraph
- [ ] (D) Move the cursor to the end of the screen

Correct answer: (A) Move the cursor to the end of the line

Explanation: In standard text-editing applications such as Microsoft Word, pressing End moves the cursor to the end of the current line.

Remember:
- `Home` → Beginning of the line
- `End` → End of the line
- `Ctrl + Home` → Beginning of the document
- `Ctrl + End` → End of the document

---

**Q82. `Ctrl + Page Down`**

Question: `Ctrl + Page Down` is used to:
- [ ] (A) Move the cursor one paragraph down
- [x] (B) Move the cursor one page down
- [ ] (C) Move the cursor one line down
- [ ] (D) Move the cursor one screen down

Answer indicated in the paper: (B) Move the cursor one page down

Explanation: In older Microsoft Word versions, `Ctrl + Page Down` moves to the next page or browsing location, depending on the version and navigation context. It is not the same as moving down one line.

---

**Q83. `Ctrl + Down Arrow`**

Question: `Ctrl + Down Arrow` is used to:
- [x] (A) Move the cursor one paragraph down
- [ ] (B) Move the cursor one line down
- [ ] (C) Move the cursor one page down
- [ ] (D) Move the cursor one screen down

Correct answer: (A) Move the cursor one paragraph down

Explanation: In Microsoft Word, `Ctrl + Down Arrow` moves the insertion point to the beginning of the next paragraph.

Exam tip: Do not confuse the `Down Arrow` with `Ctrl + Down Arrow`.

---

**Q84. Non-Linear Data Structure**

Question: Which one is a non-linear data structure?
- [ ] (A) Stack
- [ ] (B) Queue
- [ ] (C) Linked list
- [x] (D) Tree

Correct answer: (D) Tree

Explanation:
- Stack: Linear data structure; follows LIFO.
- Queue: Linear data structure; follows FIFO.
- Linked list: Usually classified as linear.
- Tree: Non-linear data structure with hierarchical relationships.
Examples of trees include binary trees, binary search trees, and heaps.

---

**Q85. `Ctrl + Left Arrow`**

Question: `Ctrl + Left Arrow` is used to:
- [ ] (A) Move the cursor to the beginning of the line
- [x] (B) Move the cursor one word left
- [ ] (C) Move the cursor one paragraph up
- [ ] (D) Move the cursor one paragraph down

Correct answer: (B) Move the cursor one word left

Explanation: `Ctrl + Left Arrow` moves the cursor to the previous word boundary in most text editors.

Compare:
- `Left Arrow` → Move left one character.
- `Ctrl + Left Arrow` → Move left one word boundary.
- `Right Arrow` → Move right one character.
- `Ctrl + Right Arrow` → Move right one word boundary.

---

**Q86. Abstraction**

Question: Abstraction means:
- [ ] (A) Summarization
- [ ] (B) Elimination
- [x] (C) Hiding
- [ ]  (D) Casting

Correct answer: (C) Hiding

Explanation: In object-oriented programming, abstraction means exposing essential features while hiding unnecessary implementation details.

Example: When you use an ATM, you select an operation and enter a PIN without needing to understand the internal banking software.

Important distinction:
- Abstraction: Hides implementation details and exposes essential functionality.
- Encapsulation: Bundles data and methods together and controls access to them.

---

**Q87. `Ctrl + Page Up`**

Question: `Ctrl + Page Up` is used to:
- [x] (A) Move the cursor one page up
- [ ] (B) Move the cursor one paragraph up
- [ ] (C) Move the cursor one screen up
- [ ] (D) Move the cursor one line up

Answer indicated in the paper: (A) Move the cursor one page up

Explanation: In older versions of Word, `Ctrl + Page Up` navigates to the previous page or browsing location, depending on the context.

---

**Q88. Polymorphism**

Question: Polymorphism is a feature of:
- [ ] (A) Procedural programming
- [ ] (B) SQL
- [ ] (C) Non-procedural programming
- [x] (D) Object-oriented programming

Correct answer: (D) Object-oriented programming

Explanation: Polymorphism means “many forms.” It allows the same interface or method name to behave differently depending on the object or arguments involved.

For example, in Java, a method named `draw()` might draw a circle for a Circle object and a rectangle for a Rectangle object.

Common forms include:
- Compile-time polymorphism: Method overloading.
- Runtime polymorphism: Method overriding through dynamic dispatch.

---

**Q89. `Ctrl + Home`**

Question: `Ctrl + Home` is used to:
- [x] (A) Move the cursor to the beginning of the document
- [ ] (B) Move the cursor to the beginning of the line
- [ ] (C) Move the cursor to the beginning of the paragraph
- [ ] (D) All of these
Correct answer: (A) Move the cursor to the beginning of the document

Explanation: In Microsoft Word, `Ctrl + Home` takes the insertion point to the beginning of the document.

**Quick revision**

| Shortcut	          | Function                          |
|---------------------|-----------------------------------|
| `Home`	            | Beginning of the line             |
| `End`	              |	End of the line                   |
| `Ctrl + Home`	      | Beginning of the document         |
| `Ctrl + End`        | End of the document               |
| `Ctrl + Left Arrow` | Previous word boundary            |
| `Ctrl + Down Arrow`	| Next paragraph                    |
| `Ctrl + Page Up`	  | Previous page/navigation location |
| `Ctrl + Page Down`	| Next page/navigation location     |

---

| MS Word and Microsoft Excel |
|-----------------------------|

---

**Q90. `Ctrl + End`**

Question: `Ctrl + End` is used to:
- [ ] (A) Move the cursor to the end of the line
- [x] (B) Move the cursor to the end of the document
- [ ] (C) Move the cursor to the end of the paragraph
- [ ] (D) None of these

Correct answer: (B) Move the cursor to the end of the document

Explanation: `Ctrl + End` moves the insertion point to the end of a document in Microsoft Word.

Remember: `Ctrl + Home` moves to the beginning; `Ctrl + End` moves to the end.

---

**Q91. Excel Auto Calculation**

Question: How can you update the values of formula cells if Auto Calculate mode in Excel is disabled?
- [ ] (A) F8
- [x] (B) F9
- [ ] (C) F10
- [ ] (D) F11

Correct answer: (B) F9

Explanation: In Excel, pressing `F9` recalculates formulas in open workbooks. This is useful when calculation mode is set to manual.

Exam tip: `F9` is the key to remember for recalculation.

---

**Q92. Excel Custom Lists**

Question: You want Excel to produce Jaistha, Aashadh, and so on when you type Baishakh and drag the fill handle. What should you set?
- [x] (A) Custom List
- [ ] (B) Auto Fill Options
- [ ] (C) Fill Across Worksheet
- [ ] (D) Fill Series

Correct answer: (A) Custom List

Explanation: Excel's Custom Lists feature lets you define a sequence of items that AutoFill can recognise.

For example, after creating the sequence Baishakh, Jaistha, Aashadh, entering Baishakh and dragging the fill handle can continue that sequence.

---

**Q93. Changing Excel Calculation Mode**

Question: Where can you change automatic or manual calculation mode in Excel?
- [ ] (A) Double-click the CAL indicator on the status bar
- [ ] (B) Go to Tools → Options → Calculation and select the corresponding option
- [x] (C) Both (A) and (B)
- [ ] (D) None of these

Answer indicated in the paper: (C) Both (A) and (B)

Explanation: The question refers to older Excel versions and their interface. In current Excel, calculation settings are generally found under Formulas → Calculation Options, where you can select Automatic or Manual.

---

**Q94. Excel Gridlines**

Question: How can you show or hide gridlines in an Excel worksheet?
- [ ] (A) Tools → Options → View tab → select or clear Gridlines
- [ ] (B) Click the Gridline tool on the Forms toolbar
- [x] (C) Both (A) and (B)
- [ ] (D) None of these

Answer indicated in the paper: (C) Both (A) and (B)

Explanation: The question uses an older Excel interface. In modern Excel, you can generally show or hide worksheet gridlines from the View tab by toggling the Gridlines option.


---

**Q95. Excel Screen Components**

Question: Which of the following Excel screen components cannot be turned on or off?
- [ ] (A) Formula Bar
- [ ] (B) Status Bar
- [x] (C) Tool Bar
- [ ] (D) None of these

Answer indicated in the paper: (C) Tool Bar

Explanation: The question is based on older Excel versions, where toolbars could be shown or hidden through menus. The exact interface and behaviour depend on the Excel version.

---

**Q96. `Ctrl + X` in Excel**

Question: What happens when you press Ctrl + X after selecting some cells in Excel?
- [ ] (A) The cell contents disappear from the cells and are stored in the Clipboard
- [x] (B) The cells selected are marked for cutting
- [ ] (C) The selected cells are deleted and cells are shifted left
- [ ] (D) The selected cells are deleted and cells are shifted up

Correct answer: (B) The selected cells are marked for cutting

Explanation: `Ctrl + X` cuts the selected cells. Excel marks the range for cutting so it can be pasted elsewhere. The data is moved when you complete the paste operation.

---

**Q97. Excel Paste Special**

Question: Which of the following options is not available in the Paste Special dialog box?
- [ ] (A) Add
- [ ] (B) Subtract
- [ ] (C) Divide
- [x] (D) SORT

Correct answer: (D) SORT

Explanation: Excel's Paste Special includes arithmetic operations such as `Add`, `Subtract`, `Multiply`, and `Divide`. <br/>
`Sort` is a separate feature, not a Paste Special arithmetic operation.

---

**Q98. Converting a Column into a Row**

Question: Which command would you choose to convert a column of data into a row?
- [ ] (A) Cut and Paste
- [ ] (B) Edit → Paste Special → Transpose
- [x] (C) Both (A) and (B)
- [ ] (D) None of these

Correct answer indicated in the paper: (C) Both (A) and (B)

Explanation: The reliable Excel feature for changing columns into rows is Transpose.

Example:
| Original column	| After transpose |
|-----------------|-----------------|
| Apple	          | Apple           |
| Banana	        | Banana          |
| Mango	          | Mango           |

The items originally arranged vertically become arranged horizontally. Simply cutting and pasting does not automatically transpose a range in the usual workflow, so Paste Special → Transpose is the key concept to remember.

---

**Q99. Text Overflow in Excel**

Question: It is acceptable to let long text flow into adjacent cells on a worksheet when:
- [ ] (A) Data will be entered in the adjacent cells
- [x] (B) No data will be entered in the adjacent cells
- [ ] (C) There is no suitable abbreviation for the text
- [ ] (D) There is no time to format the text

Correct answer: (B) No data will be entered in the adjacent cells

Explanation: Excel can display text overflowing into neighbouring empty cells. If the adjacent cell contains data, the overflow is blocked.

Example: If `A1` contains Computer Science and `B1` is empty, the text may extend visually into `B1`.

---

**Q100. Excel Cell Pointer — Selection**

Question: Which cell pointer indicates that you can make a selection?
- [ ] (A) Doctor's symbol (big plus)
- [ ] (B) Small thin plus icon
- [x] (C) Mouse pointer with anchor at the tip
- [ ] (D) None of these

Answer indicated in the paper: (C) Mouse pointer with anchor at the tip

Explanation: In the older Excel interface described by this question, the pointer's shape indicates the action available. The pointer with an arrow-like tip is used for selecting cells or ranges.

---

**Q101. Excel Cell Pointer — Fill Series**

Question: Which cell pointer indicates that you can fill a series?
- [x] (A) Doctor's symbol (big plus)
- [ ] (B) Small thin plus icon
- [ ] (C) Mouse pointer with anchor at the tip
- [ ] (D) None of these

Answer indicated in the paper: (A) Doctor's symbol (big plus)

Explanation: In Excel, the small black plus-shaped pointer at the fill handle is used to copy data or extend a series.

For example, enter `1` in `A1` and `2` in `A2`, select both cells, and drag the fill handle downward to continue `3, 4, 5....`

---

**Q102. Active Cell**

Question: On an Excel sheet, the active cell is indicated by:
- [ ] (A) A dotted border
- [x] (B) A dark wide border
- [ ] (C) A blinking border
- [ ] (D) Italic text

Correct answer: (B) A dark wide border

Explanation: The active cell is the currently selected cell, normally identified by a prominent border. Data you type is entered into this cell.

---

**Q103. Comments in Excel**

Question: What term describes explanatory text attached to a cell?
- [ ] (A) Context
- [ ] (B) Callout
- [x] (C) Comment
- [ ] (D) Dialog

Correct answer: (C) Comment

Explanation: A comment or note provides additional information associated with a cell without changing the cell's actual value.

---

**Q104. Selecting All Cells**

Question: Which of the following will not select all the cells in a document?
- [ ] (A) Using the Edit → Select All menu
- [ ] (B) Pressing Ctrl + A on the keyboard
- [x] (C) Clicking three times with the right mouse button in the spreadsheet
- [ ] (D) None of these

Correct answer: (C) Clicking three times with the right mouse button in the spreadsheet

Explanation: `Ctrl + A` is a standard shortcut for selecting data or the worksheet, depending on the current selection and context. Triple-clicking the right mouse button is not the standard Select All command.

---

**Q105. Default Style in Excel**

Question: The default style for new data keyed into a new workbook is:
- [ ] (A) Comma
- [x] (B) Normal
- [ ] (C) Currency
- [ ] (D) Per cent

Correct answer: (B) Normal

Explanation: The Normal style is the standard default cell style in the Excel versions this question refers to. Currency, Percentage, and Comma are specialised number formats or styles.

---

**Q106. Confirming Cell Entry**

Question: If you press ______, the cell accepts your typing as its contents.
- [ ] (A) `Tab`
- [ ] (B) `Ctrl + Enter`
- [ ] (C) `Enter`
- [ ] (D) `Alt + Enter`

Correct answer: (C) `Enter`

Explanation: Pressing `Enter` normally confirms the value or formula entered into the active cell and moves the selection down one row.

Other useful shortcuts:
- `Tab` — confirms the entry and moves right.
- `Alt + Enter` — inserts a new line within a cell while editing.
- `Ctrl + Enter` — enters the same content into all selected cells.

---

**Q107. Microsoft Excel**

Question: Which among the following is associated with Excel?
- [ ] (A) Graphic program
- [ ] (B) Word Processor
- [ ] (C) Presentation
- [x] (D) Spreadsheet

Correct answer: (D) Spreadsheet

Explanation: Microsoft Excel is spreadsheet software used for calculations, tables, charts, data analysis, and formulas.

---

**Q108. Logical Functions**

Question: Except which of the following functions, a formula with a logical function shows the words TRUE or FALSE as a result?
- [ ] (A) NOT
- [ ] (B) OR
- [x] (C) IF
- [ ] (D) AND

Correct answer: (C) IF

Explanation:
- `AND()` returns TRUE when all conditions are true.
- `OR()` returns TRUE when at least one condition is true.
- `NOT()` reverses a logical value.
- `IF()` returns one value when a condition is true and another when it is false.

Example:
```
=IF(A1>=40,"Pass","Fail")
```
This formula returns Pass or Fail, rather than necessarily returning TRUE or FALSE.

---

**Q109. Excel Zoom Percentage**

Question: Which of the following is not a valid zoom percentage in Excel?
- [ ] (A) 10
- [ ] (B) 100
- [ ] (C) 300
- [x] (D) 500

Correct answer: (D) 500

Explanation: In the Excel versions relevant to this question, the normal zoom range is 10% to 400%. Therefore, 500% is outside the supported range.

---

| Excel, SQL, OOP, Boolean Algebra and PowerPoint |
|-------------------------------------------------|

---

**Q110. Excel Conditional Formatting**

Question: You can check the conditions against ______ when applying conditional formatting.
- [ ] (A) Cell Value
- [ ] (B) Formula
- [x] (C) Both (A) and (B)
- [ ] (D) None of these

Correct answer: (C) Both (A) and (B)

Explanation: Conditional formatting changes a cell's appearance when a specified condition is satisfied. The condition can be based on a cell value or a formula.

Example: Highlight marks below 40 in red.

---

**Q111. Primary Key**

Question: Which of the following is a primary key in a student table?
- [ ] (A) UID number
- [x] (B) Admission number
- [ ] (C) Account number
- [ ] (D) PAN

Correct answer: (B) Admission number

Explanation: A primary key uniquely identifies each record in a table. A student's admission number is a suitable identifier when it is unique and non-null.

Remember: A primary key must be unique and cannot contain `NULL`.

---

**Q112. SQL Command**

Question: Which of the following is a valid SQL command?
- [ ] (A) cin
- [ ] (B) cout
- [ ] (C) tuple
- [x] (D) SELECT

Correct answer: (D) SELECT

Explanation: `SELECT` retrieves data from database tables.

Example:
```sql
SELECT name FROM Student;
```
`cin` and `cout` are commonly used for input and output in C++, not SQL commands.

---

**Q113. PowerPoint Slide Transition**

Question: Which PowerPoint option works best for adding a slide transition?
- [ ] (A) Animations
- [ ] (B) Chart Wizard
- [x] (C) Transition Wizard
- [ ] (D) Auto Content Wizard

Answer indicated in the paper: (C) Transition Wizard

Explanation: This question refers to an older PowerPoint interface. Slide transitions control how one slide changes to the next. In modern PowerPoint, use the Transitions tab.

---

**Q114. Objects in OOP**

Question: Objects are:
- [ ] (A) Design of function
- [ ] (B) Creator of data
- [x] (C) Instances of classes
- [ ] (D) Program block

Correct answer: (C) Instances of classes

Explanation: A class defines a structure or blueprint, while an object is an instance created from that class.

Example in C++:
```cpp
class Student {
public:
    int age;
};

Student s1;  // s1 is an object
```
---

**Q115. Editing an Embedded Organization Chart**

Question: You can edit an embedded organization chart object by:
- [ ] (A) Double-clicking the organization chart object
- [ ] (B) Clicking Edit Object
- [x] (C) Right-clicking the chart object, then clicking Edit MS-Organization Chart Object
- [ ] (D) Both (A) and (C)

Answer indicated in the paper: (C)

Explanation: In the older Microsoft Office environment, an embedded organization chart could be edited through its context menu. Double-clicking an embedded object could also open its editing interface, depending on the version and object type.

---

**Q116. Boolean Algebra**

Question: In Boolean algebra, `A.A` is equal to:
- [ ] (A) `A`
- [ ] (B) `2A`
- [ ] (C) `A^2`
- [ ] (D) `1`

Correct answer: (A) `A`

Explanation: This is the idempotent law of Boolean algebra: `A.A = A`

Boolean variables have values 0 or 1. Multiplying a Boolean variable by itself does not change its value.

---

**Q117. PowerPoint Slide Sorter**

Question: Slide Sorter can be accessed from which menu?
- [x] (A) View
- [ ] (B) Edit
- [ ] (C) File
- [ ] (D) Insert

Correct answer: (A) View

Explanation: Slide Sorter displays presentation slides as thumbnails, making it easier to reorder, copy, or delete slides. In older PowerPoint versions, it was available from the View menu.

---

**Q118. Boolean AND Operator**

Question: In Boolean algebra, the function of the AND operator is represented by:
- [ ] (A) `+`
- [ ] (B) `-`
- [ ] (C) `/`
- [x] (D) `.`

Correct answer: (D) `.`

Explanation: The standard Boolean algebra notation is:
- `OR`: `A+B`
- `AND`: `A.B`
- `NOT`: `inverse A or -A`

The `AND` operation returns 1 only when both inputs are 1.
| A	| B	| A.B |
| 0	| 0	| 0   |
| 0	| 1	| 0   |
| 1	| 0	| 0   |
| 1	| 1	| 1   |
  
---

**Q119. Pre-formatted PowerPoint Style**

Question: What would you choose to create a pre-formatted style?
- [ ] (A) Format
- [x] (B) Slide Layout
- [ ] (C) Slide Sorter View
- [ ] (D) None of these

Answer indicated in the paper: (B) Slide Layout

Explanation: A slide layout provides a predefined arrangement of placeholders for titles, text, images, and other content. In modern PowerPoint, themes and slide layouts help maintain consistent presentation formatting.

---

**Q120. Boolean OR Operator**

Question: Which logical operation is represented by the `+` sign in Boolean algebra?
- [ ] (A) OR
- [x] (B) NOT
- [ ] (C) NOR
- [ ] (D) AND

Correct answer: (A) OR

Explanation: In Boolean algebra, the plus sign represents `OR`: `A+B`

The output is 1 if at least one input is 1.
| A	| B	| A+B |
| 0	| 0	| 0   |
| 0	| 1	| 1   |
| 1	| 0	| 1   |
| 1	| 1	| 1   |

Important: Do not confuse Boolean algebra with ordinary arithmetic.

---

**Q121. PowerPoint Motion Path**

Question: To preview a motion-path effect using the Custom Animation task pane, we should:
- [ ] (A) Double-click the motion path
- [ ] (B) Click the Show Effect button
- [x] (C) Click the Play button
- [ ] (D) None of these

Answer indicated in the paper: (C) Click the Play button

Explanation: In the older Custom Animation task pane, the Play button previews the animation effects on the slide.

---

**Quick revision**

| Topic	                  | Key fact                           |
|-------------------------|------------------------------------|
| Conditional formatting	| Can use cell values or formulas    |
| Primary key	            | Unique, non-null identifier        |
| SQL	                    | `SELECT` retrieves data            |
| OOP	                    | Object = instance of a class       |
| Boolean idempotent law	| `A.A = A`                          |
| Boolean OR	            | `A+B`                              | 
| Boolean AND	            | `A.B`                              |
| Slide Sorter	          | View menu in older PowerPoint      |
| Motion-path preview	    | Play button in the older task pane |

---


| SQL, PowerPoint, C++ and Computer Networks |
|--------------------------------------------|

---

**Q122. SQL — DCL Command**

Question: Which one is a DCL command in SQL?
- [ ] (A) UPDATE
- [ ] (B) SELECT
- [ ] (C) DELETE
- [x] (D) GRANT

Correct answer: (D) GRANT

Explanation: DCL stands for Data Control Language. It controls access permissions in a database.

| SQL category	                  | Examples                                  |
|---------------------------------|-------------------------------------------|
| DDL — Data Definition Language	| `CREATE`, `ALTER`, `DROP`                 |
| DML — Data Manipulation Language|	`INSERT`, `UPDATE`, `DELETE`              |
| DQL — Data Query Language	      | `SELECT` (commonly classified separately) |
| DCL — Data Control Language	    | `GRANT`, `REVOKE`                         |

---

**Q123. PowerPoint — Dragging**

Question: What is the term used when you press and hold the left mouse key and move the mouse around the slide?
- [ ] (A) Moving
- [x] (B) Dragging
- [ ] (C) Monitoring
- [ ] (D) Highlighting

Correct answer: (B) Dragging

Explanation: Dragging means holding down a mouse button while moving the pointer. It is commonly used to move objects, resize shapes, or reposition images on a slide.

---

**Q124. SQL — Viewing Data**

Question: Which of the following SQL commands is used to view data?
- [ ] (A) CREATE
- [ ] (B) INSERT
- [x] (C) SELECT
- [ ] (D) UPDATE

Correct answer: (C) SELECT

Explanation: SELECT retrieves records from a table.
```sql
SELECT * FROM Student;
```
This query displays all columns from the Student table.

---

**Q125. PowerPoint — Applying Transitions**

Question: Which view is best when setting transition effects for all slides in a presentation?
- [ ] (A) Slide
- [ ] (B) Notes Page View
- [ ] (C) Outline View
- [x] (D) Slide Sorter View

Correct answer: (D) Slide Sorter View

Explanation: Slide Sorter displays multiple slides as thumbnails, making it convenient to select and manage several slides. This question refers to an older PowerPoint interface.

---

**Q126. C++ — math.h**

Question: `Math.h` is a:
- [ ] (A) Derived data type
- [ ] (B) Function
- [x] (C) Header file
- [ ] (D) Built-in data type

Correct answer: (C) Header file

Explanation: In C and older C++ code, `math.h` declares mathematical functions such as `sqrt()` and `pow()`.

In modern C++, the preferred header is: `#include <cmath>`


Example:
```c
#include <cmath>
#include <iostream>
using namespace std;

int main() {
    cout << sqrt(25);
}
// -----------------------
// Output: 5
```
---

**Q127. PowerPoint — Design Templates**

Question: The selected design template can be applied:
- [ ] (A) To the current slide only
- [x] (B) To all the slides
- [ ] (C) To all the new presentations you create
- [ ] (D) All of these

Answer indicated in the paper: (B) To all the slides

Explanation: In older PowerPoint versions, a selected design template could be applied to the whole presentation. The interface also allowed different choices depending on the version and workflow.

---

**Q128. Slide Design vs Auto Content Wizard**

Question: The difference between Slide Design and Auto Content Wizard is:
- [ ] (A) Both are the same
- [ ] (B) Auto Content Wizard is just the wizard version of Slide Design
- [x] (C) Slide Design does not provide sample content, but Auto Content Wizard provides sample content too
- [ ] (D) Slide Design asks your choice in steps, but Auto Content Wizard does not let you make choices

Answer indicated in the paper: (C)

Explanation: In the older PowerPoint versions referenced by this question, Slide Design primarily controlled a presentation’s visual appearance, while Auto Content Wizard helped create a presentation structure and could provide suggested content.

---

**Q129. PowerPoint — Slide Design and Layout**

Question: In which menu can you find features like Slide Design and Slide Layout?
- [ ] (A) Insert Menu
- [x] (B) Format Menu
- [ ] (C) Tools Menu
- [ ] (D) Slide Show Menu

Answer indicated in the paper: (B) Format Menu

Explanation: This is based on an older PowerPoint menu layout. In current PowerPoint, design themes and layouts are generally accessed through the Design and Home tabs.

---

**Q130. PowerPoint — Animation Options**

Question: Which menu provides options such as Animation Scheme, Custom Animation, and Slide Transition?
- [ ] (A) Insert Menu
- [ ] (B) Format Menu
- [ ] (C) Tools Menu
- [x] (D) Slide Show Menu

Answer indicated in the paper: (D) Slide Show Menu

Explanation: These options belonged to older PowerPoint versions. Modern PowerPoint generally uses the Animations tab for object animation and the Transitions tab for slide transitions.

---

**Q131. Distributed System**

Question: When a collection of various computers appears to its client as a single coherent system, it is called:
- [ ] (A) Computer network
- [x] (B) Distributed system
- [ ] (C) Both (A) and (B)
- [ ] (D) None of the mentioned

Correct answer: (B) Distributed system

Explanation: A distributed system consists of multiple computers that cooperate and may present a unified service to users.

A computer network provides communication between devices; a distributed system uses multiple connected computers to work together toward a shared purpose.

---

**Q132. Processes on Networked Devices**

Question: Two devices are in a network if:
- [x] (A) A process in one device is able to exchange information with a process in another device
- [ ] (B) A process is running on both devices
- [ ] (C) PIDs of processes running on different devices are the same
- [ ] (D) None of these

Correct answer: (A)

Explanation: Network communication allows processes running on different devices to exchange information. The processes do not need to have the same process ID (PID); PIDs are local identifiers managed by operating systems.

---

Q133. Which computer network is built on top of another network?
- [ ] (A) Prior network
- [ ] (B) Chief network
- [ ] (C) Prime network
- [x] (D) Overlay network

Correct answer: (D) Overlay network

An overlay network is a virtual network built on top of an existing network. Its logical connections are created using the underlying network infrastructure.

---

Q134. In a computer network, nodes are:
- [ ] (A) The computer that originates the data
- [ ] (B) The computer that routes the data
- [ ] (C) The computer that terminates the data
- [x] (D) All of these

Correct answer: (D) All of these

A network node can be a source, destination, or forwarding device. Nodes are not limited to computers; routers, switches, and other network-connected devices can also be nodes.

---

Q135. The communication channel is shared by all machines on the network in a:
- [x] (A) Broadcast network
- [ ] (B) Unicast network
- [ ] (C) Multicast network
- [ ] (D) None of these

Correct answer: (A) Broadcast network

In a broadcast network, a shared communication medium allows transmitted data to be available to all connected machines. The intended recipient processes it.

---

Q136. Which device forwards packets between networks by processing the routing information included in packets?
- [ ] (A) Bridge
- [ ] (B) Firewall
- [x] (C) Router
- [ ] (D) All of these

Correct answer: (C) Router

A router examines network-layer information, such as the destination IP address, and forwards packets toward the appropriate network.

---

Q137. The structure or format of data is called:
- [x] (A) Syntax
- [ ] (B) Semantics
- [ ] (C) Struct
- [ ] (D) None of these

Correct answer: (A) Syntax

- `Syntax`: Rules governing structure and format.
- `Semantics`: Meaning of the data or statement.

---

Q138. Communication between a computer and a keyboard involves ______ transmission.
- [ ] (A) Automatic
- [ ] (B) Half-duplex
- [ ] (C) Full-duplex
- [x] (D) Simplex

Expected answer: (D) Simplex — with a caveat

A keyboard primarily sends input to the computer, which resembles one-way communication. <br/>
However, this question is technically simplified: actual keyboard interfaces may support bidirectional communication for commands and responses. <br/> 
The scan appears to have a mark beside (B) Half-duplex, so the paper’s marking and the conceptual answer may differ.

---

Q139. Which of the following is not a network edge device?
- [ ] (A) PC
- [ ] (B) Smartphones
- [ ] (C) Servers
- [x] (D) Switch

Likely answer: (D) Switch

PCs, smartphones, and servers are end devices. A switch generally connects devices within a network rather than acting as an end device. The exact term “edge device” can vary by context.

---

Q140. Which transmission medium has the highest transmission speed in a network?
- [ ] (A) Coaxial cable
- [ ] (B) Twisted pair cable
- [x] (C) Optical fibre
- [ ] (D) Electrical cable

Correct answer: (C) Optical fibre

Optical fibre carries data as light and supports very high bandwidth over long distances, making it the best answer among these options.

---

Q141. What is the Internet?
- [ ] (A) A single network
- [x] (B) A vast collection of different networks
- [ ] (C) Interconnection of local area networks
- [ ] (D) None of these

Correct answer: (B) A vast collection of different networks

The Internet is a global network of interconnected networks. It connects private, public, academic, business, and government networks using common communication protocols.

---

Q142. To join the Internet, a computer has to be connected to a:
- [ ] (A) Internet Architecture Board
- [ ] (B) Internet Society
- [x] (C) Internet Service Provider
- [ ] (D) None of these
      
Correct answer: (C) Internet Service Provider (ISP)

An ISP provides Internet access to users, homes, and organizations.

---

Q143. Internet access by transmitting digital data over the wires of a local telephone network is provided by:
- [ ] (A) Leased line
- [x] (B) Digital subscriber line
- [ ] (C) Digital signal line
- [ ] (D) None of the mentioned

Correct answer: (B) Digital Subscriber Line (DSL)

DSL provides digital Internet access over traditional telephone copper lines.

---

Q144. ISPs exchange Internet traffic between their networks by:
- [x] (A) Internet exchange point
- [ ] (B) Subscriber end point
- [ ] (C) ISP end point
- [ ] (D) None of these

Correct answer: (A) Internet exchange point

An Internet Exchange Point (IXP) is a physical infrastructure where different networks connect to exchange Internet traffic.

---

Q145. Which of the following protocols is not used on the Internet?
- [ ] (A) HTTP
- [ ] (B) DHCP
- [ ] (C) DNS
- [x] (D) None of these

Correct answer: (D) None of these

All three are used on the Internet:
- HTTP: Transfers web resources.
- DHCP: Automatically assigns network configuration, such as IP addresses.
- DNS: Translates domain names into IP addresses.

---

Q146. An IPv6 address has a size of:
- [ ] (A) 32 bits
- [ ] (B) 64 bits
- [x] (C) 128 bits
- [ ] (D) 265 bits
  
Correct answer: (C) 128 bits

IPv4 addresses are 32 bits long, whereas IPv6 addresses are 128 bits long.

---

Q147. The Internet works on:
- [x] (A) Packet switching
- [ ] (B) Circuit switching
- [ ] (C) Both packet switching and circuit switching
- [ ] (D) None of these

Correct answer: (A) Packet switching

The Internet primarily uses packet switching: data is divided into packets that are routed independently through networks. Circuit switching is associated with traditional telephone systems.

---

Q148. Which of the following is not an application-layer protocol used on the Internet?
- [ ] (A) Remote Procedure Call
- [ ] (B) Internet Relay Chat
- [x] (C) Resource Reservation Protocol
- [ ] (D) None of these

Correct answer: (C) Resource Reservation Protocol (RSVP)

RSVP is used for resource reservation and traffic-flow signalling, rather than being a typical application-layer protocol. Remote Procedure Call (RPC) and Internet Relay Chat (IRC) are associated with application-level services.

---

Q149. Which protocol assigns an IP address to a client connected to the Internet?
- [x] (A) DHCP
- [ ] (B) IP
- [ ] (C) RPC
- [ ] (D) None of these

Correct answer: (A) DHCP

Explanation: DHCP stands for Dynamic Host Configuration Protocol. It automatically provides a client with an IP address and other network configuration settings.

---

Q150. Which one of the following is not used in Media Access Control (MAC)?
- [ ] (A) Ethernet
- [x] (B) Digital Subscriber Line
- [ ] (C) Fiber Distributed Data Interface
- [ ] (D) None of these

Correct answer: (B) Digital Subscriber Line (DSL)

Explanation: Ethernet and FDDI are networking technologies associated with data-link and media-access mechanisms. DSL is a broadband access technology over telephone lines, not a MAC protocol or LAN media-access technology.

---
</details>
<!----------------------------->

<details>
  <summary> <b> PYQs 2018 </b> </summary>


---
</details>
<!----------------------------->
