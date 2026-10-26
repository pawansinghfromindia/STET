### PYQs

<details>
  <summary> <b> 2025 - 7th Nov Shift 1  </b> </summary>

<br/>

Q.1 If a robot is able to change its own trajectory as per the external conditions, then the
robot is considered as the_
- [x] A. Intelligent
- [ ] B.Open loop
- [ ] C.Mobile
- [ ] D.Non-servo

<details>
  <summary> Solution </summary>

Correct!  A. Intelligent

An intelligent robot can sense external conditions, process information, and adjust its trajectory or actions according to changes in its environment.

An intelligent robot can sense changes in its environment and adjust its actions accordingly.

For example, if a robot detects an obstacle in its path, it can change its trajectory to avoid the obstacle.

Quick revision:
- **Intelligent robot**: Adapts its actions to changing conditions.
- **Open-loop robot**: Operates without feedback to correct its actions.
- **Mobile robot**: Can move from one place to another.
- **Non-servo robot**: Typically operates without servo-based feedback control.

Which type of control system uses feedback to adjust its output?
- [ ] A. Open-loop system
- [x] B. Closed-loop system
- [ ] C. Manual system
- [ ] D. Non-servo system
    
- **Open-loop system**: Does not use feedback to adjust its output.
- **Closed-loop system**: Uses feedback to compare the actual output with the desired output and make corrections.
- **Manual system**: Depends on human operation; this does not specifically mean feedback-based automatic control.
- **Non-servo system**: Does not specifically identify a feedback-based control system.

</details>

---

Q.2 Convert the Boolean function `F(A, B, C) = Π(0, 2, 4, 5, 7)` to its simplified POS form
- [ ] A. `A + B + C`
- [ ] B. `A + B' + C`
- [ ] C. `A'B'C'`
- [ ] D. `(A + B)(A + C')(B + C)`
- [x] E. `(A+B+C)(A+B'+C)(A'+B+C)(A'+B+C')(A'+B'+C')`

<details>
  <summary> Solution </summary>

**Step 1: Understand the notation: `F(A,B,C) = Π(0,2,4,5,7)`**

The symbol `Π` represents the product of maxterms. <br/>
These indices are the input combinations for which `F=0`.

| Index	| A	| B	| C |
|-------|---|---|---|
| 0	    | 0	| 0	| 0 |
| 2	    | 0	| 1	| 0 |
| 4	    | 1	| 0	| 0 |
| 5	    | 1	| 0	| 1 |
| 7	    | 1	| 1	| 1 |

**Step 2: Form the maxterms**

For a maxterm, use:
- Variable value 0 -> normal variable, e.g. `A`
- Variable value 1 -> complemented variable, e.g. `A'`

Therefore, **`F = (A+B+C)(A+B'+C)(A'+B+C)(A'+B+C')(A'+B'+C')`**

For a Boolean function `F(A,B,C) = Π(1,3)`, what does the notation tell us?
- [ ] A. `F=1` at indices 1 and 3
- [x] B. `F=0` at indices 1 and 3
- [ ] C. `F=0` at every index
- [ ] D. `F=1` at every index except 1 and 3


Remember:
-  (sum of minterms) lists the indices where `F=1`.
-  (product of maxterms) lists the indices where `F=0`.
For `F(A,B,C) = Π(1,3)`, the output is zero at indices 1 and 3.

Quick revision
- `Σ` -> output 1
- `Π` -> output 0

</details>

---

Q.3 Which keyword is used to define an abstract method within an abstract class?
- [x] A. abstract
- [ ] B. virtual
- [ ] C. override
- [ ] D. implement

<details>
  <summary> Solution </summary>

The `abstract` keyword is used in languages such as Java and C# to declare an abstract method within an abstract class.

An abstract method is declared without a method body and is intended to be implemented by a concrete subclass.

Example in Java:
```java
abstract class Animal {
    abstract void sound();
}

class Dog extends Animal {
    @Override
    void sound() {
        System.out.println("Bark");
    }
}
```
Here:
- `abstract` declares the method without a body.
- `@Override` indicates that the subclass method overrides or implements an inherited method.
- `virtual` allows overriding in languages such as C#; it does not itself declare an abstract method.
- `implement` is not a Java or C# keyword for declaring an abstract method.

In Java, which keyword is used when a subclass provides an implementation of an inherited abstract method?
- [ ] A. `abstract`
- [ ] B. `extends`
- [ ] C. `implements`
- [x] D. `override`

Correct D. `override`

In Java, a subclass provides the implementation of an inherited abstract method by defining a method with the same signature. <br/>
The `@Override` annotation indicates that the method overrides an inherited method.

- `abstract` - declares a method without an implementation.
- `extends` - establishes class inheritance.
- `implements` - is used when a class implements an interface, not when overriding an abstract class's method.
- `override` - the intended option, but note that Java uses the `@Override` annotation, not an `override` keyword. C# does use override as a keyword.

| Concept	                    | Java         |
|-----------------------------|--------------|
| Declare an abstract method	| `abstract`   |
| Inherit a class	            | `extends`    |
| Implement an interface	    | `implements` |
| Mark a method as overriding	| `@Override`  |

</details>

---

Q.4 The Floyd-Warshall algorithm is a popular method for solving the All-Pair Shortest
Paths problem. What is the time complexity of the Floyd-Warshall algorithm for a graph
with "n" vertices?
- [ ] A. `O(n)`
- [ ] B. `O(n log n)`
- [ ] C. `O(n^2)`
- [x] D. `O(n^3)`

<details>
  <summary> Solution </summary>

Correct! D. `O(n^3)`

The Floyd–Warshall algorithm uses three nested loops to examine all possible intermediate vertices for every pair of vertices.

<img width="617" height="392" alt="image" src="https://github.com/user-attachments/assets/18928205-903f-4734-b238-091763938b90" />

- First loop: selects the intermediate vertex `k`.
- Second loop: selects the source vertex `i`.
- Third loop: selects the destination vertex `j`.
Each loop runs up to `n` times, so the total time complexity is `n x n x n` = `O(n^3)`.

> **Floyd–Warshall -> three nested loops -> `O(n^3)`.**

Remember:
- **Binary Search** -> `O(\log n)`
- **Linear Search** -> `O(n)`
- **Bubble Sort** (average/worst case) -> `O(n^2)`
- **Floyd-Warshall** -> `O(n^3)`

</details>

---

Q.5 Which of the following applications include in the Strategic Computing Program?
- [ ] A. Battle Management
- [ ] B. Autonomous systems
- [ ] C. Pilot’s associate
- [x] D. All of the above

<details>
  <summary> Solution </summary>

Correct! D. All of the above.

The **Strategic Computing Program** was a **US Defense Advanced Research Projects Agency (DARPA)** initiative launched in the 1980s to advance artificial intelligence for military applications.

Its major application areas included:
- **Battle Management**: Using AI to support military planning and decision-making.
- **Autonomous systems**: Developing systems capable of operating with reduced human intervention.
- **Pilot’s Associate**: An AI-based assistant intended to help military pilots manage information and cockpit tasks.

> Remember these three applications together: Battle Management + Autonomous Systems + Pilot's Associate 

Which organization launched the Strategic Computing Program?
- [ ] A. NASA
- [x] B. DARPA
- [ ] C. UNESCO
- [ ] D. WHO

Correct! B. DARPA (Defense Advanced Research Projects Agency).

DARPA launched the Strategic Computing Program in the 1980s to advance artificial intelligence and computing technologies for defense applications.

> **DARPA -> Strategic Computing Program**.

</details>

---

Q.6 Turing machine can be represented using:
- [ ] A. Transition table
- [ ] B. Transition diagram
- [ ] C. Instantaneous description
- [x] D. All of these

<details>
  <summary> Solution </summary>

Correct! D. All of these.

A **Turing machine** can be represented in several ways:
- A. **Transition table**: Shows the transitions in tabular form.
- B. **Transition diagram**: Represents states and transitions graphically.
- C. **Instantaneous description (ID)**: Represents the machine’s current configuration, including its state, tape contents, and head position.

Which component of a Turing machine stores the input and symbols being processed?
- [ ] A. Finite control
- [x] B. Tape
- [ ] C. Transition function
- [ ] D. State diagram

Correct! B. Tape.

- **Tape**: Stores the input and the symbols being processed by the Turing machine.
- **Finite control**: Keeps track of the machine's current state.
- **Transition function**: Determines the next state, the symbol to write, and the direction to move.
- **State diagram**: Visually represents the machine's transitions.

> Remember: **Tape = stores data; finite control = tracks state**.

</details>

---

Q.7 All of the following are considered biometrics, except:
- [ ] A. Fingerprint
- [x] B. Password
- [ ] C. Voice
- [ ] D. Retina

<details>
  <summary> Solution </summary>

Correct! B. Password.

- **Fingerprint**: A physical biometric characteristic.
- **Voice**: A behavioral/physical characteristic used for biometric recognition.
- **Retina**: A physical biometric characteristic based on the eye.
- **Password**: Something you know, not a biometric characteristic.

Which of the following is an example of behavioral biometrics?
- [ ] A. Fingerprint
- [ ] B. Retina scan
- [x] C. Typing rhythm
- [ ] D. Iris pattern

Correct! C. Typing rhythm.

**Behavioral biometrics** identify people through patterns in their actions or behavior.
- **Typing rhythm**: Behavioral biometric — analyzes typing speed and keystroke patterns.
- **Fingerprint**: Physiological biometric.
- **Retina scan**: Physiological biometric.
- **Iris pattern**: Physiological biometric.

Quick recap
> Physiological = body characteristics; <br/>
> Behavioral = patterns in how you act.

</details>

---

Q.8 To which of the following the term "DBA" referred?
- [ ] A. Data Bank Administrator
- [x] B. Database Administrator
- [ ] C. Data Administrator
- [ ] D. None of the above

<details>
  <summary> Solution </summary>

Correct! B. Database Administrator.

A **Database Administrator (DBA)** manages and maintains databases. <br/>
Typical responsibilities include:
- Managing database access and user permissions.
- Maintaining data security and backups.
- Monitoring database performance.
- Recovering data when failures occur.

Which SQL command is commonly used to grant privileges to a database user?
- [x] A. `GRANT`
- [ ] B. `UPDATE`
- [ ] C. `SELECT`
- [ ] D. `INSERT`

The SQL `GRANT` command gives database users specific privileges, such as permission to read or modify data.
- `GRANT` - gives privileges.
- `UPDATE` - modifies existing records.
- `SELECT` - retrieves data.
- `INSERT` - adds new records.

</details>

---

Q.9 The default baud rate of Modbus RTU is?
- [ ] A. 19600
- [x] B. 19200
- [ ] C. 38400
- [ ] D. 57600

<details>
  <summary> Solution </summary>

Correct! B. 19200 baud.

**Baud rate** refers to the signaling rate used for serial communication. <br/>
Modbus RTU commonly uses baud rates such as 9600 and 19200, depending on the configuration.

For this MCQ, remember 19200 as the expected answer.

What does baud rate measure in serial communication?
- [ ] A. Number of data packets per second
- [x] B. Number of signal symbols per second
- [ ] C. Number of bytes stored in memory
- [ ] D. Number of devices connected to a network

Correct! B. Number of signal symbols per second.

**Baud rate** measures the number of signal symbols transmitted per second in a communication channel. <br/>
One symbol can represent one or more bits, so baud rate is not always the same as bits per second.

Quick recap
- **Baud rate = symbols per second**.
- **Bit rate = bits per second**.

</details>

---

Q. 10 The goal of synchronization mechanisms in parallel programming is to:
- [ ] A. Speed up the execution of processes
- [ ] B. Eliminate parallelism
- [x] C. Avoid deadlock situations
- [ ] D. Increase the number of race conditions

<details>
  <summary> Solution </summary>

Correct! C. Avoid deadlock situations.

**Synchronization mechanisms** coordinate processes or threads that access shared resources. They help prevent race conditions and can help avoid deadlocks when designed carefully.

- A. Speed up execution: Synchronization can add overhead rather than directly speed up execution.
- B. Eliminate parallelism: Incorrect; parallel execution can continue.
- C. Avoid deadlock situations: The closest option, though synchronization does not automatically prevent every deadlock.
- D. Increase race conditions: Incorrect; synchronization helps prevent race conditions.

What is a race condition?
- [x] A. Two or more threads access shared data, and the result depends on execution order.
- [ ] B. A program always executes threads in a fixed order.
- [ ] C. A process finishes before it starts.
- [ ] D. A thread permanently releases all resources.

Correct! A.

A **race condition** occurs when two or more threads access shared data and the final result depends on the order or timing of their execution.

Example: Two threads try to increase the same counter simultaneously. Without proper synchronization, one update may be lost.

Quick recap
- **Race condition** -> result depends on execution timing.
- **Synchronization** -> coordinates access to shared resources.

</details>

Q.11 Which of the following IP addresses is valid
- [ ] A. `122.94.96.212`
- [ ] B. `212.254.258.210`
- [ ] C. `210.10.12.156.209`
- [ ] D. `122.294.56.68`

<details>
  <summary> Solution </summary>

Correct! A. `122.94.96.212`

A valid **IPv4 address** has four numbers (octets) separated by dots. <br/> 
Each octet must be between `0` and `255`. <br/>
IPv4 address has four octets.

- A. `122.94.96.212` - Valid; four octets, all within range.
- B. `212.254.258.210` - Invalid; 258 exceeds 255.
- C. `210.10.12.156.209` - Invalid; it has five octets instead of four.
- D. `122.294.56.68` - Invalid; 294 exceeds 255.

Which of these is a valid IPv4 address?
- [ ] A. 192.168.1.256
- [x] B. 10.0.0.25
- [ ] C. 172.16.300.1
- [ ] D. 192.168.1

Correct! B. `10.0.0.25`

All four octets are within the valid range of 0–255, and the address contains exactly four octets.

Quick recap
- IPv4 = 4 octets
- Each octet = 0–255

</details>

---

Q.12 ___________ plot is used to show the spread and centers of a dataset.
- [x] A. box
- [ ] B. line
- [ ] C. bar
- [ ] D. histogram

<details>
  <summary> Solution </summary>

Correct! A. Box plot.

A **box plot** shows the center and spread of a dataset using the five-number summary:
- Minimum
- First quartile (Q1)
- Median (Q2)
- Third quartile (Q3)
- Maximum

**Histogram** <br/>
A histogram shows the frequency distribution of data using bars, but a box plot is specifically used to summarize the center and spread.

Which value represents the middle of a dataset in a box plot?
- [ ] A. Mean
- [x] B. Median
- [ ] C. Range
- [ ] D. Mode

Correct! B. Median.

The median is the middle value of an ordered dataset. <br/>
In a box plot, it is represented by the line inside the box.

Quick recap
- **Median**: Middle value.
- **Range**: Maximum - minimum.
- **Mean**: Average of all values.
- **Mode**: Most frequently occurring value.

</details>

---

Q.13 How can you establish a connection between PHP and MySQL?
- [x] A. Using the "`connect()`" function in PHP
- [ ] B. By including a PHP library
- [ ] C. By embedding MySQL queries directly in PHP code
- [ ] D. By using the "`mysqli_connect()`" function in PHP

<details>
  <summary> Solution </summary>

Correct D. By using the `mysqli_connect()` function in PHP.

The `mysqli_connect()` function establishes a connection between PHP and a MySQL database.

```php
$conn = mysqli_connect("localhost", "username", "password", "database");
```
- `localhost` - MySQL server address.
- `username` - Database username.
- `password` - Database password.
- `database` - Name of the database to connect to.

`connect()` by itself is not the standard procedural function used to establish a MySQL connection in PHP. <br/.
MySQLi also supports the object-oriented approach using new `mysqli(...)`.

Which PHP function is used to execute an SQL query using the procedural MySQLi approach?
- [x] A. `mysqli_query()`
- [ ] B. `mysqli_connect()`
- [ ] C. `mysqli_fetch_assoc()`
- [ ] D. `mysqli_close()`

Correct! A. `mysqli_query()`

The `mysqli_query()` function executes an SQL query using the procedural MySQLi approach.

Quick comparison:
- `mysqli_query()` - Executes an SQL query.
- `mysqli_connect()` - Establishes a database connection.
- `mysqli_fetch_assoc()` -  Fetches a row as an associative array.
- `mysqli_close()` - Closes the database connection.

> **Connect -> Query -> Fetch results -> Close connection**

</details>

---

Q.14 Which one is not a physical threat
- [x] A. Hacking
- [ ] B. Storm
- [ ] C. Fire
- [ ] D. Flood

<details>
  <summary> Solution </summary>

Correct! A. Hacking.

- **Hacking**: A cybersecurity threat involving unauthorized access to computer systems; it is not a physical threat.
- **Storm**: Can physically damage equipment and buildings.
- **Fire**: Can destroy hardware and facilities.
- **Flood**: Can damage computers, servers, and infrastructure.

Which of the following is an example of a physical security measure?
- [ ] A. Antivirus software
- [ ] B. Firewall
- [x] C. Biometric door access
- [ ] D. Data encryption

Correct! C. Biometric door access.

Biometric door access is a physical security measure because it controls who can enter a building or restricted area using fingerprints, facial recognition, or other biometric features.

Quick recap
- **Physical security**: Protects buildings, equipment, and facilities.
- **Cybersecurity**: Protects computer systems, networks, and data.


</details>

---

Q.15 The SQL keyword……………….is used with wildcards.
- [x] A. `LIKE`
- [ ] B. `IN`
- [ ] C. `NOT IN`
- [ ] D. `DISTINCT`

<details>
  <summary> Solution </summary>

Correct! The answer is A. LIKE.

In SQL, `LIKE` is used with wildcards to match patterns in text.
- `%` - Matches zero or more characters.
- `_` - Matches exactly one character.

Example:
```sql
SELECT * FROM Students WHERE name LIKE 'A%';

-- This query finds students whose names start with A.
```

Which wildcard matches exactly one character in a SQL `LIKE` pattern?
- [ ] A. `%`
- [x] B. `_`
- [ ] C. `*`
- [ ] D. `#`

Correct! B. `_` (underscore).

Explanation: In SQL `LIKE` patterns:
- `%` matches zero or more characters.
- `_` matches exactly one character.

```sql
SELECT *
FROM Students
WHERE name LIKE 'A_';

-- This matches two-character names starting with A, such as An or Al.
```

Quick recap
> **`%` = any number of characters** <br/>
> **`_` = exactly one character**

</details>

---

Q.16 What is the key advantage of using a carry-lookahead adder instead of a ripple-carry
adder?
- [ ] A. Simplicity of design
- [x] B. Faster propagation delay
- [ ] C. Lower power consumption
- [ ] D. Reduced gate count

<details>
  <summary> Solution </summary>

Correct! B. Faster propagation delay.

A carry-lookahead adder calculates carry signals in advance using generate and propagate logic. 

This reduces the time needed to compute the final sum compared with a ripple-carry adder, where the carry moves through each stage sequentially.

| Feature	          | Ripple-carry adder | Carry-lookahead adder       |
|-------------------|--------------------|-----------------------------|
| Carry calculation	| Sequential	       | Parallel-style calculation  | 
| Propagation delay	| Higher	           | Lower                       |
| Circuit design	  |Simpler	           | More complex                |

In a ripple-carry adder, how does the carry signal move?
- [ ] A. It is calculated for all bits simultaneously.
- [x] B. It moves from one bit stage to the next.
- [ ] C. It skips all intermediate stages.
- [ ] D. It is generated only after the final sum.

Correct! The answer is B. It moves from one bit stage to the next.

In a ripple-carry adder, each bit stage passes its carry output to the next stage. The carry must propagate through the stages, which increases the total delay.

Quick recap
- **Ripple-carry adder**: Carry moves stage by stage.
- **Carry-lookahead adder**: Calculates carries faster using generate and propagate logic.

</details>

---

Q.17 What is the difference between a hard disk drive and a solid-state drive?
- [x] A. A hard disk drive uses spinning disks to store data, while a solid-state drive uses flash
memory to store data.
- [ ] B. A hard disk drive is slower than a solid-state drive.
- [ ] C. A hard disk drive is more durable than a solid-state drive.
- [ ] D. All of the above

<details>
  <summary> Solution </summary>

Correct! A. A hard disk drive uses spinning disks to store data, while a solid-state drive uses flash memory to store data.

- HDDs use spinning magnetic disks; SSDs use flash memory and have no moving mechanical parts.
- SSDs are usually faster than HDDs.
- SSDs are generally more resistant to physical shocks because they have no moving parts.

Which storage device has no moving mechanical parts?
- [ ] A. HDD
- [x] B. SSD
- [ ] C. DVD drive
- [ ] D. Magnetic tape drive

Correct! B. SSD (Solid-State Drive)

An SSD stores data using flash memory and has no moving mechanical parts. <br/>
An HDD uses spinning magnetic disks and moving read/write components.

Quick recap
- **HDD**: Spinning disks, mechanical parts.
- **SSD**: Flash memory, no moving parts.

</details>

---

Q.18 In an operating system, a "buffer cache" is used to:
- [ ] A. Store files in memory
- [x] B. Store copies of frequently used files in memory
- [ ] C. Store the operating system kernel
- [ ] D. Store input/output devices

<details>
  <summary> Solution </summary>

Correct!  B. Store copies of frequently used files in memory.

A **buffer cache** keeps copies of disk data blocks in memory so the operating system can reduce repeated disk access and improve performance.

Strictly speaking, a buffer cache typically caches disk blocks, not necessarily entire files.

What is the main benefit of using a buffer cache?
- [ ] A. Increase disk access time
- [x] B. Reduce repeated disk access
- [ ] C. Increase file size
- [ ] D. Replace the operating system kernel

Correct! The answer is B. Reduce repeated disk access.

The buffer cache stores disk data blocks in memory. When the same data is needed again, the operating system may retrieve it from memory instead of reading it from the disk, improving performance.

Quick recap
> **Buffer cache -> fewer disk accesses -> faster data retrieval**.

</details>

---

Q.19 _________ are the set of rules that governs how data can be transmitted over world wide web.
- [x] A. Hyper Text Transfer Protocol
- [ ] B. Encryption Standards
- [ ] C. Cyber forensic
- [ ] D. Digital Certificates

<details>
  <summary> Solution </summary>

Correct! The answer is A. Hyper Text Transfer Protocol (HTTP).

**HTTP** is a protocol that defines rules for communication and data transfer between web clients (such as browsers) and web servers.

- A. **HTTP**: Governs web communication.
- B. **Encryption Standards**: Help protect data but are not the web's.
- C. **Cyber forensic**: Concerns investigating digital evidence.
- D. **Digital Certificates**: Help verify identities and support secure communication.


Which secure version of HTTP is commonly used to protect data exchanged between a browser and a web server?
- [ ] A. FTP
- [ ] B. SMTP
- [x] C. HTTPS
- [ ] D. Telnet

Correct! C. HTTPS

HTTPS (Hypertext Transfer Protocol Secure) encrypts data exchanged between a browser and a web server, helping protect it from interception.

</details>

---

Q.20 Multimedia system require hard real time scheduling ___________
- [x] A. to ensure critical tasks will be serviced within timing deadlines
- [ ] B. to deliver the media file to the client
- [ ] C. to minimize the delay
- [ ] D. for security

<details>
  <summary> Solution </summary>

Correct! A. To ensure critical tasks will be serviced within timing deadlines.

Hard real-time scheduling ensures that critical tasks meet their specified deadlines. Missing a deadline can mean the system has failed to meet its requirements.

Option B describes delivering media files, but it does not explain why hard real-time scheduling is needed.

Which of the following is an example of a hard real-time system?
- [ ] A. Online video streaming
- [ ] B. Email delivery
- [x] C. An aircraft flight-control system
- [ ] D. Downloading a file

Correct! C. An aircraft flight-control system.

A hard real-time system must meet strict timing deadlines. Missing a deadline in an aircraft flight-control system could have serious safety consequences.

Online video streaming (A) generally uses soft real-time requirements, where occasional delays may be tolerable.

</details>

---

Q.21 Which of the following applications is a typical use of microcontrollers in the field of home automation?
- [ ] A. Satellite communication
- [ ] B. Air traffic control
- [x] C. Temperature and lighting control
- [ ] D. Space exploration

<details>
  <summary> Solution </summary>

Correct! C. Temperature and lighting control.

**Microcontrollers** are small, programmable computing units used to control devices. 

In home automation, they can monitor temperature and control air conditioners, thermostats, lights, and other appliances.

Which component is commonly used to detect room temperature in a home automation system?
- [x] A. Temperature sensor
- [ ] B. Loudspeaker
- [ ] C. Printer
- [ ] D. Keyboard

Correct! The answer is A. Temperature sensor.

A **temperature sensor** detects the room's temperature and sends readings to the microcontroller, which can then control heating or cooling devices.

</details>

---

Q.22 What is the purpose of SQL injection attacks?
- [ ] A. To increase the performance of database queries
- [x] B. To bypass authentication systems
- [ ] C. To improve database security
- [ ] D. To enhance data encryption

<details>
  <summary> Solution </summary>

Correct! B. To bypass authentication systems.

**SQL injection** is an attack in which an attacker inserts malicious SQL code into an application's database queries. It can be used to bypass login checks, access unauthorized data, or modify database records.


Which practice helps prevent SQL injection attacks?
- [ ] A. Storing passwords in plain text
- [x] B. Using prepared statements with parameterized queries
- [ ] C. Giving every user administrator privileges
- [ ] D. Disabling database backups

Correct! B. Using prepared statements with parameterized queries.

**Prepared statements** keep SQL commands separate from user-supplied input, helping prevent malicious input from changing the intended query.

> **Prepared statements = protection against SQL injection**.

</details>

---

Q.23 What is the primary purpose of data compression in data communication?
- [ ] A. To increase latency
- [x] B. To reduce bandwidth usage
- [ ] C. To decrease error rates
- [ ] D. To improve security

<details>
  <summary> Solution </summary>

Correct! B. To reduce bandwidth usage.

**Data compression** reduces the size of data before transmission. <br/>
This helps use less network bandwidth and can reduce transmission time.

> **Data compression -> smaller data size -> less bandwidth required.**

Which type of compression allows the original data to be reconstructed exactly?
- [ ] A. Lossy compression
- [x] B. Lossless compression
- [ ] C. Analog compression
- [ ] D. Irreversible compression

Correct! B. Lossless compression.

E**Lossless compression** reduces the size of data without losing any information. The original data can be reconstructed exactly.

Example: ZIP files and PNG images use lossless compression.

Remember for the exam:
- **Lossless**: Original data recovered exactly.
- **Lossy**: Some information is permanently discarded.

| Type	                       | Meaning                                               |
|------------------------------|-------------------------------------------------------|
| **Lossy compression**	       | Some information is permanently lost.                 |
|	**Lossless compression**	   | Original data is reconstructed exactly.               |
|	**Analog compression**	     | Not the standard answer for this digital-data question.|
|	**Irreversible compression** | The original data cannot be recovered exactly.        |

> **lossless = no data loss;** <br/>
> **lossy = some data loss.**

</details>

---

**OOP**

Q.24 What is the term for a variable that references an instance of a class?
- [ ] A. Property
- [ ] B. Method
- [x] C. Object
- [ ] D. Constructor

<details>
  <summary> Solution </summary>

Correct! C. Object.

An **object** is an instance of a class. <br/>
A variable can reference that object so you can access its properties and methods.

Example in Java:
```java
Car myCar = new Car();
```
Here, `Car` is the class, `new Car()` creates an object, and `myCar` is the reference variable.


In object-oriented programming, what is a constructor primarily used for?
- [x] A. To initialize a newly created object
- [ ] B. To destroy a class
- [ ] C. To store database records
- [ ] D. To return a value from every method

Correct! A. To initialize a newly created object.

A **constructor** is a special member of a class that runs when an object is created. <br/>
It is commonly used to initialize the object's data.

Example in Java:
```java
class Car {
    String color;

    Car(String c) {
        color = c;
    }
}
```
Here, `Car(String c)` is the constructor that initializes the car's color.

> **Constructor -> initializes an object.**

</details>

---

**Computer Networks**

Q.25 Which network device serves as the entry and exit point of a network, as all data
coming in or going out of a network must first pass through it?
- [ ] A. Modem
- [x] B. Gateway
- [ ] C. Switch
- [ ] D. Repeater

<details>
  <summary> Solution </summary>

Correct! B. Gateway.

A **gateway** connects different networks and serves as an entry and exit point for data moving between them.

Remember:
- **Gateway**: Connects different networks.
- **Switch**: Connects devices within a local area network (LAN).
- **Repeater**: Regenerates or boosts signals to extend network range.
- **Modem**: Modulates and demodulates signals.

Which network device forwards data frames to the correct device within a LAN using MAC addresses?
- [ ] A. Repeater
- [ ] B. Modem
- [x] C. Switch
- [ ] D. Gateway

Correct! C. Switch.

A **network switch** uses MAC addresses to forward data frames to the appropriate device within a LAN.

> **Switch -> MAC address -> forwards frames within a LAN.**

</details>

---

**Python Programming**

Q.26 Identify the correct output of the following code snippet :
```py
game="olympic2024"
print(game.index("C") ) # ValueError
print(game.find("C"))   # -1
```
- [ ] A. 0
- [ ] B. 6
- [ ] C. -1
- [x] D. valueError

<details>
  <summary> Solution </summary>

Correct! D. `ValueError`

`.index("C")` -> raises `ValueError` if not found.
`.find("C")` -> returns `-1` if not found.

| Method	    | If the substring is missing |
|-------------|-----------------------------|
| `.index()`	| Raises ValueError           |
| `.find()`	  | Returns `-1`                |

</details>

---

**Data Structures (B-Tree)**

Q.27 In a B tree of order `m`, each internal node can have up to __ children. 
- [ ] A. `m - 1`
- [x] B. `m`
- [ ] C. `2m - 1`
- [ ] D. `2m`

<details>
  <summary> Solution </summary>

Correct! B. `m`

In a B-tree of order `m`, an internal node can have at most `m` children and at most `m-1` keys.

For example, in a B-tree of order 4:
- Maximum children = 4
- Maximum keys = 3

> Exam tip: **Maximum children = `m`; maximum keys = `m-1`.

In a B-tree of order 5, what is the maximum number of keys a node can contain?
- [ ] A. 5
- [x] B. 4
- [ ] C. 10
- [ ] D. 9

Correct! B. 4 keys.

In a B-tree of order `m`, the maximum number of keys is `m-1`.

</details>

---

Q.28 Which of the following is the correct expansion of SMS ?
- [x] A. Short Message Service `p { font–family: Arial; }`
- [ ] B. Small Multimedia Service `p { fontfamily: Arial; }`
- [ ] C. Short Multimedia Service `p { font: Arial; }`
- [ ] D. Small Message Service `p { font–type: Arial; }`

<details>
  <summary> Solution </summary>

**SMS stands for Short Message Service**, which allows users to send and receive text messages on mobile phones.

> **SMS = Short Message Service**

What does MMS stand for?
- [ ] A. Mobile Messaging System
- [x] B. Multimedia Messaging Service
- [ ] C. Mobile Message Service
- [ ] D. Multiple Messaging System

Correct! B. Multimedia Messaging Service.

**MMS** allows users to send multimedia content, such as pictures, audio, and video, through messaging services.

Remember:
- **SMS = Short Message Service**
- **MMS = Multimedia Messaging Service**

</details>

---

**Media Access Control (MAC) Address**

Q.29 Which of the following statement (s) is/are TRUE in respect of Media Access Control (MAC) Address? <br/>
A. It can be changed if a node is removed from one network and connected to another network. <br/>
B. Each MAC address is a 12-digit hexadecimal number.  <br/>
C. It is a unique value associated with a network adapter called NIC. <br/>
D. It is provided by the Internet Service Provider to locate computers connected to the internet. <br/>
Choose the correct answer from the options given below: 
- [x] A. (B) and (C) only
- [ ] B. (A), (B) and (C) only
- [ ] C. (C) and (D) only
- [ ] D. (A) and (B) only

<details>
  <summary> Solution </summary>

Correct! A.

**Media Access Control(MAC) Address**

Moving a device to another network does not, by itself, change its MAC address. <br/>
A MAC address can sometimes be changed or spoofed, but not simply because the network changes.

A standard 48-bit MAC address is written as 12 hexadecimal digits <br/>
for example, `00:1A:2B:3C:4D:5E`.

A MAC address is associated with a **network interface controller (NIC)**.

An **ISP(Internet Service Provider)** typically assigns an IP address, not the device's MAC address.

> **MAC address -> Layer 2, NIC, 48 bits;** <br/>
> **IP address -> Layer 3, logical addressing.**

Which OSI layer primarily uses MAC addresses to forward frames?
- [ ] A. Physical layer
- [ ] B. Data Link layer
- [x] C. Network layer
- [ ] D. Transport layer

Correct! B. Data Link layer.

The **Data Link layer(Layer 2)** uses MAC addresses to identify devices on a local network and forward data frames.

Remember:
- **Layer 2 - Data Link: MAC addresses and frames**
- **Layer 3 - Network: IP addresses and packets**

</details>

---

**SQL Constraints**

Q.30 While creating a table, which constraint does not allow insertion of duplicate values in the table ?
- [x] A. `UNIQUE`
- [ ] B. `DISTINCT`
- [ ] C. `NOT NULL`
- [ ] D. `HAVING`

<details>
  <summary> Solution </summary>

Correct! A. `UNIQUE`

The `UNIQUE` constraint prevents duplicate values in a column or combination of columns in a table.

| SQL keyword	| Purpose                                   |
|-------------|-------------------------------------------|
| `UNIQUE`	  | Prevents duplicate values                 |
| `DISTINCT`	| Removes duplicate rows from query results |
| `NOT NULL`	| Prevents NULL values                      |
| `HAVING`	  | Filters groups after `GROUP BY `          |

Which SQL constraint prevents a column from containing `NULL` values?
- [ ] A. `UNIQUE`
- [ ] B. `DEFAULT`
- [x] C. `NOT NULL`
- [ ] D. `CHECK`

Correct! C. `NOT NULL`

The `NOT NULL` constraint ensures that a column must contain a value and cannot be left `NULL`.

Example:
```sql
CREATE TABLE Student (
    name VARCHAR(50) NOT NULL
);
```
Here, the `name` column cannot contain a `NULL` value.

Remember:
- `UNIQUE` -> prevents duplicate values.
- `NOT NULL` -> prevents NULL values.


</details>

---

**Object-Oriented Programming (OOP)**

Q.31 Which term is used to describe the ability of different classes to be treated as objects of the same parent class?
- [ ] A. Overloading
- [x] B. Polymorphism
- [ ] C. Abstraction
- [ ] D. Encapsulation

<details>
  <summary> Solution </summary>

Correct! B. Polymorphism.

**Polymorphism** means "many forms". <br/>
It allows objects of different classes to be treated through a common parent-class interface, while each object can provide its own behavior.

Remember :
- **Polymorphism**: One interface, different behaviors.
- **Encapsulation**: Bundles data and methods together.
- **Abstraction**: Hides implementation details.
- **Overloading**: Uses the same function or method name with different parameter lists.

Suppose `Dog` and `Cat` both inherit from `Animal`, and each provides its own implementation of `makeSound()`. Which OOP concept does this demonstrate?
- [ ] A. Encapsulation
- [ ] B. Abstraction
- [x] C. Polymorphism
- [ ] D. Constructor

Correct C. Polymorphism

Both `Dog` and `Cat` inherit from `Animal`, but each can implement `makeSound()` differently. <br/>
This is **polymorphism** - the same method call can produce different behavior depending on the object.

For example:
- `Dog.makeSound()` -> Bark
- `Cat.makeSound()` -> Meow

 > **Same interface, different behavior = Polymorphism**.

</details>

---

**Artificial Intelligence (Frame Structures)**

Q.32 Building blocks of a frame structure are?
- [ ] A. Facts and Data
- [x] B. Procedure and Default values
- [ ] C. Frame names
- [ ] D. Frame inference in hierarchy

<details>
  <summary> Solution </summary>

Correct! B. Procedure and Default values.

In AI, a **frame** represents knowledge about an object or situation. <br/>
A frame typically contains slots (attributes) and facets that describe information such as default values, constraints, or procedures.

- **Facts and data** are knowledge that may be stored in frames, but they are not the most specific option here.
- **Procedure and default values** are associated with frame slots and their facets.

In an AI frame, what is a slot primarily used for?
- [x] A. To store an attribute or property of an object
- [ ] B. To execute machine instructions
- [ ] C. To connect computers in a network
- [ ] D. To encrypt stored information

Correct! A. To store an attribute or property of an object.

In an AI frame, a **slot** represents an attribute or property, such as a person's name, age, or address. <br/>
Its value can describe that property.

Example:
- Frame: `Car`
- Slot: `Colour`
- Value: `Red`

> **Frame = knowledge representation;** 

> **Slot = attribute;**

> **value = information stored in the slot.**

</details>

---

**Operating Systems (Memory Management)**

Q.33 Segmentation is a memory management technique where memory is divided into segments, with each segment containing:
- [ ] A. Fixed-sized blocks of memory
- [ ] B. Different types of data structures
- [x] C. Variable-sized blocks of memory
- [ ] D. Non-contiguous blocks of memory

<details>
  <summary> Solution </summary>

Correct! C. Variable-sized blocks of memory.

In segmentation, a program is divided into logical units such as code, data, and stack. <br/>
These segments can have different sizes.

- **Segmentation**: Variable-sized segments.
- **Paging**: Fixed-sized blocks called **pages (in logical memory)** and **frames (in physical memory)**.

<img width="990" height="320" alt="image" src="https://github.com/user-attachments/assets/20599b92-9373-4baa-a56d-83ecc6007684" />


<img width="1000" height="660" alt="image" src="https://github.com/user-attachments/assets/a92aad31-5045-4315-961e-3148b0cc5937" />


In paging, what is the size of each page within a given paging system?
- [ ] A. Variable, depending on the program
- [x] B. Fixed
- [ ] C. Always equal to the entire program size
- [ ] D. Determined by the size of the data segment


| Paging	                         | Segmentation                         |
|----------------------------------|--------------------------------------|
| Fixed-sized pages	               | Variable-sized segments              |
| Divides memory into equal blocks | Divides a program into logical units | 
| Uses a page table	               | Uses a segment table                 |

> **Paging = equal pieces; segmentation = meaningful pieces.**

If a paging system uses a page size of 4 KB, what is the size of every page in that system?
- [ ] A. It varies for each page
- [x] B. 4 KB
- [ ] C. It equals the whole program size
- [ ] D. It depends on the data segment

</details>

---


Q.34 About IoT, which among the followings is not correct?
- [ ] A. Light sensor is analog
- [ ] B. microphone is a digital sensor
- [ ] C. Keyboard is a digital sensor
- [ ] D. Push button is a digital Sensor

<details>
  <summary> Solution </summary>


</details>

Q.35 Connected components in a graph can be found using which graph traversal
algorithm?
- [ ] A. DFS
- [ ] B. BFS
- [ ] C. Both DFS and BFS
- [ ] D. Neither DFS nor BFS

<details>
  <summary> Solution </summary>


</details>

Q.36 A complex SCADA system has _______levels?
- [ ] A. 6
- [ ] B. 5
- [ ] C. 3
- [ ] D. 4

<details>
  <summary> Solution </summary>


</details>

Q.37 Hierarchical addressing in the Network Layer allows for:
- [ ] A. More efficient use of IP addresses
- [ ] B. Dynamic allocation of MAC addresses
- [ ] C. Faster data transmission rates
- [ ] D. Reduced latency in data communication

<details>
  <summary> Solution </summary>


</details>

Q.38 According to Chomsky hierarchy, which of the following is recognized by Recursively
Enumerable language?
- [ ] A. Type 0
- [ ] B. Type 1
- [ ] C. Type 2
- [ ] D. Type 3

<details>
  <summary> Solution </summary>


</details>

Q.39 Which SQL clause is used to retrieve specific rows from a table?
- [ ] A. `SEARCH`
- [ ] B. `FETCH`
- [ ] C. `SELECT`
- [ ] D. `FIND`

<details>
  <summary> Solution </summary>


</details>

Q.40 In conditional asymptotic notation, "`Θ(f(n)) if g(n)`" indicates that the algorithm's
complexity is both upper and lower bounded by `f(n)` when:
- [ ] A. `g(n)` is a lower bound on `f(n)`
- [ ] B. `g(n)` is an upper bound on `f(n)`
- [ ] C. `g(n)` is true
- [ ] D. `g(n)` is false

<details>
  <summary> Solution </summary>


</details>

Q.41 The OSI model consists of how many layers?
- [ ] A. 5
- [ ] B. 6
- [x] C. 7
- [ ] D. 8

<details>
  <summary> Solution </summary>


</details>

Q.42 In a relational database, what is a primary key?
- [ ] A. A key used for opening encrypted data
- [ ] B. A unique identifier for a record in a table @
- [ ] C. A foreign key from another table
- [ ] D. An index for sorting data

<details>
  <summary> Solution </summary>


</details>

Q.43 What will be the output of the following code segment?
```py
a = 5
def func_1(b=10):
global a
a=b-10
b+=a
print (a,b)
func_1(a)
```
- [ ] A. 0 5
- [ ] B. 5 0
- [ ] C. 0 -5
- [ ] D. -5 0

<details>
  <summary> Solution </summary>


</details>

Q.44 Which JavaScript method is used to add a new HTML element to the DOM?
- [ ] A. `appendElement()`
- [ ] B. `createElement()`
- [ ] C. `newElement()`
- [ ] D. `addElement()`

<details>
  <summary> Solution </summary>


</details>

Q.45 The primary function of firewall in network security is
- [ ] A. To monitor network traffic and detect anomalies.
- [ ] B. To create virtual private networks for secure communication.
- [ ] C. To filter incoming and outgoing network traffic based on security rules
- [ ] D. To encrypt data before Transmission

<details>
  <summary> Solution </summary>


</details>

Q.46 In AI systems, Knowledge can be represented in two ways. What are these two ways? <br/>
i. Machine Logic <br/>
ii. Predicate Logic <br/>
iii. Propositional Logic <br/>
iv. Compound Logic
- [ ] A. (i) and (ii)
- [ ] B. (i) and (iii)
- [ ] C. (ii) and (iii)
- [ ] D. (iii) and (vi)

<details>
  <summary> Solution </summary>


</details>

Q.47 What is the difference between a URL and a web address?
- [ ] A. A URL is a Uniform Resource Locator, while a web address is away to identify a
website on the internet.
- [ ] B. A URL is a software program, while a web address is ahardware device.
- [ ] C. A URL is a physical object, while a web address is a logicalobject.
- [ ] D. All of the above.

<details>
  <summary> Solution </summary>


</details>

Q.48 Monitors are primarily used for achieving:
- [ ] A. Deadlocks
- [ ] B. Starvation
- [ ] C. Mutual exclusion and synchronization
- [ ] D. Process termination

<details>
  <summary> Solution </summary>


</details>

Q.49 In EDI, I stands for?
- [ ] A. Indian
- [ ] B. India
- [x] C. Interchange
- [ ] D. Interval

<details>
  <summary> Solution </summary>


</details>

Q.50 Which protocol provides connectionless communication with minimal overhead?
- [ ] A. TCP
- [ ] B. UDP
- [ ] C. IP
- [ ] D. HTTP

<details>
  <summary> Solution </summary>


</details>

Q.51 Which maintenance activity involves updating software to work with new hardware or
software environments?
- [ ] A. Corrective Maintenance
- [ ] B. Adaptive Maintenance
- [ ] C. Perfective Maintenance
- [ ] D. Preventive Maintenance

<details>
  <summary> Solution </summary>

</details>

Q.52 A formal model of protection in an operating system provides:
- [ ] A. A mathematical framework for analyzing resource allocation
- [ ] B. Guidelines for designing user interfaces
- [ ] C. Methods for optimizing memory management
- [ ] D. Techniques for improving CPU utilization

<details>
  <summary> Solution </summary>

</details>

Q.53 minimum number of states required to recognize an octal number divisible by 3 are/is
- [ ] A. 3
- [ ] B. 4
- [ ] C. 1
- [ ] D. 2

<details>
  <summary> Solution </summary>

</details>

Q.54 Which command is used to remove a relation from an SQL?
- [ ] A. Drop table
- [ ] B. Delete
- [ ] C. Purge
- [ ] D. Remove

<details>
  <summary> Solution </summary>

</details>

Q.55 What does the term "Software Maintenance" refer to?
- [ ] A. Developing new software applications
- [ ] B. Enhancing software performance
- [ ] C. Managing hardware components
- [ ] D. Modifying and updating existing software

<details>
  <summary> Solution </summary>

</details>

Q.56 The recurrence equation `T(n) = T(n/2) + T(n/3) + n` represents the time complexity of
which algorithmic paradigm?
- [ ] A. Divide and Conquer
- [ ] B. Dynamic Programming
- [ ] C. Greedy Algorithms
- [ ] D. Backtracking

<details>
  <summary> Solution </summary>

</details>

Q.57 What does the term "harvard architecture" refer to in the context of microcontrollers?
data
- [ ] A. A type of microcontroller with high processing speed
- [ ] B. A microcontroller architecture that uses a separate memory space for instructions and
- [ ] C. A microcontroller with advanced addressing modes
- [ ] D. A microcontroller with a large number of I/O ports

<details>
  <summary> Solution </summary>

</details>

Q.58 Consider the statements given below and then choose the correct output from the
given options :
```py
L=['TIC' , 'TAC' ]
print (L[::-1])
```
- [ ] A. ['CIT' , 'CAT' ]
- [ ] B. ['TIC' , 'TAC' ]
- [ ] C. ['CAT' , 'CIT' ]
- [ ] D. ['TAC' , 'TIC' ]

<details>
  <summary> Solution </summary>

</details>

Q.59 Which of the following is not an attribute of the tag ?
- [ ] A. face
- [ ] B. height
- [ ] C. size
- [ ] D. colour

<details>
  <summary> Solution </summary>

</details>

Q.60 The term "multi-user" in an OS context refers to:
- [ ] A. An OS that can execute multiple programs simultaneously
- [ ] B. An OS that supports multiple users working on the same machine
- [ ] C. An OS that can only run on multiple computers
- [ ] D. An OS with a graphical user interface

<details>
  <summary> Solution </summary>

</details>

Q.61 TPDU (Transport Protocol Data Unit) refers to:
- [ ] A. A unit of data in the physical layer
- [ ] B. A unit of data in the data link layer
- [ ] C. A unit of data in the transport layer
- [ ] D.   A unit of data in the network layer

<details>
  <summary> Solution </summary>

</details>

Q.62 **`A*` search algorithm** is based on?
- [ ] A. BFS
- [ ] B. DFS
- [ ] C. Uniform cost search
- [ ] D. Best first Search

<details>
  <summary> Solution </summary>

</details>

Q.63 What is the primary purpose of using Don't Care conditions in Karnaugh Map
simplification?
- [ ] A. To mark cells that should not be included in the simplification process
- [ ] B. To indicate cells that have an undefined logic value
- [ ] C. To identify cells that are already in their simplest form
- [ ] D. To mark cells with special logic functions

<details>
  <summary> Solution </summary>

</details>

Q.64 Which among the followins is not a type of Zigbee Device?
- [ ] A. Zigbee Coordinator device
- [ ] B. Zigbee Router
- [ ] C. Zigbee start devce
- [ ] D. Zigbee end devce

<details>
  <summary> Solution </summary>

</details>

Q.65 Zigbee is a task group in-----
- [ ] A. LAN
- [ ] B. PAN
- [ ] C. MAN
- [ ] D. WAN

<details>
  <summary> Solution </summary>

</details>

Q.66 In a threaded binary tree, the space required for threads is usually:
- [ ] A. Greater than the space required for regular pointers
- [ ] B. Equal to the space required for regular pointers
- [ ] C. Less than the space required for regular pointers
- [ ] D. Unpredictable

<details>
  <summary> Solution </summary>

</details>

Q.67 Given the Boolean expression `F(A, B, C, D) = Σ(0, 1, 2, 3, 8, 9, 10, 11)`, what is the
simplified expression using the algebraic method?
- [ ] A. A + B + C + D
- [ ] B. AB + AC + AD + BC + BD + CD
- [ ] C. AB + CD
- [ ] D. A'BC'D + ABC'D + A'BCD + ABCD

<details>
  <summary> Solution </summary>

</details>

Q.68 Which model considers risk assessment and incremental development in software
projects?
- [ ] A. Waterfall Model
- [ ] B. Agile Model
- [x] C. Prototype Model
- [ ] D. Spiral Model

<details>
  <summary> Solution </summary>

</details>

Q.69 Which of the following expression in SQL would calculate the square root of 16?
- [ ] A. `POWER (16,2)`
- [ ] B. `POWER (16, 0.5)`
- [ ] C. `POWER (16, 1)`
- [ ] D. `MOD (16)`

<details>
  <summary> Solution </summary>

</details>


Q.70 A relation in a relational database is also known as:
- [ ] A. A data type
- [ ] B. An attribute
- [ ] C. A schema
- [ ] D. A table

<details>
  <summary> Solution </summary>

</details>



Q.71 A Database Management System is a type of _________software.
- [ ] A. It is a type of system software
- [ ] B. It is a kind of application software
- [ ] C. It is a kind of general software
- [ ] D. Both A and C

<details>
  <summary> Solution </summary>

</details>


Q.72 A grammar that produces more than one parse tree for the same sentence is called
- [ ] A. Contiguous
- [ ] B. Ambiguous
- [ ] C. Unambiguous
- [ ] D. Regular

<details>
  <summary> Solution </summary>

</details>


Q.73 Which traversal technique is used to visit each node of a linked list exactly once?
- [ ] A. Preorder traversal
- [ ] B. Inorder traversal
- [ ] C. Postorder traversal
- [ ] D. Linear traversal

<details>
  <summary> Solution </summary>

</details>


Q.74 Which of the following is not a Search Engine available over the Internet ?
- [ ] A. Google
- [ ] B. Bing
- [ ] C. Diksha
- [ ] D. Yahoo

<details>
  <summary> Solution </summary>

</details>


Q.75 In a PLA, what components are used to implement the combinational logic functions?
- [ ] A. `AND` gates and `OR` gates
- [ ] B. `NAND` gates and `XOR` gates
- [ ] C. `NOR` gates and `XNOR` gates
- [ ] D. `NOT` gates and `multiplexers`

<details>
  <summary> Solution </summary>

</details>


Q.76 Which protocol is used for sending emails?
- [ ] A. HTTP
- [ ] B. FTP
- [ ] C. SMTP
- [ ] D. SNMP

<details>
  <summary> Solution </summary>

</details>


Q.77 …………….are the unorganized facts that can be processed to generate meaningful
information.
- [ ] A. Information
- [ ] B. Data
- [ ] C. Blog
- [ ] D. contexts

<details>
  <summary> Solution </summary>

</details>


Q.78 Which one of the following resource is not necessarily required on a file server?
- [ ] A. secondary storage
- [ ] B. processor
- [ ] C. network
- [ ] D. monitor

<details>
  <summary> Solution </summary>

</details>


Q.79 The letter S in the abbreviation HTTPS in context of Networking protocols, stands for :
- [ ] A. Single
- [ ] B. Static
- [ ] C. Secure
- [ ] D. Sensitive

<details>
  <summary> Solution </summary>

</details>


Q.80 Which version control system is commonly used for collaborative web development projects?
- [ ] A. SVN
- [ ] B. Git
- [ ] C. Mercurial
- [ ] D. CVS

<details>
  <summary> Solution </summary>

</details>


Q.81 The term "DFD" stands for?
- [ ] A. Data file diagram
- [ ] B. Data flow document
- [ ] C. Data flow diagram
- [ ] D. None of the above

<details>
  <summary> Solution </summary>

</details>


Q.82 Which symbol is used to define the start and end of `XML` tags?
- [ ] A.  ` `  
- [ ] B. `{ }`
- [ ] C. `[ ]`
- [ ] D. `( )`

<details>
  <summary> Solution </summary>

</details>


Q.83 What is the full form of FTP ?
- [ ] A. File Transfer Protocol
- [ ] B. File Transmission Protocol
- [ ] C. Fast Transfer Protocol
- [ ] D. Fast Transmission Protocol

<details>
  <summary> Solution </summary>

</details>


Q.84 The language accepted by Push down Automaton:
- [ ] A. Recursive Language
- [ ] B. Context free language
- [ ] C. Linearly Bounded language
- [ ] D. All of the mentioned


<details>
  <summary> Solution </summary>

</details>


Q.85 What is an encryption system that uses two keys: a public key that everyone can have
and a private key for only the recipient?
- [ ] A. Encryption
- [ ] B. IDS
- [ ] C. Security Audit software
- [ ] D. Public key Encryption

<details>
  <summary> Solution </summary>

</details>


Q.86 Let u='1101', v='0001', then uv=11010001 and vu= 00011101. Using the given information
what is the identity element for the string?
Ans
- [ ] A. `u-1`
- [ ] B. `v-1`
- [ ] C. `u-1v-1`
- [ ] D. `ε`

<details>
  <summary> Solution </summary>

</details>


Q.87 Which keyword is used to create an instance of a class in most programming
languages?
- [ ] A. `alloc`
- [ ] B. `new`
- [ ] C. `create`
- [ ] D. `instance`

<details>
  <summary> Solution </summary>

</details>


Q.88 Which of the following is known as a set of entities of the same type that share same
properties, or attributes?
- [ ] A. Relation set
- [ ] B. Tuples
- [ ] C. Entity set
- [ ] D. Entity Relation model

<details>
  <summary> Solution </summary>

</details>


Q.89 What is the time complexity of Merge Sort for sorting an array of size "n"?
- [ ] A. `O(n)`
- [ ] B. `O(log n)`
- [ ] C. `O(n log n)`
- [ ] D. `O(n^2)`

<details>
  <summary> Solution </summary>

</details>


Q.90 Maximum read range of RFID module is?
- [ ] A. 10 CM
- [ ] B. 5 CM
- [ ] C. 15 CM
- [ ] D. 2 CM

<details>
  <summary> Solution </summary>

</details>


Q.91 Which type of register is primarily used to temporarily hold data during arithmetic and
logical operations in a microprocessor?
- [ ] A. Shift register
- [ ] B. Parallel register
- [ ] C. Accumulator register
- [ ] D. Counter register

<details>
  <summary> Solution </summary>

</details>


Q.92   Safeguards in an operating system are mechanisms used to:
- [ ] A. Ensure the efficient utilization of CPU time
- [ ] B. Prevent data loss during power outages
- [ ] C. Enhance the performance of I/O operations
- [ ] D. Protect against unauthorized access and security breaches

<details>
  <summary> Solution </summary>

</details>



Q.93 Which of the following is a service for real-time text communication on the internet ?
- [ ] A. e-Learning
- [ ] B. FTP
- [ ] C. Video conferencing
- [x] D. Chat

<details>
  <summary> Solution </summary>

</details>


Q.94 If the dictionary D1 is defined as: `D1 = {1: 'a', 2: 'b'}`
then which of the following statements is incorrect and hence will result in an error?
- [ ] A. `D1.get (1)`
- [ ] B. `D1.get (3)`
- [ ] C. `D1.del (1)`
- [ ] D. `D1.clear (1)`

<details>
  <summary> Solution </summary>

</details>


Q.95 Telnet is commonly used for:
- [ ] A. Secure file transfers
- [ ] B. Remote terminal access
- [ ] C. Web browsing
- [ ] D.   Email communication

<details>
  <summary> Solution </summary>

</details>



Q.96 Separate chaining involves storing collided elements in separate data structures,
typically in:
- [ ] A. Linked lists
- [ ] B. Arrays
- [ ] C. Stacks
- [ ] D. Queues

<details>
  <summary> Solution </summary>

</details>


Q.97 PDA can be represented with the help of
- [ ] A. Instantaneous description
- [ ] B. Transition diagram
- [ ] C. Transition table
- [ ] D. All of these

<details>
  <summary> Solution </summary>

</details>


Q.98 Which Karnaugh Map simplification technique involves grouping cells that are not
adjacent but share a common variable value?
- [ ] A. Pair simplification
- [ ] B. Quad simplification
- [ ] C. Octet simplification
- [ ] D. Group simplification

<details>
  <summary> Solution </summary>

</details>


Q.99 which of the following is/ are components of Expert Systems?
- [ ] A. Knowledge Base
- [ ] B. Inference logic
- [ ] C. User Interface
- [ ] D. All of the above

<details>
  <summary> Solution </summary>

</details>

Q.100 Arrange the following electromagnetic waves in increasing order of their frequency
range.
A. Microwaves <br/>
B. Infrared Waves <br/>
C. Light Waves <br/>
D. Radio Waves <br/>
Choose the correct answer from the options given below :
- [ ] A. (A), (C), (D), (B)
- [ ] B. (D), (C), (B), (A)
- [ ] C. (B), (A), (D), (C)
- [ ] D. (D), (A), (B), (C)

<details>
  <summary> Solution </summary>

</details>


Q.101 The mirror of the Society is:
- [ ] A. playground
- [ ] B. community
- [ ] C. Hospital
- [ ] D. Schoo

<details>
  <summary> Solution </summary>

</details>



Q.102 The number of domains in taxonomies of educational objective is
- [ ] A. Two
- [ ] B. Three
- [ ] C. Five
- [ ] D. Six

<details>
  <summary> Solution </summary>

</details>


Q.103 Who has developed the 'Guidelines on information literacy for lifelong learning?
- [ ] A. RUSA
- [ ] B. ACRL
- [ ] C. SCONUL
- [ ] D. IFLA

<details>
  <summary> Solution </summary>

</details>


Q.104 Which type of lesson plan is simple and straightforward?
- [ ] A. Daily lesson plan
- [ ] B. Weekly lesson plan
- [ ] C. Sequential lesson plans
- [ ] D. Monthly lesson plan

<details>
  <summary> Solution </summary>

</details>



Q.105 The most natural and simple way of teaching a lesson is to proceed from <br/>
Statement I. something that the students already know <br/>
Statement II. those facts which are unknown to the learners <br/>
Statement III. Examples <br/>
Statement IV. Illustrations <br/>
Choose the correct option:
- [ ] A. I, III and IV
- [ ] B. Only I
- [ ] C. Only II
- [ ] D. III and IV

<details>
  <summary> Solution </summary>

</details>


Q.106 Which one of the following options best describes progressive education?
- [ ] A. Learning by doing, project method, cooperative learning
- [ ] B. Thematic units, regular unit tests, ranking
- [ ] C. Personalized learning, ability grouping, labelling students
- [ ] D. Project method, ability grouping, ranking

<details>
  <summary> Solution </summary>

</details>


Q.107 In M.C.Q the correct option is:
- [ ] A. Response
- [ ] B. Answer
- [ ] C. Distractors
- [ ] D. None of these

<details>
  <summary> Solution </summary>

</details>


Q.108 Which of the following is a sign of motivated teaching?
- [ ] A. Maximum presence of students in the class
- [ ] B. Asking questions by students
- [ ] C. Pin drop silence in the class
- [ ] D. Complition of home assignment

<details>
  <summary> Solution </summary>

</details>


Q.109 In M.C.Qs the statement of the problem is:
- [ ] A. Option
- [ ] B. Distractor
- [ ] C. Premise
- [ ] D. Stem

<details>
  <summary> Solution </summary>

</details>


Q.110 The stage in problem solving that includes the preparation of suitable hypothesis for
investigation.
- [ ] A. Survey
- [ ] B. Planning for action
- [ ] C. Problem description
- [ ] D. Discussion

<details>
  <summary> Solution </summary>

</details>



Q.111 While discussing about friction, a teacher gave a number of examples to explain the
concept. Some of the examples where friction is useful in our day-to-day life as-quoted
by the teacher are given below. <br/>
I. We are able to write because of friction between the tip of the pen and the paper. <br/>
II. We are able to walk because of friction between our feet and the ground. <br/>
III. A ball thrown vertically upwards comes back to us due to friction. <br/>
IV. We are able to stop a moving vehicle by applying brakes because of friction. <br/>
The correct examples were
- [ ] A. III, IV and I
- [ ] B. IV, I and II
- [ ] C. I, III and IV
- [ ] D. II, III and IV

<details>
  <summary> Solution </summary>

</details>


Q.112  Having variety of question sets in a question paper increases it __________
- [ ] A. Objectivity
- [ ] B. Reliability
- [ ] C. Validity
- [ ] D. Difficulty

<details>
  <summary> Solution </summary>

</details>



Q.113 If you join a teacher fraternity and choose to dress like most of the others in your
group, you are exhibiting
- [ ] A. group identity
- [ ] B. group obedience
- [ ] C. group compliance
- [ ] D. group conformity

<details>
  <summary> Solution </summary>

</details>



Q.114 What is the 4 steps for constructing a test ?
- [ ] A. Planning and preparing the test
- [ ] B. Try Out the test
- [ ] C. Evaluating the test
- [ ] D. All of these

<details>
  <summary> Solution </summary>

</details>


Q.115 Continuous and Comprehensive evaluation was initiated by:
- [ ] A. NCTE
- [ ] B. CBSE
- [x] C. NCERT
- [ ] D. SCERT

<details>
  <summary> Solution </summary>

</details>


Q.116 Learning is generally considered as a permanent change in behavior' based on
- [x] A. Practice and experience.
- [ ] B. Practice and challenge.
- [ ] C. Challenge and experience.
- [ ] D. Challenge and reinforcement.


<details>
  <summary> Solution </summary>

</details>


Q.117 The characteristics of discussion method is
- [ ] A. Ensure maximum participation
- [ ] B. Students have the opportunity to criticize and evaluate.
- [ ] C. Logical and meaningful criticism should be accepted
- [x] D. All of them

<details>
  <summary> Solution </summary>

</details>


Q.118 Which of the following teaching method is focused on the development of creative minds?
- [ ] A. Project 
- [x] B. Brain storming
- [ ] C. Observation 
- [ ] D. Demonstration


<details>
  <summary> Solution </summary>

</details>


Q.119 Which type of lesson plan is concise and focused on specific concepts or skills?
- [ ] A. Sequential lesson plans
- [ ] B. Weekly lesson plan
- [x] C. Daily lesson plan
- [ ] D. Monthly lesson plan

<details>
  <summary> Solution </summary>

</details>


Q.120 The 5E learning cycle boosts student engagement and motivation through
- [x] A. Constructivist approach
- [ ] B. Humanistic approach
- [ ] C. Naturalistic approach
- [ ] D. Pragmatist approach

<details>
  <summary> Solution </summary>

</details>


Q.121 The part of the curriculum designed to meet the needs of all students is:
- [ ] A. General education
- [x] B. Specialized education
- [ ] C. The extra-curriculum
- [ ] D. The program of studies

<details>
  <summary> Solution </summary>

</details>



Q.122. To demonstrate success by focusing on the learner’s desired outcome, a reasonable list of 
_____________objectives should be provided.
- [ ] A. Informational
- [ ] B. Mastery
- [ ] C. Challenging
- [ ] D. General

<details>
  <summary> Solution </summary>

</details>


Q.123 In comparing lecture and demonstration lessons, which one of the following is not
true?
- [ ] A. Slow children derive benefit from a lecture than brighter one
- [ ] B. There are more activities for the students in a demonstration lesson
- [ ] C. The lecture method is more conductive and useful for larger group
- [ ] D. It is difficult to ascertain students' learning in a lecture session

<details>
  <summary> Solution </summary>

</details>


Q.124 Which one of the following is the duty of a class teacher?
- [ ] A. Check the books, exercise books and bages of the students suddenly
- [ ] B. Check the lunch boxes of the students and advise them to take healthy food
- [ ] C. Check cleanliness of the class
- [ ] D. All of these

<details>
  <summary> Solution </summary>

</details>


Q.125 The most expected immediate outcome of teaching is
- [ ] A. Changes in the behavior of students in a desirable direction.
- [ ] B. Development of the total personality of students.
- [ ] C. Building characters of the students.
- [ ] D. Getting selected for a suitable job.

<details>
  <summary> Solution </summary>

</details>



Q.126 To select subject matter, one should consider student’s:
- [ ] A. I.Q
- [ ] B. Class
- [ ] C. Health
- [ ] D. Physical age

<details>
  <summary> Solution </summary>

</details>



Q.127 Micro teaching was first adopted at Stanford University by
- [ ] A. Stephen M Corey
- [ ] B. Dwight W Allen
- [ ] C. John Dewey
- [ ] D. Arthur Cunningham

<details>
  <summary> Solution </summary>

</details>



Q.128 Introduce a problem that students might not be able to solve yet is an example of
- [ ] A. Explore
- [ ] B. Engage
- [ ] C. Explain
- [ ] D. Elaborate

<details>
  <summary> Solution </summary>

</details>



Q.129 Full form of SIOP Model is
- [ ] A. Sheltered Intervention Observation Protocol
- [x] B. Sheltered Instruction Observation Protocol
- [ ] C. Sheltered Instruction Objection Protocol
- [ ] D. Sheltered Intervention Objection Protocol

<details>
  <summary> Solution </summary>

</details>


Q.130 Which one of the following is the most suitable to improve children's learning?
- [ ] A. Regular assessment test should be conducted.
- [ ] B. Teacher should explain the content using different examples and illustrations.
- [ ] C. All types of learning material should be there in the class.
- [ ] D. Teacher should facilitate children to interact with each other on real-life situations.

<details>
  <summary> Solution </summary>

</details>


Q.131 Which one among the following is NOT a major oil field located in Gujarat?
- [ ] A. Ankaleshwar
- [ ] B. Kosamba
- [ ] C. Mehsana
- [ ] D. Moran

<details>
  <summary> Solution </summary>

</details>


Q.132 Who among the following is the author of the book 'The Indian Struggle 1920 - 1942' ?
- [ ] A. Vinayak Damodar Savarkar
- [ ] B. Subhas Chandra Bose
- [ ] C. Vallabhbhai Patel
- [ ] D. Sarat Chandra Bose

<details>
  <summary> Solution </summary>

</details>


Q.133 7 is to 34 as 5 is to ?
- [ ] A. 33
- [ ] B. 24
- [ ] C. 54
- [ ] D. 41

<details>
  <summary> Solution </summary>

</details>



Q.134 Chronologically arrange the following political events related to Indian National
Movement beginning from the earliest :
1. Formation of Swaraj Party
2. Communal Award
3. Lucknow Pact
4. Simla Conference
Select the correct answer from the given options:
- [ ] A. 3, 1, 2, 4
- [ ] B. 1, 3, 2, 4
- [ ] C. 2, 1, 4, 3
- [ ] D. 1, 2, 3, 4


<details>
  <summary> Solution </summary>

</details>


Q.135 As per the Cabinet Resolution of 1st January 2015, the NITI Aayog consists of :
1. Prime Minister of India
2. Governing Council comprising of Chief Minister of all the States and Leiutenant
Governors of Union Territories
3. Rural Development Minister
4. Chief Executive Officer to be appointed by the Prime Minister
Select the correct answer from the given options :
- [ ] A. 1, 2 and 3
- [ ] B. 1, 2 and 4
- [ ] C. 1 and 2 only
- [ ] D. 3 and 4 only


<details>
  <summary> Solution </summary>

</details>


Q.136 Which nutrient protects us from diseases?
- [ ] A. Vitamin and minerals
- [ ] B. Fats and carbohydrates
- [ ] C. Protein
- [x] D. All of these

<details>
  <summary> Solution </summary>

</details>


Q.137 In the given letter series what letter will come in place of the question Symbol.
DIL, GLO, JOR, ?
- [ ] A. MRV
- [ ] B. MRQ
- [ ] C. MRU
- [ ] D. NRO

<details>
  <summary> Solution </summary>

</details>


Q.138 B is the Aunt of C. A is the Husband of B. B is the sister of D. Tell how A is related to D?
- [ ] A. Uncle
- [ ] B. Brother-in-Law
- [ ] C. Niece
- [ ] D. Son


<details>
  <summary> Solution </summary>

</details>


Q.139 The joint between separate faces of a solid is called an…...............
- [ ] A. edge
- [ ] B. face
- [ ] C. vertex
- [ ] D. None of these

<details>
  <summary> Solution </summary>

</details>


Q.140 Which is the longest National Highway in India?
- [ ] A. NH 5
- [ ] B. NH 44
- [ ] C. NH 10
- [ ] D. NH 15

<details>
  <summary> Solution </summary>

</details>


Q.141 Aaron weight 49 kg 357 g and Ron weights 32 kg 458 g. Who weighs less and by how
much?
- [ ] A. Ron weighs less by 16 kg 899 g
- [ ] B. Aaron weighs less by 16 kg 899 g
- [ ] C. Ron weighs more by 16 kg 899 g
- [ ] D. Aaron weighs more by 16 kg 899 g

<details>
  <summary> Solution </summary>

</details>


Q.142 If we combine two consecutive triangular numbers, we get?
- [ ] A. Rational Number
- [ ] B. Whole Number
- [ ] C. Perfect Square
- [ ] D. Prime Number


<details>
  <summary> Solution </summary>

</details>


Q.143 Which of the following is a waterborne disease?
- [ ] A. Measles
- [ ] B. malaria
- [ ] C. Lung disease
- [ ] D. Hepatitis

<details>
  <summary> Solution </summary>

</details>


Q.144 “Family is a unit consisting of a mother, father and their two children”. This statement is
- [ ] A. incorrect, because the statement should specify that the children are biological
- [ ] B. incorrect, because there are many kinds of families and one cannot classify family as
being of only one kind
- [ ] C. correct, since this is an ideal family size
- [ ] D. correct, because this is what all Indian families are like


<details>
  <summary> Solution </summary>

</details>


Q.145 If the median of the data 30,8,7,3,17,15,21,24,29,23 is x and the median of the data
obtained by replacing 3 by 33 and 8 by 18 in the above data is y, then what is the
difference between y and x ?
- [ ] A. 2
- [ ] B. 3
- [ ] C. 4
- [ ] D. 1

<details>
  <summary> Solution </summary>

</details>


Q.146 Choose the correct option instead of the question mark in the given question.
456 : 15 :: 627 : ?
- [ ] A. 12
- [ ] B. 15
- [ ] C. 18
- [ ] D. 21

<details>
  <summary> Solution </summary>

</details>


Q.147 In English alphabet which Letter is in between the Letter S and the Letter G ?
- [ ] A. N
- [ ] B. M
- [ ] C. L
- [ ] D. P
 
<details>
  <summary> Solution </summary>

</details>


Q.148 Which of the following are macronutrients commonly found in soil?
- [ ] A. Carbon, Hydrogen, Oxygen
- [ ] B. Nitrogen, Phosphorus, Potassium
- [ ] C. Iron, Manganese, Zinc
- [ ] D. Boron, Copper, Molybdenum

<details>
  <summary> Solution </summary>

</details>



Q.149 ABCD is a rhombus in which ∠ADB = 25 Degree. Then, the value of ( 2∠BAD - ∠ABC ) is:
- [ ] A. 230 Degree
- [ ] B. 240 Degree
- [ ] C. 210 Degree
- [ ] D. 260 Degree

<details>
  <summary> Solution </summary>

</details>


Q.150 Globalization signifies which of the following :
- [ ] A. Time-space compression
- [ ] B. The integration of the world economy
- [ ] C. The growth of supra- territorial relations between people
- [x] D. All the above

<details>
  <summary> Solution </summary>

</details>



</details>
<!----------------------------------------->
