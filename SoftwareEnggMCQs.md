
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

Q 22. Putnam's Model is used for estimating:
- [ ] A. Software size
- [ ] B. Software development time
- [ ] C. Software Complexity
- [ ] D. Software testing effors

<details>
  <summary> </summary>

<br/>
  
</details>
<!--------------------->

---

Q 23.
- [ ] A.
- [ ] B.
- [ ] C.
- [ ] D.

<details>
  <summary> </summary>

<br/>
  
</details>
<!--------------------->

---

Q 24.
- [ ] A.
- [ ] B.
- [ ] C.
- [ ] D.

<details>
  <summary> </summary>

<br/>
  
</details>
<!--------------------->

---

Q 25.
- [ ] A.
- [ ] B.
- [ ] C.
- [ ] D.

<details>
  <summary> </summary>

<br/>
  
</details>
<!--------------------->

---

Q 26.
- [ ] A.
- [ ] B.
- [ ] C.
- [ ] D.

<details>
  <summary> </summary>

<br/>
  
</details>
<!--------------------->

---

Q 27.
- [ ] A.
- [ ] B.
- [ ] C.
- [ ] D.

<details>
  <summary> </summary>

<br/>
  
</details>
<!--------------------->

---

Q 28.
- [ ] A.
- [ ] B.
- [ ] C.
- [ ] D.

<details>
  <summary> </summary>

<br/>
  
</details>
<!--------------------->

---

Q 29.
- [ ] A.
- [ ] B.
- [ ] C.
- [ ] D.

<details>
  <summary> </summary>

<br/>
  
</details>
<!--------------------->

---

Q 30.
- [ ] A.
- [ ] B.
- [ ] C.
- [ ] D.

<details>
  <summary> </summary>

<br/>
  
</details>
<!--------------------->

---

Q 31.
- [ ] A.
- [ ] B.
- [ ] C.
- [ ] D.

<details>
  <summary> </summary>

<br/>
  
</details>
<!--------------------->

---

Q 32.
- [ ] A.
- [ ] B.
- [ ] C.
- [ ] D.

<details>
  <summary> </summary>

<br/>
  
</details>
<!--------------------->

---

Q 33.
- [ ] A.
- [ ] B.
- [ ] C.
- [ ] D.

<details>
  <summary> </summary>

<br/>
  
</details>
<!--------------------->

---

Q 34.
- [ ] A.
- [ ] B.
- [ ] C.
- [ ] D.

<details>
  <summary> </summary>

<br/>
  
</details>
<!--------------------->

---

Q 35.
- [ ] A.
- [ ] B.
- [ ] C.
- [ ] D.

<details>
  <summary> </summary>

<br/>
  
</details>
<!--------------------->

---

Q 36.
- [ ] A.
- [ ] B.
- [ ] C.
- [ ] D.

<details>
  <summary> </summary>

<br/>
  
</details>
<!--------------------->

---

Q 37.
- [ ] A.
- [ ] B.
- [ ] C.
- [ ] D.

<details>
  <summary> </summary>

<br/>
  
</details>
<!--------------------->

---

Q 38.
- [ ] A.
- [ ] B.
- [ ] C.
- [ ] D.

<details>
  <summary> </summary>

<br/>
  
</details>
<!--------------------->

---

Q 39.
- [ ] A.
- [ ] B.
- [ ] C.
- [ ] D.

<details>
  <summary> </summary>

<br/>
  
</details>
<!--------------------->

---

Q 40.
- [ ] A.
- [ ] B.
- [ ] C.
- [ ] D.

<details>
  <summary> </summary>

<br/>
  
</details>
<!--------------------->

---

Q 41.
- [ ] A.
- [ ] B.
- [ ] C.
- [ ] D.

<details>
  <summary> </summary>

<br/>
  
</details>
<!--------------------->

---

Q 42.
- [ ] A.
- [ ] B.
- [ ] C.
- [ ] D.

<details>
  <summary> </summary>

<br/>
  
</details>
<!--------------------->

---

Q 43.
- [ ] A.
- [ ] B.
- [ ] C.
- [ ] D.

<details>
  <summary> </summary>

<br/>
  
</details>
<!--------------------->

---

Q 44.
- [ ] A.
- [ ] B.
- [ ] C.
- [ ] D.

<details>
  <summary> </summary>

<br/>
  
</details>
<!--------------------->

---

Q 45.
- [ ] A.
- [ ] B.
- [ ] C.
- [ ] D.

<details>
  <summary> </summary>

<br/>
  
</details>
<!--------------------->

---

Q 46.
- [ ] A.
- [ ] B.
- [ ] C.
- [ ] D.

<details>
  <summary> </summary>

<br/>
  
</details>
<!--------------------->

---

Q 47.
- [ ] A.
- [ ] B.
- [ ] C.
- [ ] D.

<details>
  <summary> </summary>

<br/>
  
</details>
<!--------------------->

---

Q 48.
- [ ] A.
- [ ] B.
- [ ] C.
- [ ] D.

<details>
  <summary> </summary>

<br/>
  
</details>
<!--------------------->

---

Q 49.
- [ ] A.
- [ ] B.
- [ ] C.
- [ ] D.

<details>
  <summary> </summary>

<br/>
  
</details>
<!--------------------->

---

Q 50.
- [ ] A.
- [ ] B.
- [ ] C.
- [ ] D.

<details>
  <summary> </summary>

<br/>
  
</details>
<!--------------------->

---

Q 51.
- [ ] A.
- [ ] B.
- [ ] C.
- [ ] D.

<details>
  <summary> </summary>

<br/>
  
</details>
<!--------------------->
