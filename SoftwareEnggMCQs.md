
## Software Engineering

Q 1. Which software life cycle model is based on **iterative protyping**?
- [ ] A. Waterfall Model
- [x] B. Spiral Model
- [ ] C. Agile Model
- [ ] D. Prototype Model

<details>
  <summary> Spiral Model </summary>

<br/>

The **Spiral Model** combines iterative development with repeated prototyping and risk analysis. <br/>
The software is developed through multiple cycles, or spirals, with each cycle refining the product.

**How spiral Model works?**

<img width="681" height="432" alt="image" src="https://github.com/user-attachments/assets/e846640c-eb8c-46f9-ba76-84f3510fedf5" />

> **Spiral Model -> iterative cycles + risk analysis.**

> **Prototyping Model -> builds and refines prototypes based on feedback.**

> **Waterfall Model -> sequential phases.**

  
</details>
<!--------------------->

---

Q 2. In the context of software project management, what is LOC an acronym for?
- [ ] A. Line of Change
- [ ] B. Level of Complexity
- [x] C. Lines of Code
- [ ] D. List of Components

<details>
  <summary> LOC = Lines of Code </summary>

<br/>

In software project management, LOC (Lines of Code) is a metric used to measure the size of a software program by 
counting its source-code lines.

**Why is LOC useful?**
- **Size estimation**: Estimates software size.
- **Effort estimation**: Helps estimate development effort.
- **Productivity measurement**: Can be used to calculate LOC produced per developer or unit of time.
- **Maintenance**: Helps assess the size of a codebase.

> **LOC = Lines of Code; <br/>
> KLOC = Thousand Lines of Code. <br/>
> FP = Function Points**
  
</details>
<!--------------------->

---

Q 3. The cost estimation technique that involves experts judgements and consensus is called:
- [ ] A. COCOMO
- [x] B. Delphi Method
- [ ] C. Waterfall Model
- [ ] D. Prototype Model

<details>
  <summary> <b> Delphi Technique (Delphi Method) </b> </summary>

<br/>

> **Experts + repeated rounds + consensus = Delphi Technique**

Panels of experts(jugdes) sit for evaluating everything is Delphi Method.

The **Delphi Technique** is a software cost-estimation method that gathers judgments from a panel of experts through multiple 
rounds of consultation until a consensus or reasonable agreement is reached.

**How it works**:
- 1. Experts independently estimate the project cost or effort.
- 2. Their estimates are collected and summarized.
- 3. Experts review the anonymous feedback and revise their estimates.
- 4. Rounds continue until estimates converge sufficiently.
  
</details>
<!--------------------->

Which technique primarily **relies on comparing a new project with similar completed projects**?
- [ ] A. Delphi Technique
- [x] B. Estimation by analogy
- [ ] C. COCOMO
- [ ] D. Function Point Analysis

**Delphi Technique** - Uses expert opinions and repeated rounds of feedback to reach consensus.

**Estimation by Analogy** - Estimates cost or effort by comparing the new project with similar completed projects.

**COCOMO** - Uses a mathematical model to estimate software development effort, based largely on project size.

**Function Point Analysis** - Estimates software size based on functionality, such as inputs, outputs, and queries.

---

Q 4. Which type of maintenance involves **adding new features to existing software**?
- [ ] A. Corrective Maintenance
- [x] B. Perfective Maintenance
- [ ] C. Adaptive Maintenance
- [ ] D. Preventive Maintenance

<details>
  <summary> <b> Types of software maintenance </b> </summary>

<br/>

| Type	          | Purpose	                                | Example                                      |
| **Corrective**	| **Fix errors or bugs**	                | Fixing a login failure                       |
| **Adaptive**	  | **Adjust to a changed environment**	    | Updating software for a new operating system, obselete features |
| **Perfective**	| **Add features or improve performance**	| Adding a search feature                      |
| **Preventive**	| **Reduce future maintenance problems**	| Refactoring code to improve maintainability, Future  |
  
</details>
<!--------------------->

---

Q 5. The framework that provides **guidelines for achieving consistent and high-quality software** is:
- [ ] A. COCOMO
- [x] B. ISO 9000
- [ ] C. Delphi Method
- [ ] D. Agile Manifesto

<details>
  <summary> <b> Software Quality Assurance (SQA) framework : ISO 9000 </b> </summary>

<br/>

SQA provides processes, standards, and guidelines to help ensure software is developed consistently and meets defined quality 
requirements

ISO 9001, a quality-management standard, or ISO/IEC 25010, a software product-quality model.

- **ISO 9001**: Quality Management System, Specifies requirements for a Quality Management System (QMS), helping organizations
   consistently deliver products and services that meet requirements.

- **ISO/IEC 25010**:  Software product-quality model

- **IEEE 754**: Defines standards for floating-point arithmetic in computing.

- **HTML5**: Defines technologies for structuring and presenting web content.

- **TCP/IP**: A suite of networking protocols used for communication between devices.
  
</details>
<!--------------------->

---

Q 6. Which software life cycle model allows for **iterative development and incorporate risk analysis**?
- [ ] A. Waterfall Model
- [ ] B. Prototype Model
- [x] C. Spiral Model
- [ ] D. Agile Model

<details>
  <summary> Spiral Model </summary>

<br/>
  
</details>
<!--------------------->

---

Q 7. What is the main goal of **software quality assurance(SAQ)**?
- [ ] A. To eliminate all defects from the software
- [ ] B. To ensure the softwareis defect-free before release
- [x] C. To establish and enforce standards and processes to improve software quality
- [ ] D. To test software under different conditions

<details>
  <summary> <b> Software Quality Assurance(SAQ) </b> </summary>

<br/>

The main goal of **Software Quality Assurance (SQA)** is ***to ensure that software development processes follow established 
standards and procedures so that the resulting software meets specified quality requirements***.

- Focus: Prevent defects by improving and monitoring development processes.
- Goal: Ensure consistent software quality and compliance with standards.
- Activities: Process audits, standards enforcement, reviews, and quality monitoring.


> **Software Quality Assurance (SQA)** -> Focuses on processes and preventing defects.

> **Software Quality Control (SQC)** -> Focuses on checking the product to identify defects.

**SQA = Process-oriented and defect prevention; SQC = Product-oriented and defect detection.**
  
</details>
<!--------------------->

---

Q 8. **Reverse Engineering** is primarily used for:
- [ ] A. creating new software from scratch
- [ ] B. improving software performance
- [x] C. understanding and documenting existing software
- [ ] D. testing software components

<details>
  <summary> <b> Reverse Engineering </b> </summary>

<br/>

Reverse Engineering is the process of analyzing existing software to understand its internal structure, design, components, 
and functionality, usually without having the original design documents.

Example: <br/>
Suppose you have an old software application but no source-code documentation. <br/>
You analyze its code and behavior to understand how it works and create design documents.

**Why is reverse engineering used?**
- Understanding legacy software.
- Recovering missing design documentation.
- Analyzing software components and dependencies.
- Supporting software maintenance and modernization.

### Reverse engineering vs. forward engineering

| Reverse engineering	                        | Forward engineering         |
|---------------------------------------------|-----------------------------|
| Existing software -> design or understanding| Design -> implementation    |
| Analyzes what already exists	              | Builds or develops a system | 
| Often used for legacy systems	              | Used in new development     |

> **Reverse engineering means moving from an existing implementation toward understanding its design. <br/>
> It does not necessarily mean modifying or rebuilding the software.**
  
</details>
<!--------------------->

---

Q 9. Which testing approach involves testing individual components or units of code?
- [ ] A. Intergration testing
- [ ] B. System testing
- [x] C. Unit testing
- [ ] D. Acceptance testing

<details>
  <summary> Types of Testing </summary>

<br/>

| Testing type	      | Main focus                                               |
|---------------------|----------------------------------------------------------|
| Unit testing	      | Individual functions or components                       |
| Integration testing	| Interactions between components                          |
| System testing	    | The complete integrated system                           |
| Acceptance testing	| Whether the software meets user or business requirements |
  
</details>
<!--------------------->

---

Q 10. What is the main goal of **System Testing**?
- [ ] A. Testing individual components in isolation
- [ ] B. Testing the integration between different software components
- [x] C. Testing the software functionality from the user's perspective
- [ ] D. Identifying defects in the source code

<details>
  <summary> </summary>

<br/>

The main goal of System Testing is to test the complete, integrated software system against its specified requirements.

Testing individual components in isolation -  This is unit testing.

Testing integration between different software components - This is integration testing.

Identifying defects in the source code - This is more closely associated with code inspection, static analysis, and debugging.

  
</details>
<!--------------------->

---

Q 11. Which metric is used for estimating the size of a software project?
- [ ] A. Cyclomatic Complexity
- [x] B. Function Points(FP)
- [ ] C. Defect Density
- [ ] D. Software Reliability Index

<details>
  <summary> Lines of Code + Functions used </summary>

<br/>

A common metric used to estimate the size of a software project is **LOC (Lines of Code)**.

However, **Function Points (FP)** is also a standard software-size metric, measuring the functionality delivered to users 
rather than the number of code lines.

**Common software size metrics**

| Metric	              | What it measures                                    |
|-----------------------|-----------------------------------------------------|
| LOC	                  | Number of lines of source code                      |
| KLOC	                | Thousands of lines of code                          |
| Function Points (FP)	| Software functionality from the user's perspective  |
| Use Case Points (UCP)	| Size estimated from use cases and system complexity |

- **LOC (Lines of Code)**: Measures software size by counting source-code lines.
- **KLOC (Thousand Lines of Code)**: Measures size in thousands of lines of code.
- **Function Points (FP)**: Estimates software size based on functionality delivered to users, such as inputs, outputs,
  inquiries, files, and interfaces.

- **Defect Density**: Measures the number of defects relative to software size; it is a quality metric, not a size-estimation
  technique by itself.
  
</details>
<!--------------------->

---

Q 12. What is the purpose of staffing level estimation in software project management?
- [ ] A. to determine the number of hardware components required
- [ ] B. to identify potential risks in the project
- [x] C. to allocate appropriate resources to the project
- [ ] D. to estimate the maintenance costs of the software

<details>
  <summary> staffing in software project management </summary>

<br/>

The purpose of staffing level estimation in software project management is to determine how many people are needed to work 
on a project and when they are needed during its development.

**Why is it important?**
- **Resource planning**: Determines the number of developers, testers, and other team members required.
- **Scheduling**: Identifies when staff should join or leave the project.
- **Budgeting**: Helps estimate personnel costs.
- **Workload management**: Helps distribute work effectively and avoid overstaffing or understaffing.

Example: <br/>
A project may need 2 developers initially, <br/>
5 during intensive development, and <br/>
3 testers during the testing phase.

- Effort estimation -> How much work?
- Staffing estimation -> How many people, and when?
- Cost estimation -> How much money?
- Schedule estimation -> How much time?
  
</details>
<!--------------------->

---

Q 13. What is the primary purpose of **Software Requirement Specification(SRS) documents**?
- [ ] A. to list the programming languages used
- [ ] B. to describe the user interface design
- [x] C. to define the software's functional and non-functional requirements
- [ ] D. to specify the hardware components required

<details>
  <summary> Software Requirements Specification (SRS) document </summary>

<br/>

The primary purpose of a **Software Requirements Specification (SRS) document** is **to clearly define and document the 
functional and non-functional requirements of a software system**.

**What does an SRS contain?**

- **Functional requirements**: What the software must do. Example: users can log in using a username and password.

- **Non-functional requirements**: How well the software must perform. Example: the login page should load within two seconds.

- **Constraints**: Limitations or rules the system must follow.

**Why is an SRS important?** <br/>
It serves as an agreement and reference for customers, developers, testers, and project managers. <br/>
It guides design, development, testing, and validation.


> **SRS = What the software must do and the conditions it must satisfy.**

  
</details>
<!--------------------->

---

Q 14. **ISO 9000 and SEI CMM** both frameworks are related to:
- [ ] A. Network Protocols
- [ ] B. Software Architecture
- [x] C. Software Quality Standards and Process Improvement
- [ ] D. Software Development Language

<details>
  <summary> <b> ISO 9000 and SEI CMM </b> </summary>

<br/>

**ISO 9000** and **SEI CMM** are two important frameworks used in software engineering to improve and assess the quality of 
software development processes.

### 1. ISO 9000

ISO 9000 is a family of international standards related to **quality management systems (QMS)**.
- Purpose: Establish a systematic approach to quality management.
- Focus: Documented processes, consistency, customer satisfaction, and continual improvement.
- Application: Used across many industries, including software development.
- Important fact: ISO 9001 specifies requirements for a quality management system and is the standard used for certification.


### 2. SEI CMM

**SEI CMM stands for Software Engineering Institute Capability Maturity Model**.
- Purpose: Assess and improve the maturity of an organization's software development processes.
- Focus: Process maturity and continuous improvement.
- Application: Helps organizations develop more predictable and disciplined software processes.

<img width="650" height="625" alt="image" src="https://github.com/user-attachments/assets/6ed8cb75-ce9d-432b-b549-35401adf5eab" />

###  ISO 9000 family	vs SEI CMM

| ISO 9000 family	                            | SEI CMM                                              |
|---------------------------------------------|------------------------------------------------------|
| Quality management standards	              | Software process maturity model                      |
| Emphasizes quality-management requirements	| Emphasizes process maturity and improvement          |
| ISO 9001 can be used for certification	    | Traditional CMM assesses maturity across five levels |
| Applies across industries	                  | Original CMM focused on software engineering         |


ISO 9001 - Specifies requirements for a Quality Management System.

SEI CMM - The traditional Capability Maturity Model assesses software-process maturity using five levels, from Initial 
to Optimizing.

IEEE 754 - Defines standards for floating-point arithmetic.

ISO/IEC 25010 - Defines a model for evaluating software and system product quality.
  
</details>
<!--------------------->

---

Q 15. Software design approach involves:
- [ ] A. Hardware integration
- [ ] B. User training techniques
- [ ] C. Creating plan for coding
- [x] D. Defining the structure and organization of software components

<details>
  <summary> Software design approach </summary>

<br/>

Software design approach involves converting software requirements into a blueprint for implementation.

The two major software design approaches are:
1. **Top-down approach**: Start with the whole system and break it into smaller modules.
2. **Bottom-up approach**: Start by designing small, reusable components and combine them into a complete system.

| Approach	      | Key idea                    |
|-----------------|-----------------------------|
| Top-down	      | Large -> Small              |
| Bottom-up	      | Small -> Large              |
| Object-oriented	| Objects and classes         |
| Prototype	      | Build, get feedback, refine |
  
</details>
<!--------------------->

---

Q 16. Which document provides a comprehensive description of software requirements?
- [ ] A. Source Code
- [x] B. Software Specification Document
- [ ] C. User Manula
- [ ] D. Test Plan

<details>
  <summary> Software Specification Document </summary>

<br/>
  
</details>
<!--------------------->

---

Q 17. Which model considers risk assessment and incremental development in software projects?
- [ ] A. Waterfall Model
- [ ] B. Agile Model
- [ ] C. Prototype Model
- [x] D. Spiral Model

<details>
  <summary> Spiral Model </summary>

<br/>

The Spiral Model is a software development life-cycle (SDLC) model **that combines iterative development, prototyping, 
and risk analysis**.

Development proceeds through repeated cycles called spirals.

<img width="1022" height="717" alt="image" src="https://github.com/user-attachments/assets/8a66ca74-bfd4-4e0c-9448-16ca6ac3d434" />


### Four phases of the Spiral Model

1. **Planning**: Identify objectives, requirements, alternatives, and constraints.
2. **Risk analysis**: Identify potential risks and evaluate ways to reduce them. Prototypes may be built to investigate risks.
3. **Engineering**: Design, develop, and test the next version of the software.
4. **Evaluation**: The customer evaluates the result, provides feedback, and helps plan the next cycle.
These activities repeat in successive spirals until the software is completed.

### Advantages
- Strong emphasis on risk management.
- Supports changing requirements.
- Customer feedback is incorporated in each cycle.
- Suitable for large, complex, high-risk projects.

### Disadvantages
- Can be expensive and time-consuming.
- Requires expertise in risk assessment.
- May be unsuitable for small, low-risk projects.


| Model	          | Key identifying feature                  |
|-----------------|------------------------------------------|
| **Waterfall**	  | Sequential phases                        |
| **Prototyping**	| Early model for feedback                 |
| **Spiral**	    | Iterative development with risk analysis |
| **Incremental**	| Software delivered in increments         |
| **Agile**	      | Short iterations and frequent feedback   |
  
</details>
<!--------------------->

---

Q 18. The Waterfall, Prototype, and Spiral are the example of:
- [ ] A. Software development languages
- [ ] B. Software metrics
- [x] C. Software life cycle models
- [ ] D. Software quality standards

<details>
  <summary> Software life cycle models </summary>

<br/>
  
</details>
<!--------------------->

---

Q 19. Which metric is used to measure software reliability?
- [ ] A. Functional Points(FP)
- [ ] B. Lines of Code(LOC)
- [x] C. Musa's Basic Model
- [ ] D. Cyclomatic Complexity

<details>
  <summary> <b> Musa's Basic Model - Software Reliability growth and execution time </b> </summary>

<br/>

**Musa's Basic Execution Time Model** is a software reliability growth model used **to estimate how software reliability**
improves as faults are detected and removed during testing.

It is associated with **John D. Musa**.

**Key concept** <br/>
As software is executed and defects are discovered and corrected, the number of remaining faults generally decreases, 
so the software’s failure intensity tends to decline.
- **Execution time**: Time the software is actually running, rather than calendar time.
- **Failure intensity**: Expected number of failures per unit of execution time.
- **Reliability growth**: Reliability improves as faults are removed.

> **Musa -> Software reliability growth and execution time.**

| Model	       | Main purpose                |
|--------------|-----------------------------|
| **Musa**	   | Software reliability growth |
| **COCOMO**	 | Cost and effort estimation  |
| **SEI CMM**	 | Process maturity            |
| **ER model** | Database relationships      |
  
</details>
<!--------------------->

---

Q 20. Which testing method is primarily concerned with testing the software's functionality?
- [x] A. Black Box Testing
- [ ] B. White Box Testing
- [ ] C. Grey Box Testing
- [ ] D. Regression Testing

<details>
  <summary> Black Box Testing </summary>

<br/>

### Black Box Testing 
- Tests the software's functionality without examining its internal source code.
- Checks inputs against expected outputs and requirements.
- Example: Enter valid and invalid login credentials and check the results.

###  White Box Testing
- Examines internal code, logic, branches, and execution paths.
- Requires knowledge of the program's internal structure.

### Grey Box Testing 
- Combines aspects of black-box and white-box testing.
- The tester has partial knowledge of the internal system.

### Regression Testing 
- Checks whether previously working functionality still works after code changes, bug fixes, or updates.
- It can include functional tests, but its defining purpose is to detect unintended effects of changes.


| Testing method | Key purpose                            |
|----------------|----------------------------------------|
| **Black box**	 | Test functionality without seeing code |
| **White box**	 | Test internal code and logic           |
| **Grey box**	 | Test with partial internal knowledge   |
| **Regression** | Check existing features after changes  |
  
</details>
<!--------------------->

---

Q 21. **Halstead Software science** is concerned with:
- [ ] A. Project Scheduling
- [x] B. Software metric based on code attributes
- [ ] C. User interface design
- [ ] D. Quality Assurance Processes

<details>
  <summary> Halstead Software Science - Measuring software complexity using operators and operands.</summary>

<br/>

**Halstead Software Science - Measuring software complexity using operators and operands**

Halstead Software Science is a software metric approach developed by Maurice Halstead to estimate program characteristics
using counts of operators and operands in source code.

**Four basic measures**

| Symbol | Meaning                       |
|--------|-------------------------------|
| `n1`	 | Number of distinct operators  |
| `n2`	 | Number of distinct operands   |
| `N1`	 | Total occurrences of operators|
| `N2`	 | Total occurrences of operands |

These are used to calculate measures such as program vocabulary, program length, volume, difficulty, and estimated effort.

Formula 1: `n = n1 + n2`, where `n` denotes total number of operands and operators

Formula 2: `N = N1 + N2`, where `N` denotes total used number of operands and operators

Formula 3: `Volume = N log2 n`

> **Halstead = Operators + Operands -> Software metrics and complexity.**
  
</details>
<!--------------------->

---

Q 22. **Putnam's Model** is used for estimating:
- [ ] A. Software size
- [x] B. Software development time
- [ ] C. Software Complexity
- [ ] D. Software testing effors

<details>
  <summary> Putnam's Model: Software development effort, cost, and schedule estimation. </summary>

<br/>

Putnam’s Model is a software cost-estimation model used to estimate the effort and time required to develop a software project.

It is associated with the **SLIM (Software Life-Cycle Management) model** and the **Rayleigh manpower distribution**.

**Key concepts**
- **Effort**: Total human work required, often measured in person-months.
- **Schedule**: Time required to complete the project.
- **Staffing**: How the number of people assigned to the project changes over time.

Putnam’s model highlights **the relationship between software size, development effort, and delivery time**.

| Model	       | Main purpose                   |
|--------------|--------------------------------|
| **Putnam**	 | Effort and schedule estimation |
| **COCOMO**	 | Cost and effort estimation     |
| **Musa**	   | Software reliability growth    |
| **SEI CMM**	 | Process maturity               |
| **Halstead** | Code complexity metrics        |

| Model	        |  Remember                          |
|---------------|------------------------------------|
| **Putnam**	  | Rayleigh staffing curve            |
| **Halstead**	| Operators and operands             |
| **SEI CMM**	  | Process maturity                   |
| **Musa**	    | Reliability and failure intensity  |
  
</details>
<!--------------------->

---

Q 23. **Reverse Engineering** in software referes to:
- [ ] A. Developing Software without any planning
- [x] B. Analysing and understanding existing software
- [ ] C. Creating new software based on requirements
- [ ] D. Testing software components for defects

<details>
  <summary> Analysing and understanding existing software </summary>

<br/>

> **Reverse engineering = Existing software to design/understanding.**

Reverse Engineering refers to analyzing existing software to understand its components, structure, design, and functionality, often recovering higher-level design information from source code or an existing system.

Example: <br/>
Suppose a company has an old software application but has lost its original design documents. <br/>
Engineers examine the source code and database structure to reconstruct how the application works and document its design. <br/>
This is reverse engineering.

**Reverse engineering vs. forward engineering**

| Reverse engineering	                       | Forward engineering                    |
|--------------------------------------------|----------------------------------------|
| Existing system -> Design or understanding |	Requirements/design -> Implementation |
| Understand how software works	             | Build the software                     |

> **Re-engineering involves examining and modifying or transforming an existing system to improve or modernize it.**
  
</details>
<!--------------------->

---

Q 24. Which **maintenance process model** focuses on _fixing defects_ as they are identified?
- [ ] A. Waterfall Model
- [x] B. Corrective Maintenance
- [ ] C. Perfective Maintenance
- [ ] D. Adaptive Maintenance

<details>
  <summary> Corrective Maintenance </summary>

<br/>

**Corrective Maintenance**
- Fixes defects discovered during software operation.
- Example: Fixing a calculation bug in a school fee-management application.
> **Corrective = Correct errors**


**Perfective Maintenance**
- Improves performance, usability, or existing features.
- Example: Adding a report-export feature or making a slow report faster.

**Adaptive Maintenance**
- Modifies software to work in a changed environment.
- Example: Updating an application to support a new operating system or database version.

**Waterfall Model**
- A sequential software development life-cycle model.
- Its phases typically proceed from requirements to design, implementation, testing, and maintenance.
- It is not a type of software maintenance.


| Maintenance type|	Purpose	                        | Example               |
|-----------------|---------------------------------|-----------------------|
| **Corrective**	| Fix defects	                    | Fix a calculation bug |
| **Perfective**	| Improve features or performance	| Add a useful report   |
| **Adaptive**	  | Adjust to environmental changes	| Support a new OS      |
| **Preventive**	| Reduce future problems 	        | Refactor fragile code |

> - Corrective = bug fixing;
> - Perfective = improvement;
> - Adaptive = environment change;
> - Preventive = future-risk reduction.
  
</details>
<!--------------------->

---

Q 25. **Program Analysis Tools** are used for:
- [ ] A. Designing Software Architecture
- [ ] B. Measuring Siftware Reliability
- [ ] C. Automatically generating test cases
- [x] D. Analysing code for errors and performance bottlenecks

<details>
  <summary> <b>Program Analysis Tools</b> </summary>

<br/>

**Program analysis** tools are tools used to examine source code or a running program to understand its behavior, detect defects, and assess code quality.

There are two important categories:

**1. Static analysis tools** <br/>
Analyze source code without executing the program.

Examples:
- Detect unused variables and unreachable code.
- Identify possible security vulnerabilities.
- Find coding-standard violations and potential bugs.

Examples of tools: `SonarQube`, `ESLint`, and `static-analysis` features in compilers.

**2. Dynamic analysis tools** <br/>
Analyze a program while it is executing.

Examples:
- Detect memory leaks and invalid memory access.
- Measure runtime performance.
- Observe program behavior using test inputs.

Examples of tools: `Valgrind` and `runtime profilers`.


**Other useful program analysis tools**

| Tool	                  | Purpose                                               |
|-------------------------|-------------------------------------------------------|
| **Debugger**  	        | Finds and investigates program errors                 |
| **Profiler**          	| Measures execution time and resource usage            |
| **Code coverage tool**	| Measures which code is executed during tests          |
| **Compiler**	          | Translates code and may report syntax or other errors |

> - Static analysis -> No execution.
> - Dynamic analysis -> Program runs.
> - Debugger -> Investigates errors.
> - Profiler -> Measures performance.

> **Static = Source code without execution. <br/>
> Dynamic = Program executing.**
  
</details>
<!--------------------->

---

Q 26. What is the purpose of **estimating staffing levels in software project management**?
- [ ] A. to determine the number of required hardware components
- [ ] B. to identify potential risks in the project
- [x] C. to allocate appropriate resources for the project
- [ ] D. to estimate the software maintenance cost

<details>
  <summary> Staffing Levels in Software Project Management </summary>

<br/>

### Purpose of Estimating Staffing Levels in Software Project Management

The primary purpose is to determine the number of people required for a software project and when they will be needed throughout its life cycle.

Staffing-level estimation helps a project manager:
- Determine how many developers, testers, and other specialists are needed.
- Plan when team members should join or leave the project.
- Allocate human resources to different project phases.
- Avoid understaffing or unnecessary staffing costs.

Example: A project may need 2 analysts during requirements gathering, 6 developers during implementation, and 3 testers during testing.

Important points
- Staffing estimation -> Number of people and their timing.
- Effort estimation -> Amount of work, usually in person-hours or person-months.
- Cost estimation -> Money required.
- Schedule estimation -> Time needed to complete the project.

> **Effort = person-months; Schedule = calendar duration. They are related, but they are not interchangeable.**
  
</details>
<!--------------------->

---

Q 27. **Software Engineering** emerged due to:
- [ ] A. the decline of computer technology
- [ ] B. the need for complex hardware systems
- [x] C. the challenges posed by software development
- [ ] D. the focus on hardware-only solutions

<details>
  <summary> <b> Software Engineering </b> </summary>

### Software Engineering emerged due to the Software Crisis.

The term software crisis describes the difficulties experienced as software systems became larger and more complex, including cost overruns, missed deadlines, unreliable software, and challenges in maintenance.

The term Software Engineering gained prominence at the 1968 NATO conference, where systematic engineering approaches to software development were discussed.

Main causes of the Software Crisis
- Increasing software complexity.
- Projects exceeding budgets and deadlines.
- Unreliable software with frequent defects.
- Difficulty maintaining and modifying software.
- Lack of systematic development methods.
  
</details>
<!--------------------->

---

Q 28. **Musa's Basic Model** is used for measuring:
- [ ] A. Software Complexity
- [x] B. Software Reliability
- [ ] C. Software Performance
- [ ] D. Software Size

<details>
  <summary> Musa's Basic Model -  Software Reliability and reliability growth</summary>

<br/>

**Musa's Basic Execution Time Model** is used to estimate software reliability by analyzing failures observed during software execution and predicting how failure intensity changes as testing continues.

- **Software reliability**: The probability that software operates without failure for a specified time under specified conditions.
- **Failure intensity**: The expected number of failures per unit of execution time.
- **Reliability growth**: Reliability generally improves as defects are identified and corrected.

| Model	                        | What it measures or estimates                    |
|-------------------------------|--------------------------------------------------|
| **Musa's Basic Model**	      | Software reliability and failure intensity       |
| **Halstead Software Science**	| Software complexity using operators and operands |
| **Putnam Model**  	          | Software effort and schedule                     |
| **COCOMO**	                  | Software development effort and cost             |
| **SEI CMM**	                  | Software process maturity                        |

  
</details>
<!--------------------->

---

Q 29. **Delphi and COCOMO** are technique used for estimating:
- [ ] A. Software size
- [ ] B. Software reliability
- [ ] C. Software complexity
- [x] D. Software development cost

<details>
  <summary> Software development cost </summary>

<br/>

| Technique/model	| Key idea                                            |
|-----------------|-----------------------------------------------------|
| **Delphi**	    | Expert judgment and consensus                       |
| **COCOMO**	    | Mathematical model using project size and factors   |
| **Putnam**	    | Effort and schedule; Rayleigh staffing distribution |
| **Musa**	      | Software reliability growth                         |
| **Halstead**	  | Operators, operands, and software complexity        |

**Software size**
- Software size is measured using metrics such as LOC (Lines of Code), KLOC (thousand lines of code), or Function Points. Size can be an input to COCOMO, but estimating size is not the main purpose of both techniques.

**Software reliability**
- Reliability models such as Musa’s Basic Execution Time Model are used to predict software reliability and failure intensity.

**Software complexity**
- Halstead Software Science estimates program characteristics and complexity using operators and operands.

**Software development cost**
- Delphi: Uses expert judgment and repeated feedback to develop estimates.
- COCOMO: Uses a mathematical model, including software size and project factors, to estimate effort and schedule, which can then help estimate cost.

> **COCOMO directly estimates effort and schedule; cost can be derived from effort and the applicable rates.** <br/>
> **Delphi can estimate cost as well as other project quantities.**
  
</details>
<!--------------------->

---

Q 30. The model used **for estimating software maintenance cost** is called:
- [ ] A. COCOMO
- [ ] B. Putnam's Model
- [ ] C. Musa's Basic Model
- [x] D. Boehm's Model

<details>
  <summary> <b> Boehm's Model </b> </summary>

<br/>

**Boehm's software maintenance cost model** is used to estimate the effort and cost involved in maintaining existing software. 

It considers factors such as the amount of software that needs to be changed and the effort required for those changes.

| Model	  | Remember                               |
|---------|----------------------------------------|
| COCOMO	| Development effort and cost by Lines of code, Functions Provided |
| Delphi	| Development effort and cost by experts |
| Putnam	| Effort, schedule, Rayleigh staffing    |
| Musa	  | Software reliability                   |
| Boehm	  | Software maintenance cost              |
  
</details>
<!--------------------->

---

Q 31. Which maintenance activity **involves updating software to work with new hardware or software environment**?
- [ ] A. Corrective Maintenance
- [x] B. Adaptive Maintenance
- [ ] C. Perfective Maintenance
- [ ] D. Preventive Maintenance

<details>
  <summary> The 4 types of maintenance activity </summary>

<br/>

The four types of software maintenance:
| Type	          | Key phrase                 |
|-----------------|----------------------------|
| **Corrective**	| Fix bugs                   |
| **Adaptive**	  | Adapt to a new environment |
| **Perfective**	| Improve or enhance         |
| **Preventive**	| Prevent future problems    |

1. **Corrective Maintenance**: Fixes defects or bugs discovered after software delivery.

2. **Adaptive Maintenance**: Modifies software so it continues to work in a changed environment, such as a new operating system, database, or hardware platform.

3. **Perfective Maintenance**: Improves performance, usability, or existing features, or adds enhancements based on user needs.

4. **Preventive Maintenance**: Makes changes to reduce the likelihood of future problems and improve maintainability.


> - Bug found -> Corrective
> - Environment changed -> Adaptive
> - Feature improved -> Perfective
> - Future problem prevented -> Preventive
  
</details>
<!--------------------->

---

Q 32. What does the term **Software Maintenance** refers to:
- [ ] A. Developing new software applications
- [ ] B. Enhacing software performance
- [ ] C. Managing hardware components
- [x] D. Modifying and updating existing software

<details>
  <summary> <b> Modifying and updating existing software is: Software Maintenance </b> </summary>

<br/>

> **Software Maintenance = Changes made to software after delivery.**

  
</details>
<!--------------------->

---

Q 33. Which version control system is commonly used for collaborative web development projects?
- [ ] A. SVN
- [x] B. Git
- [ ] C. Mercurial
- [ ] D. CVS

<details>
  <summary> Git </summary>

<br/>

**Git** is the most commonly used version control system for collaborative web development projects.

**`Git`**: A distributed version control system that allows developers to work independently, track changes, create branches, and merge code. 
- Platforms such as `GitHub` and `GitLab` support **Git-based collaboration**.

**`SVN` (Subversion)**: A centralized version control system that stores a repository on a central server.

**`CVS` (Concurrent Versions System)**: An older centralized version control system.

**`Mercurial`**: Also a distributed version control system, but less commonly used than `Git` today.

> - `Git` -> Distributed + GitHub/GitLab
> - `SVN` / `CVS` -> Centralized
> - `Mercurial` -> Distributed


Note: **Git is the version control system;** <br/>
**GitHub is a platform that hosts Git repositories and supports collaboration.**

Which Git command creates a copy of a remote repository on your local computer?
- [ ] A. git push
- [x] B. git clone
- [ ] C. git merge
- [ ] D. git commit

| Git command	  | Purpose                            |
|---------------|------------------------------------|
| `git clone`	  | Copy a repository                  |
| `git pull`	  | Fetch and integrate remote changes |
| `git add`	    | Stage changes                      |
| `git commit`	| Save a snapshot locally            |
| `git push`	  | Upload commits                     |
  
</details>
<!--------------------->

---

Q 34. The term **DFD** stands for:
- [ ] A. Data File Diagram
- [ ] B. Data Flow Document
- [x] C. **Data Flow Diagram**
- [ ] D. None of the above

<details>
  <summary> DFD = Data Flow Diagram </summary>

<br/>

A **Data Flow Diagram (DFD)** is a graphical representation of how data moves through a system, showing where data comes from, how it is processed, where it is stored, and where it goes.

**Main components of a DFD**

1. **External Entity**
- A source or destination of data, such as a customer.

2. **Process**
- Transforms input data into output, such as processing an order.

3. **Data Store**
- Stores data, such as a database or file.

4. **Data Flow**
- Shows the movement of data between components, usually with arrows.

<img width="765" height="492" alt="image" src="https://github.com/user-attachments/assets/197a69cc-b99c-4325-bf9b-aa9a4fad7c03" />


> **DFD = Data Flow Diagram -> movement of data through a system.**

Do not confuse it with a **flowchart**, which primarily represents the sequence of steps or control logic in an algorithm or process.
  
</details>
<!--------------------->

---

Q 35. Which charateristics of software distinguishes it from most physical engineering products?
- [ ] A. Software wears out physically
- [ ] B. Software is manufactured repeatedly
- [x] C. Software is developed, not manufactured
- [ ] D. Software requires raw material

<details>
  <summary> Software is developed, not manufactured </summary>

<br/>
  
</details>
<!--------------------->

---

Q 36. The **emergence of Software Engineering as a discipline** was primarily a response to:
- [ ] A. Hardware  miniaturization
- [x] B. the software crisis
- [ ] C. Database expansion
- [ ] D. Network standardization

<details>
  <summary> software crisis </summary>

<br/>

The emergence of Software Engineering as a discipline was primarily due to the Software Crisis of the late 1960s.

**Why did the Software Crisis occur?**
- Software systems became increasingly large and complex.
- Projects frequently exceeded budgets and deadlines.
- Software often contained defects and was difficult to maintain.
- Informal programming methods were insufficient for managing large projects.

The term **Software Engineering** gained prominence at the 1968 NATO Conference, where systematic engineering approaches to software development were discussed.

> **Software Engineering emerged to address the Software Crisis**.
  
</details>
<!--------------------->

---

Q 37. Which metric is most directly associated with software product size?
- [x] A. Lines of code(LOC)
- [ ] B. Defective removal time
- [ ] C. Team productivity
- [ ] D. Project Duration

<details>
  <summary> Lines of code(LOC/KLOC) + Function Points(FP) </summary>

<br/>

The metric most directly associated with software product size is LOC (Lines of Code).
- LOC/KLOC: Measures the number of source-code lines (KLOC = 1,000 lines of code).
- Function Points (FP): Measures software size based on functionality delivered to users.

> **Lines of Code(LOC) measures code size; <br/>
> while Function Points(FP) measure functional size.**
  
</details>
<!--------------------->

---

Q 38. Which of the following is a **process metric** rather than a product metric?
- [ ] A. Cyclomatic Complexity
- [ ] B. Code Size
- [ ] C. Defect Density
- [x] D. **Review Efficiency**

> **Product metrics = characteristics of the software.**

> **Process metrics = effectiveness of activities used to develop the software.**

<details>
  <summary> Product metrics vs Process metrics </summary>

<br/>

A **process metric** measures how effectively software development activities are performed. <br/>
**Review efficiency** evaluates how effectively reviews identify defects.

- **Review Efficiency** - Process metric: Evaluates the effectiveness of the software review process in detecting defects.

- **Cyclomatic Complexity** - Product metric: Measures the number of linearly independent paths through a program’s control-flow graph.

- **Code Size** - Product metric: Measures software size, often using LOC or KLOC.

- **Defect Density** - Product metric: Measures defects relative to software size, such as defects per KLOC.
  
</details>
<!--------------------->

---

Q 39. In the **Waterfall Model**, a major limitation is that:
- [ ] A. It lacks defined phases
- [ ] B. It discourages documentation
- [x] C. Changes become costly
- [ ] D. It requires repeated risk analysis

<details>
  <summary> <b> Waterfall Model </b> </summary>

<br/>

The Waterfall Model is a traditional SDLC (Software Development Life Cycle) model in which software development proceeds through a sequence of phases.

Each phase is generally completed before the next phase begins.

> **Waterfall = Sequential development, phase by phase.**




### Phases of the Waterfall Model

1. Requirements Analysis
2. System Design
3. Implementation (Coding)
4. Testing
5. Deployment
6. Maintenance

<img width="577" height="340" alt="image" src="https://github.com/user-attachments/assets/356ea281-43aa-4b53-a622-a83047368c96" />

### Advantages
- Simple and easy to understand.
- Clear phases and documentation.
- Suitable when requirements are stable and well understood.

### Disadvantages
- Difficult and costly to accommodate changing requirements.
- Working software is generally available relatively late.
- Problems discovered late in testing can be expensive to fix.


> - **Waterfall** -> Sequential phases, stable requirements
> - **Agile** -> Iterative development, frequent feedback
> - **Spiral** -> Risk analysis in every cycle
> - **Prototyping** -> Early model for user feedback
  
</details>
<!--------------------->

---

Q 40. A prototype is developed mainlu to:
- [ ] A. Eliminates all testing
- [x] B. Clarify user requirements
- [ ] C. Replace maintenance
- [ ] D. Gurantee zero defects

<details>
  <summary> Clarify user requirements </summary>

<br/>
  
</details>
<!--------------------->

---

Q 41. Which features most clearly **distinguish the spiral model from the waterfall model**?
- [ ] A. Sequential phase
- [x] B. Risk-driven iteration
- [ ] C. No customer feedback
- [ ] D. Fixed requirement
 
<details>
  <summary> Spiral = Iteration + Risk Analysis </summary>

<br/>

**Sequential phase**: This is more characteristic of the Waterfall Model, where phases generally proceed in sequence.

**No customer feedback**: The Spiral Model can involve customer evaluation and feedback at the end of each cycle.

**Fixed requirement**: The Spiral Model can accommodate changing requirements as the project evolves.  

**Risk-driven iteration**: The Spiral Model develops software through repeated cycles, with risk analysis performed in each cycle.


<img width="1052" height="162" alt="image" src="https://github.com/user-attachments/assets/566f1459-5974-4a3f-8ccf-8de2488fc51b" />


<img width="1065" height="156" alt="image" src="https://github.com/user-attachments/assets/aeaa01ee-f60d-494f-a95e-b2d192dd35e6" />


> **Spiral = Iteration + Risk Analysis.**

**If mentioned risk-driven development, risk assessment in every cycle, or repeated development cycles, think of the Spiral Model.**

</details>
<!--------------------->

---

Q 42. Consider the following statements about software metrics:
1. Process metrics help evaluate development activities
2. Product metrics measures attributes of the software.
3. Funtion Points(FP) Analysis depends exclusively on source-code length

Which of the following are correct
- [x] A. 1 and 2 only
- [ ] B. 1 and 3 only
- [ ] C. 2 and 3 only
- [ ] D. 1, 2 and 3

<details>
  <summary> Process metrics, Product metrics and Function Points (FP) </summary>

<br/>

**1. Process metrics help evaluate development activities - True**

Process metrics measure the effectiveness of software development and maintenance activities, such as review efficiency, defect removal efficiency, and development cycle time.


**2. Product metrics measure attributes of the software - True**

Product metrics measure characteristics of the software itself, such as code size, cyclomatic complexity, performance, and defect density.

**3. Function Points (FP) Analysis depends exclusively on source-code length - False**

Function Point Analysis estimates software size based on the functionality delivered to users, considering elements such as inputs, outputs, inquiries, internal logical files, and external interface files. <br/>
It does not depend exclusively on source-code length.

> - **Process metric** -> How well the work is done.
> - **Product metric** -> Characteristics of the software.
> - **Function Points(FP)** -> Functionality, not lines of code.
  
</details>
<!--------------------->

---

Q 43. Which limitation is most closely associated with LOC-based software size estimation?
- [ ] A. It ignores coding language
- [x] B. It depends on coding language
- [ ] C. It measures user satisfaction
- [ ] D. It excludes source code

<details>
  <summary>  Lines of code (LOC)-based, depends on coding language </summary>

<br/>
  
</details>
<!--------------------->

---

Q 44. In **Function Points(FP) Analysis**, which component represents a logical group of data maintained by the application?
- [ ] A. External Inquiry (EQ)
- [ ] B. External Output  (EO)
- [ ] C. External Input   (EI)
- [x] D. Internal Logical File (ILF)

<details>
  <summary> <b> Internal Logical File (ILF) </b> </summary>

<br/>

In Function Point (FP) Analysis, an Internal Logical File (ILF) represents a logical group of data that is maintained within the application boundary by the application being measured.

Example <br/>
In a school management system, student records stored and maintained by that application form an ILF.

**FP components to remember**

| Component	| Meaning                                                            |
|-----------|--------------------------------------------------------------------|
| ILF	      | Logical data group maintained by the application                   |
| EIF	      | Data used by the application but maintained by another application |
| EI	      | External Input - data entering the application                     |
| EO	      | External Output - processed data leaving the application           |
| EQ	      | External Inquiry - request and response with minimal processing    |

> **ILF = Internal + Maintained;**

> **EIF = External + Referenced.**
  
</details>
<!--------------------->

---

Q 45. Which basic COCOMO project mode is most appropriate for a complex system with stringent harware, software and operational constraints?
- [ ] A. Organic mode
- [ ] B. Semi-detached mode
- [x] C. Embedded mode
- [ ] D. Prototype mode

<details>
  <summary> Embedded mode </summary>

<br/>

The Embedded mode in Basic COCOMO is appropriate for complex software systems operating under stringent hardware, software, and operational constraints.

Organic mode: Suitable for relatively small, simple projects with familiar requirements and an experienced team.

Semi-detached mode: Suitable for projects of intermediate complexity, with a mix of experienced and less-experienced team members.

Embedded mode: Suitable for systems with tight constraints, such as real-time control systems, avionics, and medical-device software.

Prototype mode: Prototyping is a development approach, not one of the three Basic COCOMO project modes.

| COCOMO mode	  | Key clue                                         |
|---------------|--------------------------------------------------|
| Organic	      | Small and relatively simple                      |
| Semi-detached	| Intermediate complexity                          |
| Embedded	    | Strict hardware/software/operational constraints |
  
</details>
<!--------------------->

---

Q 46. The **Delphi Technique** is primarily used in software cost estimation to:
- [x] A. obtain experts consensus
- [ ] B. measure source-code length
- [ ] C. calculate program value
- [ ] D. determine defect density

<details>
  <summary> Delphi = Experts + Anonymous opinions + Multiple rounds + Consensus. </summary>

<br/>

**How the Delphi Technique works**

The Delphi Technique is an expert-based estimation method used to estimate software development effort, cost, or project duration.
1. A group of experts independently provides estimates.
2. Their estimates are collected anonymously.
3. A summary of the estimates is shared with the experts.
4. Experts reconsider and revise their estimates over several rounds.
5. The process continues until estimates converge sufficiently toward a consensus.

> **Delphi relies on expert judgment; COCOMO uses a mathematical estimation model.**


**Obtain experts' consensus**: The technique combines expert judgment through structured, iterative feedback.

**Measure source-code length**: LOC (Lines of Code) measures code size.

Calculate program value: This is not the primary purpose of Delphi estimation.

Determine defect density: Defect density measures defects relative to software size.
  
</details>
<!--------------------->

---

Q 47. In **Basic COCOMO**, the estimated effort is expressed in:
- [ ] A. Line per month
- [x] B. Person-months
- [ ] C. Function Points
- [ ] D. Calendar years

`E = a(KLOC)^b`, where `E` is effort, `KLOC` is lines of code in thousand, `a` and `b` are predefined values depends organic, semi-detached or embeded project mode to calculate in effort in **Person-months**

<details>
  <summary> Person-months </summary>

<br/>

In Basic COCOMO, estimated software development effort is expressed in **person-months (PM)**.

**COCOMO effort = Person-months; schedule = Months.**

Basic COCOMO uses the effort equation: **`E = a(KLOC)^b`**
- Here, `E` is effort in person-months, and KLOC means thousands of lines of code.
- The constants `a` and `b` depend on the project mode(organic, semi-detached or embeded).
  
</details>
<!--------------------->

---

Q 48. Which relationship is used in **Putnam's Software Estimation Model**?
- [ ] A. Effort is independent of time
- [ ] B. Size depends only on LOC
- [ ] C. Staffing remains constant throughout
- [x] D. Development time strongly affects effort

> **Putnam = Size + Effort + Time + Rayleigh staffing curve.**

<details>
  <summary> Putnam's Software Estimation Model </summary>

<br/>

**Putnam's Software Estimation Model** describes _the relationship among software size, development time, and effort_. 

It uses a **Rayleigh curve to model how staffing effort is distributed over the project lifecycle**.

> **Putnam = Size + Effort + Time + Rayleigh staffing curve.**
  
</details>
<!--------------------->

---

Q 49. Which statement best distinguish functional requirements from non-functional requirements?
- [x] A. Functional requirement specify system behaviour
- [ ] B. Functional requirement specify quality levels
- [ ] C. Non-Functional requirement define user inputs
- [ ] D. Non-Functional requirement define usystemr outputs

<details>
  <summary> functional requirements vs non-functional requirements </summary>

<br/>

In Software Engineering, requirements describe **what a software system must do** and **the qualities or constraints it must satisfy**.

| Basis	                      | Functional Requirements	              | Non-functional Requirements                          |
|-----------------------------|---------------------------------------|------------------------------------------------------|
| Meaning	                    | Describe what the system does	        | Describe how well the system works or its constraints|
| Focus	                      | Features and behavior	                | Quality attributes and performance                   |
| Examples	                  | Login, registration, search, payment	| Security, speed, reliability, usability              |
| Testing	| Check whether a feature works correctly	| Measure qualities such as response time, security, and availability    |
| Example for a school website | A teacher can upload marks	          | The marks page loads within 2 seconds                |

Example: Banking application

- Functional requirement: <br/>
The application must allow users to transfer money between accounts.

- Non-functional requirement <br/>
The application must display the transfer result within 2 seconds under specified load conditions.

> **Functional = WHAT the system does.**

> **Non-functional = HOW WELL the system does it.**

Both types of requirements are documented in the SRS (Software Requirements Specification).

A requirement states: “The system must support 10,000 concurrent users.” Which type is it?
- [ ] A. Functional requirement
- [x] B. Non-functional requirement
- [ ] C. User input
- [ ] D. Maintenance requirement
  
</details>
<!--------------------->

---

Q 50. Which of the following is the primary objective of **function-oriented software design**?
- [ ] A. Oraganizing the system around objects
- [x] B. Organizing the system around functions
- [ ] C. Eliminating data flow
- [ ] D. Combining all modules

<details>
  <summary> </summary>

<br/>

**Function-oriented design** divides a system into functions or modules, each responsible for a specific task.

Example

A student management system might be divided into these functions: `AddStudent()` -> `CalculateMarks()` -> `GenerateReport()`

Each function performs a specific task.

> **Function-oriented design -> Functions and modules**

**DFD -> data movement and processes -> commonly associated with structured/function-oriented analysis.**

Object-oriented design (OOD), which organizes software around objects and classes.

> **Object-oriented design -> Objects and classes**
  
</details>
<!--------------------->

---

Q 51. In the Software Engineering Institute's **Capability Maturity Model(CMM)**, which level is characterized by a defined and documented standard software process across the organization?
- [ ] A. Initial
- [ ] B. Repeatable
- [x] C. Defined
- [ ] D. Optimizing

<details>
  <summary> </summary>

<br/>

In the Software Engineering Institute's Capability Maturity Model (CMM), Level 3 means the organization has a standard, documented software process that is established and followed across the organization.

**Level-1: Initial** <br/>
Ad hoc <br/>
Entry-level, organization/Office or freelancing where 1-2 projects are handled, starting point in ad-hoc.

**Level-2: Repeatable** <br/>
Repeat successful practices <br/>
Establishes basic project-management practices to repeat previous successes. <br/>
Capabibilities of Building same kind of products repeatedly by improving few levels

**Level-3: Defined** <br/>
Organization-wide documented process <br/>
Establishes documented, standardized processes across the organization.


**Level-4: Managed** <br/>
Measured and quantitatively controlled <br/>
Organizations use data to monitor process performance and maintain predictable results.


**Level-5: Optimizing** <br/>
Continuous improvement <br>
Focuses on continuous improvement and preventing defects. <br/>
Investing in new new ideas

Which CMM level emphasizes quantitative measurement and control of software processes?
- [ ] A. Repeatable
- [ ] B. Defined
- [x] C. Managed
- [ ] D. Optimizing
  
</details>
<!--------------------->

---

Q 52. Which principle is most desirable in structured software design?
- [ ] A. High coupling and low cohesion
- [ ] B. High coupling and high cohesion
- [x] C. Low coupling and low cohesion
- [ ] D. Low coupling and high cohesion

> **Coupling = how strongly one module depends on another module.**

> **Cohesion = how closely related the tasks within a single module are.**

<details>
  <summary> Low Coupling and High Cohesion </summary>

<br/>

This is a fundamental principle of structured software design.

### 1. Understand the two concepts

**Coupling** = how strongly one module depends on another module.
- Low coupling: Modules are relatively independent, so changing one module has minimal impact on others.
- High coupling: Modules depend heavily on one another, making changes and maintenance more difficult.

Cohesion = how closely related the tasks within a single module are.
- High cohesion: A module focuses on one well-defined responsibility.
- Low cohesion: A module performs unrelated tasks.

Example: Imagine a school management system.
- High cohesion: A FeeCalculator module calculates student fees and handles related fee calculations.
- Low coupling: The fee module works independently and interacts with other modules through clear interfaces.
This design is easier to test, maintain, reuse, and modify.

A module that performs only database backup and restoration tasks has which desirable property?
- [x] A. High cohesion
- [ ] B. High coupling
- [ ] C. Low cohesion
- [ ] D. High redundancy
  
</details>
<!--------------------->

---

Q 53. Which statement best describes **object-oriented design(OOD)**?
- [x] A. It models a system using object and classes
- [ ] B. It focuses only on data flow
- [ ] C. It eliminates encapsulation
- [ ] D. It organizes software only into functions

<details>
  <summary> <b> Object-Oriented Design (OOD) </b> </summary>

<br/>

Object-Oriented Design (OOD) is a software design approach that organizes a system around objects and classes, combining data (attributes) and behavior (methods).

Example: **Consider a school management system**

<img width="766" height="542" alt="image" src="https://github.com/user-attachments/assets/b3d7fc5b-eb97-4eac-9bbb-d643a2e232bd" />


### 2. Four important OOD/OOP concepts

| Concept	      | Meaning	                                      | Example                                                    |
|---------------|-----------------------------------------------|------------------------------------------------------------|
| Encapsulation	| Bundling data and methods; controlling access	| Protecting a student's marks                               |
| Abstraction	  | Hiding implementation details	                | Using `print()` without knowing its internal implementation|
| Inheritance	  | Creating a class based on another class	      | GraduateStudent inherits from Student                      |
| Polymorphism	| Same interface, different behavior	          | Different classes implement calculateFee() differently     |


### 3. OOD vs function-oriented design

| Object-oriented design	              | Function-oriented design                 |
|---------------------------------------|------------------------------------------|
| Organized around objects and classes	| Organized around functions and processes |
| Emphasizes data and behavior together	| Emphasizes transformations of data       |
| Commonly uses class diagrams and UML	| Commonly uses Data Flow Diagrams (DFDs)  |

### 4. Connection with coupling and cohesion

Object Oriented Design(OOD) also aims for **low coupling and high cohesion**:
- A class should have a clear, focused responsibility.
- Classes should depend on one another as little as reasonably possible.

> **OOD -> objects + classes + attributes + methods**.

  
</details>
<!--------------------->

---

Q 54. Which statemenr correctly distinguishes **debugging from testing**?
- [ ] A. Testing removes defects from code
- [x] B. Debugging identifies and fixes defect causes
- [ ] C. Testing requires sourcecode access
- [ ] D. Debugging replaces system testing

<details>
  <summary> Debugging from Testing </summary>

<br/>

> **Testing detects defects, while Debugging investigates and fixes them.**

### Testing

Finds failures or defects by executing or evaluating software.

Example: Run a login test and discover that valid users cannot log in.

### Debugging

Locates the cause of a defect and corrects it.

Example: Inspect the login code, find an incorrect password comparison, and fix it.

| Testing	                                  | Debugging                                |
|-------------------------------------------|------------------------------------------|
| Detects failures	                        | Finds and fixes their causes             |
| Checks whether software behaves correctly	| Investigates why it behaves incorrectly  |
| Can be performed by testers or developers	| Usually performed by developers          |
| May reveal a defect	                      | Starts from a known or suspected problem |

**Typical sequence:** <br/>
Testing reveals a failure -> debugging identifies and fixes the cause -> testing is repeated to verify the fix.

> **Testing = detect; Debugging = diagnose and fix.**

Different terms and meaning
- Testing: Detects failures, such as a program crashing during execution.
- Debugging: Examines the code, traces the problem, and fixes its cause.
- Deployment: Releases software into its target environment.
- Requirement analysis: Identifies and documents what the software must do.
  
</details>
<!--------------------->

---

Q 55. Which tool is most suitable for identitying potential memory leaks and invalid memory access during program execution?
- [ ] A. Requirement traceability matrix
- [ ] B. Data Flow Diagram
- [x] C. Dynamic analysis tool
- [ ] D. Project scheduling tool

<details>
  <summary> <b> Dynamic analysis tool </b> </summary>

<br/>

A dynamic analysis tool examines a program while it is running. 

It can help detect:
- Memory leaks: Allocated memory that is no longer needed but is not released.
- Invalid memory access: Accessing memory illegally, such as reading or writing outside an allocated array.
- Runtime errors: Problems that occur during program execution.

Examples include **Valgrind** and **AddressSanitizer (ASan)**.


  
</details>
<!--------------------->

---

Q 56. In Musa's Basic Execution Time Model, software failure intensity is primarily related to:
- [x] A. Execution time and remaining faults
- [ ] B. Number of developers only
- [ ] C. Source-code length only
- [ ] D. Hardware cost only

<details>
  <summary> Musa's Basic Execution Time Model </summary>

<br/>

Musa's Basic Execution Time Model is a software reliability model used to predict how software failure intensity changes as the software is executed and faults are detected and removed.

**Execution time**: The model tracks software reliability as execution proceeds.

**Remaining faults**: As faults are detected and removed, the failure intensity generally decreases, assuming the model’s underlying conditions hold.

**Failure intensity**: The expected rate of software failures per unit of execution time.
  
</details>
<!--------------------->

---

Q 57. Which activity is most directly associated with **Software Quality Assurance(SQA)**?
- [ ] A. Fixing every defect after delivery
- [ ] B. Increasing code size
- [ ] C. Eliminating all documentations
- [x] D. Ensuring processes follow quality standards

<details>
  <summary> Software Quality Assurance(SQA) </summary>

<br/>

Software Quality Assurance (SQA) is a set of planned and systematic activities used to ensure that software development processes follow defined standards and are capable of producing quality software.

> **SQA focuses on preventing defects by improving the process used to develop software.**

### What does SQA do?

- Establishes software development standards and procedures.
- Checks whether the team follows the defined processes.
- Conducts process audits and reviews.
- Monitors compliance with quality requirements.
- Helps prevent defects and improve software development practices.

Example: A software company establishes coding standards and reviews whether developers follow them throughout development. This is an SQA activity.

### SQA vs SQC

| Software Quality Assurance (SQA)	              | Software Quality Control (SQC)                 |
|-------------------------------------------------|------------------------------------------------|
| Process-oriented	                              | Product-oriented                               |
| Focuses on defect prevention	                  | Focuses on defect detection                    |
| Ensures development processes follow standards	| Checks whether the software meets requirements | 
| Examples: process audits, standards compliance	| Examples: software testing, product inspection |

<img width="511" height="222" alt="image" src="https://github.com/user-attachments/assets/20eef8bd-b861-41ff-98b3-3bb5290304e1" />

> **QA = Assurance of the process**

> **QC = Control of the product**

SQA does not mean that defects can never occur; it helps establish processes that reduce the likelihood of defects.

Which of the following is primarily an SQA activity?
- [ ] A. Executing test cases to find bugs in the final product
- [x] B. Conducting a process audit to verify compliance with development standards
- [ ] C. Fixing a syntax error in source code
- [ ] D. Installing software on the customer's computer
  
</details>
<!--------------------->

---

Q 58. A tester checks whether a program produces the expected output for valid and invalid inputs from login page. This is an
example of:
- [x] A. Black-box testing
- [ ] B. White-box testing
- [ ] C. Path testing
- [ ] D. Mutation testing

<details>
  <summary> Black-box testing </summary>

<br/>

**Black-box testing** checks whether software produces the expected outputs for given inputs without requiring knowledge of its internal code or structure.

Example: A tester checks a login page using:
- Valid username and password -> login succeeds.
- Invalid password -> an error message appears.
- Empty fields -> validation message appears.

The tester focuses on the system’s externally observable behavior.

- Black-box testing: Tests inputs and outputs without examining internal implementation.
- White-box testing: Examines internal code, logic, conditions, and execution paths.
- Path testing: A white-box technique that tests selected execution paths through a program.
- Mutation testing: Introduces small changes into code to evaluate whether the test suite detects them.
  
</details>
<!--------------------->

---

Q 59. Which statement correctly distinguish ISO 9000 from SEI CMM?
- [x] A. ISO 9000 focuses on quality system, while CMM assesses process maturity.
- [ ] B. ISO 9000 measures code size, while CMM measures program output.
- [ ] C. ISO 9000 applies only to software, while CMM applies to hardware.
- [ ] D. ISO 9000 defines testing levels, while CMM defines coding styles.


<details>
  <summary> </summary>

<br/>
  
</details>
<!--------------------->

---

Q 60. Which of the following best define coupling in software design?
- [ ] A. The degree of interaction within module
- [x] B. The degree of dependency between modules
- [ ] C. The number of functions in a module
- [ ] D. The number of statements in a program

<details>
  <summary> Coupling in software design </summary>

<br/>

**Coupling** in software design is the degree of interdependence between different modules in a software system.
- **Low coupling**: Modules are relatively independent, making software easier to maintain and modify.
- **High coupling**: Modules depend heavily on one another, making changes more difficult.

> **Coupling = between modules;**

> **cohesion = within a module.**

Desirable design aims for **low coupling and high cohesion**.
  
</details>
<!--------------------->
