
## DBMS (Database Management System)

Q 1. What is a **NoSQL database**?
- [x] A. A NoSQL database is a database that doesn't use the relational model.
- [ ] B. A NoSQL database is a database that is not manage by a DBMS
- [ ] C. A NoSQL database is a database that is not stored on a physical device.
- [ ] D. All of above

<details>
  <summary> <b> NoSQL Database </b> </summary>

<br/>

A NoSQL database is a **non-relational database** designed to store and manage data using models such as documents, key-value 
pairs, wide-column stores, or graphs.

Unlike traditional relational databases, NoSQL databases often support flexible data structures and horizontal scaling.


### Types of NoSQL databases

**1. Document database**
Stores data as documents, commonly JSON-like structures.

Example: `MongoDB`

<img width="292" height="286" alt="image" src="https://github.com/user-attachments/assets/638dda81-5e8b-44a6-8eb8-a51307bad99e" />


**2. Key-value database** <br/>
Stores values associated with unique keys.

Example: Redis

<img width="296" height="246" alt="image" src="https://github.com/user-attachments/assets/0bc1d331-25b7-4710-be1f-3dfd50d8e5b3" />


**3. Wide-column database** <br/>
Organizes data into rows and column families.

Example: `Apache Cassandra`

<img width="315" height="122" alt="image" src="https://github.com/user-attachments/assets/9d13bd61-39e1-4832-a5b1-64b5083fd57e" />


**4. Graph database** <br/>
Represents data as nodes and relationships.

Example: `Neo4j`

<img width="392" height="207" alt="image" src="https://github.com/user-attachments/assets/dd902bf9-20c5-4a04-81aa-8276e799a432" />

### SQL vs NoSQL

| SQL databases	                   | NoSQL databases                                         |
|----------------------------------|---------------------------------------------------------|
| Primarily **relational tables**	 | **Documents, key-value pairs, graphs, or wide columns** |
| Often use **predefined schemas** | Often support **flexible schemas**                      |
| Commonly use SQL	               | Query methods depend on the database                    |
| Example: MySQL	                 | Example: MongoDB                                        |

**NoSQL** does not mean that a database can't use SQL-like queries or transactions. Capabilities vary by database.

> **Document -> Key-value -> Wide-column -> Graph**

- `MySQL`: Relational database (RDBMS).
- `Oracle Database`: Primarily a relational database.
- `Microsoft SQL Server`: Relational database (RDBMS).
- `MongoDB`: Document-oriented NoSQL database.
- `Redis`: Key-value
- `Cassandra`: Wide-column
- `Neo4j`: Graph


</details>
<!--------------------->

---

Q 2. What is **CRUD** in DMBS?
- [x] A. Create, Read, Update, Delete
- [ ] B. Cache, Read, Update, Delete
- [ ] C. Copy, Replace, Update, Delete
- [ ] D. Collect, Read, Use, Discard

<details>
  <summary> <b> CRUD = Create, Read, Update, Delete </b> </summary>

<br/>

**CRUD** represents the four basic operations used to manage data in a database.

CRUD stands for:
- C - Create: Insert new records.
- R - Read: Retrieve or view existing records.
- U - Update: Modify existing records.
- D - Delete: Remove records.

Example: Student database
| ID	| Name	| Marks |
|-----|-------|-------|
| 101	| Aman	| 85    |
| 102	| Priya	| 90    |

**Create (Insert a record)**
```sql
INSERT INTO Student (ID, Name, Marks)
VALUES (103, 'Rahul', 78);
```

**Read (Retrieve records)**
```sql
SELECT * FROM Student;
```
**Update (Modify marks)**
```sql
UPDATE Student SET Marks = 95 WHERE ID = 101;
```
**Delete (Remove a record)**
```sql
DELETE FROM Student WHERE ID = 102;
```



</details>
<!--------------------->

---

Q 3. SQL implies conditions on the groups through ________ clause after grough have been formed.
- [ ] A. `WHERE`
- [x] B. **`HAVING`**
- [ ] C. `NEW`
- [ ] D. `ALL`

<details>
  <summary> <b> HAVING </b> </summary>

<br/>

### `HAVING` vs `WHERE`

- `WHERE` filters individual rows before grouping.
- `HAVING` filters groups after aggregation.

```sql
SELECT Class, AVG(Marks)
FROM Student
GROUP BY Class
HAVING AVG(Marks) > 75;
```
This displays only classes whose average marks exceed 75.

</details>
<!--------------------->

---

Q 4. Ginni has created a table, `SCORE` in MySQL to store runs scored by players in a cricket match. The table contains the following records:
| PLAYERS | SCORE |
|---------|-------|
| Ranveer | 50    |
| Suresh  | 35    |
| Mirza   | 10    |
| John    | 51    |
| Murugan | 70    |
Which of the following give 10 as output:
- [ ] A. `SELECT MAX(score) FROM scores;`
- [x] B. `SELECT MIN(score) FROM scores;`
- [ ] C. `SELECT SUM(score) FROM scores;`
- [ ] D. `SELECT AVG(score) FROM scores;`

<details>
  <summary> <b> Aggregate Functions  </b> </summary>

<br/>

**Aggregate functions** perform calculations on a group of rows and return a single result.

They are commonly used with the SQL `SELECT`, `GROUP BY`, and `HAVING` clauses.

| Function	| Purpose                         |	Example            |
|-----------|---------------------------------|--------------------|
| `COUNT()`	| Counts rows or non-NULL values	| Number of students |
| `SUM()`	  | Calculates total	              | Total marks        |
| `AVG()`	  | Calculates average	            | Average marks      |
| `MAX()`	  | Finds maximum value	            | Highest marks      |
| `MIN()`	  | Finds minimum value	            | Lowest marks       |

```sql
SELECT COUNT(*) FROM Student;
SELECT SUM(Marks) FROM Student;
SELECT AVG(Marks) FROM Student;
SELECT MAX(Marks) FROM Student;
SELECT MIN(Marks) FROM Student;
```

### `COUNT(*)` vs `COUNT(column)`

- `COUNT(*)` counts all rows.
- `COUNT(Marks)` counts only rows where Marks is not `NULL`.

### `GROUP BY` with aggregate functions

```sql
SELECT Class, AVG(Marks) FROM Student GROUP BY Class;
```

### `HAVING` vs `WHERE`

- `WHERE` filters individual rows before grouping.
- `HAVING` filters groups after aggregation.

```sql
SELECT Class, AVG(Marks)
FROM Student
GROUP BY Class
HAVING AVG(Marks) > 75;
```
This displays only classes whose average marks exceed 75.

</details>
<!--------------------->

---

Q 5. __________ offers the ability to query the data and `insert`, `alter` and `delete` tuples.
- [ ] A. Trasaction Control Language(TCL)
- [ ] B. Data Control Language(DCL)
- [ ] C. Data Definition Language(DDL)
- [x] D. Data Manipulation Language(DML)

<details>
  <summary> <b> Classification of SQL commands </b> </summary>

<br/>

SQL commands are commonly classified into five categories:

<img width="560" height="647" alt="image" src="https://github.com/user-attachments/assets/091d3c9f-d32c-4464-9c10-f6cabbf8f3c0" />



| Category	                        | Main purpose	              | commands                                           |
|-----------------------------------|-----------------------------|----------------------------------------------------|
| DDL	(Data Definition Language)    | Define, Structure	          | `CREATE`, `ALTER`, `DROP`, `TRUNCATE`, `RENAME`    |
| DML	(Data Manipulation Language)  | Modify data	                | `INSERT`, `UPDATE`, `DELETE`                       |
| DQL	(Data Query Language)         | Query, Retrieve data	      | `SELECT`                                           |
| DCL	(Data Control Language)       | Control access, Permissions	| `GRANT`, `REVOKE`                                  |
| TCL	(Transaction Control Language)| Transactions	              | `COMMIT`, `ROLLBACK` `SAVEPOINT`, `SET TRANSACTION`|

### 1. DDL - Data Definition Language

DDL is used to create or modify database structures.

**CREATE**: to create structure
```sql
CREATE TABLE Student (
    ID INT,
    Name VARCHAR(50),
    Marks INT
);
```
**ALTER**: to alter already created structure
```sql
ALTER TABLE Student ADD Age INT;
```

**DROP** : to drop structure permanently
```sql
DROP TABLE Student;
```

**TRUNCATE**: to delete the data, not the structure
```sql
TRUNCATE TABLE Student;
```

### 2. DML - Data Manipulation Language

DML is used to insert, modify, and delete records.

**INSERT**: to insert
```sql
INSERT INTO Student
VALUES (101, 'Aman', 85);
```
**UPDATE** to update/modify
```sql
UPDATE Student
SET Marks = 95
WHERE ID = 101;
```

**DELETE**: to delete
```sql
DELETE FROM Student
WHERE ID = 101;
```


### 3. DQL - Data Query Language

DQL is used to retrieve information.

**SELECT**: `SELECT *` to retrieve all columns
```sql
SELECT * FROM Student;
````

`SELECT column` to retrieve only student names:
```sql
SELECT Name FROM Student;
```

### 4. DCL - Data Control Language

DCL is used to control database access and permissions.

DCL manages user privileges and database access.

**GRANT**: Gives user1 permission to read the Student table.
```sql
GRANT SELECT ON Student TO user1;
```
**REVOKE**: Removes that permission.
```sql
REVOKE SELECT ON Student FROM user1;
```



### 5. TCL - Transaction Control Language

TCL is used to manage database transactions.

**COMMIT**: Permanently saves the current transaction's changes.
```sql
COMMIT;
```
`COMMIT` saves the transaction's changes.

**ROLLBACK**: Undoes uncommitted changes.
```sql
ROLLBACK;
```

**SAVEPOINT**: Creates a point to which you can roll back within a transaction.
```sql
SAVEPOINT sp1;
```


</details>
<!--------------------->

---

Q 6. What is **DBMS**?
- [ ] A. DBMS is a collection of queries
- [ ] B. DBMS is a high-level language
- [ ] C. DBMS is a programming langauge
- [x] D. DBMS stores, modifies and retrieve data

<details>
  <summary> <b> DBMS stands for Database Management System </b> </summary>

<br/>

> A DBMS is software that allows users **to create, store, organize, retrieve, update, and manage data** in a database.

In simple words, a DBMS acts as an interface between users/applications and the database.

### How DBMS Works?

<img width="315" height="410" alt="image" src="https://github.com/user-attachments/assets/89840683-2a81-48aa-810b-380b1ca791b4" />

### 2. Examples of DBMS

| DBMS	                  | Type             |
|-------------------------|------------------|
| `MySQL`	                | Relational       |
| `Oracle Database`	      | Relational       |
| `Microsoft SQL Server`	| Relational       |
| `PostgreSQL`	          | Relational       |
| `SQLite`	              | Relational       |
| `MongoDB`	              | NoSQL / Document |
| `Neo4j`                 | Graph database   |
| `Redis`                 | Key-value NoSQL  |


### 3. Main functions of DBMS

1. Data storage: Stores data systematically.
2. Data retrieval: Retrieves information when requested.
3. Data security: Controls unauthorized access.
4. Data integrity: Maintains data accuracy and consistency.
5. Concurrency control: Allows multiple users to access data safely.
6. Backup and recovery: Helps restore data after failures.
7. Transaction management: Manages database transactions.

### 4. Advantages of DBMS

- Reduces data redundancy.
- Improves data consistency.
- Provides data security.
- Supports data sharing.
- Provides backup and recovery.
- Maintains data integrity.

### 5. DBMS vs RDBMS

| DBMS	                                  | RDBMS                                   |
| General database management system	    | Relational database management system   |
| May use different data models	          | Organizes data using relations (tables) |
| Relationships may or may not be central	| Supports relationships between tables   |
| Example: MongoDB (DBMS, NoSQL)	        | Example: MySQL, Oracle                  |

> **DBMS = software that manages databases.**
   
</details>
<!--------------------->

---

Q 7. Which of the following is not a limitation of **File system**?
- [ ] A. Data Redundancy
- [ ] B. Data Inconsistency
- [ ] C. Data Dependence
- [x] D. Storing spaces

<details>
  <summary> <b> Traditional file system </b> </summary>

<br/>

A **traditional file system** stores data in separate files, often managed by individual applications.

It has several limitations that motivated the development of DBMS.

- Data Redundancy,	A limitation. The same data may be stored in multiple files, wasting storage.
- Data Inconsistency,	A limitation. If duplicated data is updated in one file but not another, values may differ.
- Data Dependence,	A limitation. Changes in file structure may require changes in application programs.
- Storing spaces,	Not a standard limitation. Storing data requires storage space; the option does not describe a recognized file-system problem.

### File-system limitations:

- Data redundancy: Duplicate storage of the same data; generally an undesirable condition.
- Data inconsistency
- Data isolation: Data is scattered across separate files and formats, making access and integration difficult.
- Difficulty in accessing data
- Integrity problems
- Atomicity problems
- Concurrent-access anomalies
- Security problems: Protects data from unauthorized access, modification, or deletion.
- Program-data dependence: Application programs depend on the structure of stored files.


</details>
<!--------------------->

---

Q 8. Which of the following provides the ability to query information from the database and insert tuples into, delete tuples, and modify tuples in the database?
- [x] A. DML(Data Manipulation Language)
- [ ] B. DDL(Data Definition Language)
- [ ] C. Query
- [ ] D. Relational Schema

<details>
  <summary> <b> DML(Data Manipulation Language) </b> </summary>

<br/>

</details>
<!--------------------->

---

Q 9. What does **SQL** stands for:
- [x] A. **Structured Query Language**
- [ ] B. Simple Query Language
- [ ] C. Systematic Query Logic
- [ ] D. Standard Query Level

<details>
  <summary> <b> SQL stands for Structured Query Language </b> </summary>

<br/>

It is a standard language used to communicate with relational databases (RDBMS) to:
- **Create** database tables.
- **Retrieve** data using `SELECT`.
- **Insert** records using `INSERT`.
- **Update** records using `UPDATE`.
- **Delete** records using `DELETE`.

</details>
<!--------------------->

---

Q 10. Which statement is used **to retrieve data** from a database in SQL?
- [x] A. `SELECT`
- [ ] B. `UPDATE`
- [ ] C. `DELETE`
- [ ] D. `INSERT`

<details>
  <summary> SELECT is used to retrieve data from a database in SQL </summary>

<br/>

</details>
<!--------------------->

---

Q 11. Which of the following a **DML(Data Manipulation Language)** command in SQL?
- [x] A. `UPDATE`
- [ ] B. `CREATE`
- [ ] C. `ALTER`
- [ ] D. `DROP`

<details>
  <summary> UPDATE is DML(Data Manipulation Language) </summary>

<br/>

</details>
<!--------------------->

---

Q 12. 
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

Q 13. The easiest way in which we can transfer crontrol is when the old backup site sends ________ to the old primary.
- [x] A. Redo logs
- [ ] B. Primary logs
- [ ] C. Undo logs
- [ ] D. All of these

<details>
  <summary> <b> Database recovery and site failover/switchover </b> </summary>

<br/>

**Primary site**: The main database site that handles normal operations.

**Backup/standby site**: Maintains a copy of the primary database.

**Redo logs**: Record changes made to the database so those changes can be applied to another database during recovery or synchronization.

During a database role transition, redo information helps keep the databases synchronized.

**Undo logs**: Help reverse uncommitted transactions and provide read consistency.



| Log type	   | Main purpose              |
|--------------|---------------------------|
| Redo	       | Re-apply changes          |
| Undo	       | Reverse/Rollback changes  |
| Archive logs | Store copies of filled redo logs for recovery <br/> Preserve redo-log records for recovery |

</details>
<!--------------------->

---

Q 14. What are the **three main types of DBMS**?
- [x] A. Relational DBMS, Hierarchical DBMS, Network DBMS
- [ ] B. Relational DBMS, Object Oriented DBMS, NoSQL DBMS
- [ ] C. Hierarchical DBMS, Network DBMS, Object-Oriented DBMS
- [ ] D. NoSQl DBMS, Object-Oriented DBMS, Realtional DBMS

<details>
  <summary> <b> Hierarchical DBMS, Network DBMS, Relational DBMS (RDBMS) </b> </summary>

<br/>

The three main types of DBMS commonly taught in introductory Computer Science are:
1. Hierarchical DBMS
2. Network DBMS
3. Relational DBMS (RDBMS)

### 1. Hierarchical DBMS

Data is organized in a **tree-like structure with parent-child relationships**.

<img width="536" height="275" alt="image" src="https://github.com/user-attachments/assets/23a12b72-d976-4fff-a573-71978b521f3e" />

- Each child record generally has only one parent.
- Example: An organization structure with departments and employees.
- Data is accessed through predefined paths.


### 2. Network DBMS

Data is organized like a network of interconnected records.

<img width="511" height="316" alt="image" src="https://github.com/user-attachments/assets/82a6a66b-ec1a-4269-b18c-46c49784f785" />

- A child record can have multiple parent records.
- Supports many-to-many relationships.
- Example: Students enrolled in multiple courses, with each course having multiple students.


### 3. Relational DBMS (RDBMS)

Data is **stored in tables consisting of rows and columns**.

<img width="567" height="310" alt="image" src="https://github.com/user-attachments/assets/1a694e58-3dbf-4b72-a88b-3195b7b07682" />

- Tables are related using keys.
- Uses SQL to manage and retrieve data.
- Examples: MySQL, Oracle, PostgreSQL and SQL Server.


| Feature	      | Hierarchical | Network	         | Relational      |
|---------------|--------------|-------------------|-----------------|
| Structure	    | Tree	       | Graph/network     |	Tables         |
| Relationship	| One-to-many	 | Many-to-many	     | Through keys    |
| Parent records| One	         | Multiple possible | 	Not tree-based |
| Example	      | `IBM IMS`	   | `IDMS`	           | `MySQL`         |

> - Hierarchical = Tree (parent-child relationships)
> - Network = Multiple connections, Interconnected records
> - Relational = Tables (rows and columns)

</details>
<!--------------------->

---

Q 15. In `MySQL`, which type of value should not be enclosed within quotation mark?
- [ ] A. `DATE`
- [ ] B. `VARCHAR`
- [x] C. `FLOAT`
- [ ] D. `CHAR`

| Data type	| Example	     | Quotation marks?|
|-----------|--------------|-----------------|
| `DATE`	  | '2026-10-30' | 	Yes            |
| `VARCHAR`	| 'Ram'	       |  Yes            |
| `FLOAT`	  | 45.75	       |  No             |
| `CHAR`	  | 'A'	         |  Yes            |


<details>
  <summary> <b> SQL Datatypes </b> </summary>

<br/>

SQL provides different data types to define what kind of values a table column can store.

### 1. Numeric data types: Used to store numbers.

| Data type	      | Purpose	                                       | Example      |
|-----------------|------------------------------------------------|--------------|
| `INT`	          | Whole numbers	                                 | `25`         |
| `TINYINT`	      | Small-range integers	                         | `100`        |
| `BIGINT`	      | Very large integers	                           | `9876543210` |
| `FLOAT`	        | Approximate decimal values	                   | `25.75`      |
| `DOUBLE`	      | Approximate decimal values with more precision | `123.456789` |
| `DECIMAL(p,s)`	| Exact decimal values	                         | `DECIMAL(6,2)` -> `1250.50` |

> - `DECIMAL` is preferred for exact financial calculations; 
> - `FLOAT` and `DOUBLE` are preferred for approximate.

### 2. String / Character data types: Used to store text, letters and characters.

| Data type	    | Purpose	                | Example           |
|---------------|-------------------------|-------------------|
| `CHAR(n)`	    | Fixed-length string	    | `'ABC'`           |
| `VARCHAR(n)`	| Variable-length string	| `'Rahul'`         |
| `TINYTEXT`	  | Small text	            | Short description |
| `TEXT`	      | Longer text	            | Article content   |
| `MEDIUMTEXT`	| Medium-sized text	      | Large document    |
| `LONGTEXT`	  | Very large text	        | Extensive content |

**`CHAR` vs `VARCHAR`**
- `CHAR(10)` -> Fixed-length field of 10 characters.
- `VARCHAR(10)` -> Variable-length field, maximum 10 characters.

### 3. Date and Time data types: Used to store dates and time values.

| Data type	  | Purpose	      | Example                 |
|-------------|---------------|-------------------------|
| `DATE`	    | Date	        | `'2026-10-30'`          |
| `TIME`	    | Time	        | `'14:30:00'`            |
| `DATETIME`	| Date and time | `'2026-10-30 14:30:00'` |
| `TIMESTAMP`	| Date and time, with time-zone-related conversion behavior	| `'2026-10-30 14:30:00'` |
| `YEAR`	    | Year value	  | `2026`                  |


### 4. Boolean data type: used to represent logical values.

| Data type	       | Values            |
|------------------|-------------------|
| `BOOLEAN`/`BOOL` | `TRUE` or `FALSE` |

Typically, `0` represents `FALSE` and `1` represents `TRUE`.

### 5. Binary data types: used to store binary data, such as files and raw bytes.

| Data type	     | Purpose                     |
|----------------|-----------------------------|
| `BINARY(n)`	   | Fixed-length binary data    |
| `VARBINARY(n)` | Variable-length binary data |
| `TINYBLOB`	   | Small binary objects        |
| `BLOB`	       | Binary large objects        |
| `MEDIUMBLOB`	 | Medium-sized binary objects |
| `LONGBLOB`	   | Large binary objects        |


| Summary of the five categories                         |
|--------------------------------------------------------|
| 1. Numeric - `INT`, `FLOAT`, `DOUBLE`, `DECIMAL`       |
| 2. String - `CHAR`, `VARCHAR`, `TEXT`                  |
| 3. Date/Time - `DATE`, `TIME`, `DATETIME`, `TIMESTAMP` |
| 4. Boolean - `BOOL`, `BOOLEAN`                         |
| 5. Binary - `BINARY`, `VARBINARY`, `BLOB`              |

</details>
<!--------------------->

---

Q 16. In general, **a file is basically a collection of all related**:
- [ ] A. Rows and Columns
- [ ] B. Database
- [ ] C. Fields
- [x] D. Records

<details>
  <summary> <b> File: Collection of related records </b> </summary>

<br/>

> **A file is generally a collection of related records.**

<img width="667" height="455" alt="image" src="https://github.com/user-attachments/assets/142ce6ca-3985-4459-b523-31f6b8de6d34" />


**Understand the data hierarchy**

| Term	        | Meaning	                                   | Example                          |
|---------------|--------------------------------------------|----------------------------------|
| **Field**	    | Single data item	                         | Name = Rahul                     |
| **Record**	  | Collection of related fields	             | Rahul's complete student details |
| **File**	    | Collection of related records	             | Student file                     |
| **Database**	| Collection of related data/files or tables | School database                  |

A collection of related fields is called:
- [ ] A. Database
- [x] B. Record
- [ ] C. File
- [ ] D. Table

In a relational database table, a row generally represents:
- [ ] A. Field
- [x] B. Record
- [ ] C. Database
- [ ] D. File extension

</details>
<!--------------------->

> Hierarchy: **Field -> Record -> File -> Database**
> - **Field(Column)** = Single data item, represents one attribute
> - **Record(Row)** = Collection of related fields, represents one complete entry
> - **File** = Collection of related records
> - **Database** = Organized collection of related data


---

Q 17. Which of the following refers to the **level of data abstraction** that describes exactly how the data stored?
- [ ] A. Conceptual Level
- [x] B. Physical level
- [ ] C. File level
- [ ] D. Logical level

<details>
  <summary> Three levels of data abstraction : Physical(Internal), Conceptual(Logical) and External(View)</summary>

<br/>

<img width="927" height="417" alt="image" src="https://github.com/user-attachments/assets/bc0697b9-7ab8-4d7e-8213-19869d45646b" />

**Physical level (Internal level)** <br/>
Describes exactly how data is actually stored in the database.

It deals with:
- Storage locations
- File organization
- Indexing
- Record placement
- Storage structures

Example: How student records are stored on a disk, which indexes are used, and how files are organized.

**Conceptual Level(logical)** <br/>
Describes what data is stored and relationships among data.

**External Level (View Level)** <br/>
What individual users see

</details>
<!--------------------->

---

Q 18. An index is clustered, if
- [ ] A. it is on set of fields that form a candidate key
- [ ] B. it is on a set of fields that include the primary key
- [x] C. the data records of the file are organized in the same order as data entries of the index
- [ ] D. the data records of the file are organized not in the same order as the data entries of the index

<details>
  <summary> Clustered Index </summary>

<br/>

A **clustered index** is an index in which the physical order of data records in the file follows the order of the index entries.

In simple words, **the actual data is stored in the same order as the clustered index key**.

- **Candidate key**: A candidate key uniquely identifies records. It does not define whether an index is clustered.
- **Primary key**: A clustered index does not have to be on the primary key.
- **Same order**: Data records follow the index-entry order.
- **Different order**: This describes a non-clustered arrangement.

| Clustered index	                | Non-clustered index                      |
|---------------------------------|------------------------------------------|
| Data records follow index order	| Data records need not follow index order |
| Determines data organization	  | Separate index structure                 |
| Typically one per table	        | Multiple can exist                       |

> Clustered = Data clustered together in index order.

> Non-clustered = Index is separate from the data's physical order.

Can a table generally have multiple clustered indexes on different columns in the same physical organization?
- [ ] A. Yes, unlimited
- [x] B. No, generally only one
- [ ] C. Exactly two
- [ ] D. It depends only on the number of rows

Why? <br/>
A clustered index determines the physical order of data records in a table.

A table can have only one physical ordering at a time. Therefore, it generally supports only one clustered index.

However, it can have multiple non-clustered indexes.

Example <br/>
A Student table might have:
- Clustered index on Roll_No
- Non-clustered index on Name
- Non-clustered index on City

> **One table -> Generally one clustered index -> Multiple non-clustered indexes.**

</details>
<!--------------------->

---

Q 19. Which of the following is **a top-down approach** in which the enity's higher level can be divided into two lower sub-entities?
- [ ] A. Aggregation
- [ ] B. Generalization
- [x] C. Specialization
- [ ] D. All of the above

<details>
  <summary> <b> EER (Enhanced Entity-Relationship) model in DBMS </b> </summary>

<br/>

### 1. Specialization

Specialization is a top-down approach in which a higher-level entity (superclass) is divided into lower-level entities (subclasses) based on their specific characteristics.

<img width="962" height="292" alt="image" src="https://github.com/user-attachments/assets/90e73987-fd4c-42a6-bc8d-56668cc9efcc" />


### Specialization vs Generalization vs Aggregation

| Concept	            | Approach	  | Operation                       | Meaning                                        |
|---------------------|-------------|---------------------------------|------------------------------------------------|
| **Specialization**	| Top-down	  | Divide                          | Higher entity -> Lower entities                |
| **Generalization**	| Bottom-up	  | Combine                         | Lower entities -> Higher entity                |
| **Aggregation**	    | Abstraction	| Treat relationship as an entity | Treats a relationship as a higher-level entity |


> - Specialization = `is-a` Top-down = Divide
> - Generalization = `is -a` Bottom-up = Combine
> - Aggregation = `has-a` Relationship abstraction

Combining `Car`, `Bus`, and `Truck` into a higher-level entity called `Vehicle` is an example of:
- [ ] A. Specialization
- [ ] B. Aggregation
- [x] C. Generalization
- [ ] D. Normalization

</details>
<!--------------------->

---

Q 20. The ability to query data, as well as insert, delete and alter tuple is offered by
- [ ] A. TCL(Transaction Control Language)
- [ ] B. DCL(Data Control Language)
- [ ] C. DDL(Data Definition Language)
- [x] D. DML(Data Manipulation Language)

<details>
  <summary> DML(Data Manipulation Language) </summary>

<br/>

</details>
<!--------------------->

---

Q 21. **Aggregate function** can be used with ______ clause. They can't be used with ______ clause.
- [ ] A. `WHERE`, `HAVING`
- [x] B. `HAVING`, `WHERE`
- [ ] C. `GROUP BY`, `HAVING`
- [ ] D. `SELECT`, `HAVING`

<details>
  <summary> HAVING, WHERE </summary>

<br/>

Aggregate functions such as `COUNT()`, `SUM()`, `AVG()`,  `MAX()` and `MIN()` are commonly used with the `HAVING` clause to filter groups.

They generally cannot be used directly in the `WHERE` clause to filter aggregate results.

### `WHERE` vs	`HAVING`

| `WHERE`                                 | 	`HAVING`                   |
|-----------------------------------------|------------------------------|
| Filters individual rows	                | Filters groups               |
| Applied before `GROUP BY`	              | Applied after `GROUP BY`     |   
| Can't directly filter aggregate results | Can filter aggregate results |

`WHERE`: This filters individual employee records.
```sql
SELECT *
FROM Employee
WHERE Salary > 35000;
```

`HAVING`: This filters departments based on their average salary.
```sql
SELECT Department, AVG(Salary)
FROM Employee
GROUP BY Department
HAVING AVG(Salary) > 35000;
```

`HAVING` + `WHERE` : This filters departments based on their average salary and then where avg(salary).
```sql
SELECT Department, AVG(Salary)
FROM Employee
GROUP BY Department
WHERE salary > 30000
HAVING AVG(Salary) > 35000;
```

</details>
<!--------------------->

---

Q 22. Given below Assertion(A) and Reason(R) based on question mark the correct choice as: <br/>
Assertion(A): We can retrieve records from more than one table in MySQL. <br/>
Reason(R): Foreign key is used to established a relationship between two tables.
- [x] A. Both A and R are true, R is the correct explanation of A.
- [ ] B. Both A and R are true, R is not the correct explanation of A.
- [ ] C. A is true but R is not false
- [ ] D. A is false but R is true

<details>
  <summary> Primary key, Foreign key and Joins </summary>

<br/>

- **Primary Key** -> Uniquely identifies a record.
- **Foreign Key** -> References a key in another table.
- **JOIN** -> Retrieves related data from multiple tables.

Student table
| Student_ID | Name  |
|------------|-------|
| 1	         | Rahul |
| 2	         | Priya |

Marks table
| Student_ID | Marks |
|------------|-------|
| 1	         | 85    |
| 2	         | 90    |

We can retrieve data from both tables:
```sql
SELECT Student.Name, Marks.Marks
FROM Student
JOIN Marks
ON Student.Student_ID = Marks.Student_ID;
```

</details>
<!------------------------>

---

Q 23. Which SQL statement is used to update data in database:
- [ ] A. `ALTER`
- [ ] B. `CHANGE`
- [x] C. `UPDATE`
- [ ] D. `MODIFY`

<details>
  <summary> UPDATE </summary>

<br/>

The SQL `UPDATE` statement is used to modify existing records in a database table.

```sql
UPDATE Student
SET Marks = 90
WHERE Roll_No = 101;
```
Always use `WHERE` when you want to update specific records. Without it, all rows may be updated.

|          | Purpose                                                             |
|----------|---------------------------------------------------------------------|
| `ALTER`	 | Changes table structure                                             |
| `CHANGE` | MySQL clause used with `ALTER TABLE` to rename or redefine a column |
| `UPDATE` | Modifies existing records                                           |
| `MODIFY` | MySQL clause used with `ALTER TABLE` to change a column definition  |


| SQL command	| Purpose                |
|-------------|------------------------|
| `INSERT`	  | Add records            |
| `SELECT`	  | Retrieve records       |
| `UPDATE`	  | Modify records         |
| `DELETE`	  | Delete records         |
| `ALTER`	    | Change table structure |
</details>
<!------------------------>

---

Q 24. Which aggregate function in SQL displays the number of values in the specified column ignoring the `NULL` values?
- [ ] A. `len()`
- [x] B. `count()`
- [ ] C. `number()`
- [ ] D. `num()`

<details>
  <summary> Aggregate function: COUNT()  </summary>

<br/>

The SQL `COUNT()` aggregate function counts values in a specified column, excluding `NULL` values.

| Student_ID | Name	  | Marks |
|------------|--------|-------|
| 1	         | Rahul	| 80    |
| 2	         | Priya	| 90    |
| 3	         | Aman	  | NULL  |
| 4	         | Simran	| 70    |

```sql
SELECT COUNT(Marks) FROM Student; -- 3
```
It ignores the `NULL` value.

```sql
SELECT COUNT(*) FROM Student; --4
```
It counts all rows, including rows containing `NULL` values.


| Function	               | What it counts         |
|--------------------------|------------------------|
| `COUNT(*)`	             | All rows               |
| `COUNT(column)`	         | Non-NULL values        |
| `COUNT(DISTINCT column)` | Unique non-NULL values |

</details>
<!------------------------>

---

Q 25. What is the **default format of date** in MySQL?
- [ ] A. `DD-MM-YYYY`
- [ ] B. `MM-DD-YYYY`
- [x] C. `YYYY-MM-DD`
- [ ] D. `YYYY-DD-MM`

<details>
  <summary> Date and Time format </summary>

<br/>

| Date/Time  | Format                |
|------------|-----------------------|
| `DATE`     | `YYYY-MM-DD`          |
| `TIME`     | `HH:MM:SS`            |
| `DATETIME` | `YYYY-MM-DD HH:MM:SS` |

What is the default format of MySQL's `TIME` data type?
- [x] A. `HH:MM:SS`
- [ ] B. `MM:HH:SS`
- [ ] C. `SS:MM:HH`
- [ ] D. `HH:SS:MM`

</details>
<!------------------------>

---

Q 26. Which of the following is a database?
- [ ] A. MySQL
- [ ] B. Informix
- [ ] C. SQL Server
- [x] D. All of the above

<details>
  <summary> MySQL, Informix, and SQL Server - RDBMS </summary>

<br/>

| Database   | Type                        |
|------------|-----------------------------|
| MySQL	     | Open-source RDBMS           |
| Informix	 | IBM's relational DBMS       |
| SQL Server | Microsoft's relational DBMS |

- Database: An organized collection of data.
- DBMS: Software used to create and manage databases.
- RDBMS: A DBMS that stores data in related tables.

Examples of RDBMS: `MySQL`, `Oracle`, `Informix`, `SQL Server`, `PostgreSQL`.

</details>
<!------------------------>

---

Q 27. Which of the following is not a valid **relational operator** used with `WHERE` clause in SQL?
- [ ] A. `>`
- [ ] B. `<=`
- [ ] C. `=`
- [ ] D. `<>`
- [x] E. None of the above

<details>
  <summary> <b> Relational operators in SQL </b> </summary>

<br/>

| Operator	   | Meaning	                 | Example       |
|--------------|---------------------------|---------------|
| `=`	         | Equal to	                 | `Marks = 80`  |
| `<>` or `!=` | Not equal to	             | `Marks <> 80` or `Marks != 80` |
| `>`	         | Greater than	             | `Marks > 80`  |
| `<`	         | Less than	               | `Marks < 80`  |
| `>=`	       | Greater than or equal to	 | `Marks >= 80` |
| `<=` 	       | Less than or equal to	   | `Marks <= 80` |

```sql
SELECT * FROM Student WHERE Marks >= 60;
SELECT * FROM Student WHERE Marks <> 50;
SELECT * FROM Student WHERE Marks = 80;
```

- **Relational operators**: `=`, `<>`, `!=`, `<`, `>`, `<=`, `>=`
- **Logical operators**: `AND`, `OR`, `NOT`.
- **Special comparison/predicate operators**: `IN`, `BETWEEN`, `LIKE`, `IS NULL`.

</details>
<!------------------------>

---

Q 28. Assertion(A) and Reason(R) <br/>
Assertion(A): Foreign key column of a table can't have NULL entries. <br/>
Reason(R): Primary key column of a table can't have NULL entries.
- [ ] A. Both A and R are true and R is the correct explanation of A
- [ ] B. Both A and R are true and R is not the correct explanation of A
- [ ] C. A is true but R is false
- [x] D. A is false but R is true

<details>
  <summary> primary key, foreign key </summary>

<br/>

A foreign key column can contain `NULL` values, provided the column is not declared `NOT NULL`.

```sql
CREATE TABLE Department (
    Dept_ID INT PRIMARY KEY
);

CREATE TABLE Employee (
    Emp_ID INT PRIMARY KEY,
    Dept_ID INT,
    FOREIGN KEY (Dept_ID) REFERENCES Department(Dept_ID)
);
```
Here, `Employee.Dept_ID` can contain `NULL`. This means the employee is not currently associated with a department.


A primary key column cannot contain `NULL` values because it uniquely identifies each record.


</details>
<!------------------------>

---

Q 29. What does SQL depends on?
- [ ] A. Realtional Algebra
- [ ] B. Tuple Relational Calculus
- [x] C. Both A and B
- [ ] D. None of the above

<details>
  <summary> <b> SQL is based on concepts from Relational Algebra and Tuple Relational Calculus. </b> </summary>

<br/>

### 1. Relational Algebra

- It is a procedural query language.
- It specifies how to retrieve data using operations.

- Important operations include:
  - **Selection (σ)**
  - **Projection (π)**
  - **Union (∪)**
  - **Set Difference (−)**
  - **Cartesian Product (×)**
  - **Join (⋈)**
    
Example: Selection retrieves rows satisfying a condition.

### 2. Tuple Relational Calculus (TRC)

- It is a non-procedural (declarative) query language.
- It specifies what data is required, not how to retrieve it.
- It uses tuple variables and logical predicates.


> **Algebra = How; Calculus = What.**


| Concept	                  | Type           |
|---------------------------|----------------|
| Relational Algebra	      | Procedural     |
| Tuple Relational Calculus	| Non-procedural |
| SQL	                      | Declarative language, influenced by both |

</details>
<!------------------------>

---

Q 30. Which of the following refers to **the number of attributes in a relation**?
- [ ] A. Row
- [x] B. Degree
- [ ] C. Column
- [ ] D. All of the above

<details>
  <summary> Attribute(Column), Tuple(Row), Degree(total no. of cols) Cardinality(total no. of rows </summary>

<br/>

In a relational database:
- Attribute: A column in a table.
- Tuple: A row in a table.
- Degree: Total number of attributes (columns) in a relation.
- Cardinality: Total number of tuples (rows) in a relation.

</details>
<!------------------------>

---

Q 31. Which of the following is not an example of DBMS?
- [ ] A. MySQL
- [ ] B. Microsoft Access
- [ ] C. IBM DB2
- [x] D. Google

<details>
  <summary> Google: Search Engine </summary>

<br/>

</details>
<!------------------------>

---

Q 32. Which of the following is correct according to the technology deployed by DBMS?
- [ ] A. Pointers are used to maintain transactional integrity and consistency
- [ ] B. Cursors are used to maintain transactional integrity and consistency
- [x] C. **Locks** are used to maintain transactional integrity and consistency
- [ ] D. Triggers are used to maintain transactional integrity and consistency

<details>
  <summary> <b> Locks </b> </summary>

<br/>

**Locks** are used by DBMS to maintain transactional integrity and consistency, particularly when multiple users or transactions access the same data concurrently.

### Locking

A lock controls access to a database resource during a transaction.

For example, two users try to update the same bank account simultaneously.
- User A starts updating the balance.
- User B also tries to update the same balance.
- A lock controls access so that conflicting operations do not interfere with each other.

Common lock types:

|  Lock	                | Purpose                                           |
|-----------------------|---------------------------------------------------|
| **Shared Lock (S)**   | Allows reading; multiple transactions can hold it |
| **Exclusive Lock (X)**| Allows modification; prevents conflicting access  |

Trigger:
```sql
CREATE TRIGGER before_insert_student
BEFORE INSERT ON Student
FOR EACH ROW
SET NEW.Name = UPPER(NEW.Name);
```
This trigger converts the student's name to uppercase before insertion.

</details>
<!------------------------>

- **Locks** -> Concurrency control, is used to control concurrent access to data.
- **Cursors** -> Row-by-row processing, is used to process query-result rows one at a time
- **Triggers** -> Automatic event execution, automatically execute in response to database events such as `INSERT`, `UPDATE`, or `DELETE`.
- **Pointers** -> Memory references, is used to refer to memory locations or data structures; not the standard concurrency-control mechanism.

---

Q 33. What is **information about data** called?
- [ ] A. Hyper data
- [ ] B. Tera data
- [ ] C. **Meta data**
- [ ] D. Relations

<details>
  <summary> Data = Actual information; Metadata = Information about that information. </summary>

<br/>

Suppose a database contains a Student table:

| Roll_No	| Name | Age |
|---------|------|-----|
| 101	    | Aman | 20  |
| 102	    |Ravi	 | 21  |
The actual student records are **data**.

Information describing the table is metadata, such as:
- Table name: `Student`
- Column names: `Roll_No`, `Name`, `Age`
- Data types: `INT`, `VARCHAR`, `INT`
- Constraints: `Primary key`, `NOT NULL`

</details>
<!------------------------>

---

Q 34. Which SQL command is used **to remove a table from a database**?
- [ ] A. `DELETE TABLE`
- [x] B. `DROP TABLE`
- [ ] C. `REMOVE TABLE`
- [ ] D. `ERASE TABLE`

<details>
  <summary> DROP = Destroy table, DELETE = Remove Rows, TRUNCATE = Empty table </summary>

<br/>

The SQL command `DROP TABLE` is used to permanently remove a table, including its structure and data, from a database.
```sql
DROP TABLE Student;
```

| Command	         | Purpose                                        |
| `DROP TABLE`	   | Removes the entire table (structure + data)    |
| `DELETE`	       | Removes selected rows or all rows              |
| `TRUNCATE TABLE` | Removes all rows but keeps the table structure |


```sql
DELETE FROM Student WHERE Roll_No = 101;
```
Removes only the row with Roll_No 101.

```sql
TRUNCATE TABLE Student;
```
Removes all rows but keeps the table.

```sql
DROP TABLE Student;
```
Removes the table itself.


</details>
<!------------------------>

---

Q 35. The SQL keyword ________ is used with wildcards.
- [X] A. `LIKE`
- [ ] B. `IN`
- [ ] C. `NOT IN`
- [ ] D. `DISTINCT`

<details>
  <summary> <b> LIKE is used with SQL Wildcards: % and _ </b> </summary>

<br/>

The SQL keyword `LIKE` is used with wildcards to search for a specified pattern in a column.

| Wildcard | Meaning                         |
|----------|---------------------------------|
| `%`	     | Matches zero or more characters |
| `_`	     | Matches exactly one character   |

Example 1: Names starting with `A`
```sql
SELECT * FROM Student WHERE Name LIKE 'A%';
-- Matches: Aman, Ankit, Ajay.
```

Example 2: Names ending with `a`
```sql
SELECT * FROM Student WHERE Name LIKE '%a';
-- Matches: Priya, Neha.
```

Example 3: Names containing exactly four characters
```sql
SELECT * FROM Student WHERE Name LIKE '____';
-- Matches: Aman, Ajay, Neha
```

Example 4: Names starts with A and ends with a
```sql
SELECT * FROM Student WHERE Name LIKE 'N%a';
-- Matches: Neha
```

> **`LIKE` = Pattern matching = Wildcards (`%`, `_`)**

  
</details>
<!------------------------>

- `IN` -> Checks whether a value matches any value in a list.
- `NOT IN` -> Checks whether a value is absent from a list.
- `DISTINCT` -> Removes duplicate values from query results.
- `LIKE` = Pattern matching = Wildcards (`%`, `_`)

---

Q 36. In a realtional database, what is a **primary key**?
- [ ] A. A key used for opening encrypted data
- [x] B. A unique identifier for a record in a table
- [ ] C. A foreign key from another table
- [ ] D. An index for sorting data

<details>
  <summary> <b> Keys in DBMS </b>  </summary>

<br/>

A key is an attribute or a set of attributes used to identify records uniquely or establish relationships between tables.

### 1. Super Key

> A super key is **any attribute or combination of attributes that can uniquely identify a record**.

Example:
| Roll_No	| Email	          | Name |
|---------|-----------------|------|
| 101	    | aman@gmail.com	| Aman |
| 102	    | ravi@gmail.com	| Ravi |

Possible super keys:
- `Roll_No`
- `Email`
- `(Roll_No, Name)`
- `(Email, Name)`

A super key may contain extra attributes.

### 2. Candidate Key

> A candidate key is **a minimal super key**. <br/>
It uniquely identifies a record without unnecessary attributes.

Example:
- `Roll_No`
- `Email`
Both can uniquely identify a student, assuming both are unique.

### 3. Primary Key

> A primary key is **the candidate key selected to identify records uniquely**.

Properties:
- Must be unique.
- Cannot contain `NULL`.
- Only one primary key constraint per table.
- Can contain multiple columns (composite primary key).

Example: `Roll_No`.

### 4. Alternate Key

> Candidate keys that **are not selected as the primary key are called alternate keys**.

Example:
- Candidate keys: `Roll_No`, `Email`
- Primary key: `Roll_No`
- Alternate key: `Email`

### 5. Foreign Key

> A foreign key is **an attribute or set of attributes that references a candidate key (commonly the primary key) in another or the same table**.

<img width="582" height="381" alt="image" src="https://github.com/user-attachments/assets/142be5d0-4fed-4953-86bb-c296ca97bce8" />

Here, `Dept_ID` in Employee references `Dept_ID` in Department.

Properties of Foreign keys:
- Foreign keys can contain duplicate values.
- They can contain `NULL` unless declared NOT NULL.
- They maintain referential integrity.

### 6. Composite Key

> A composite key **consists of two or more attributes used together to uniquely identify a record**.

Example
| Student_ID	| Course_ID	| Grade|
|-------------|-----------|------|
| 101	        | C01	      | A    |
| 101	        | C02	      | B    |
| 102	        | C01	      | A    |
Here, `(Student_ID, Course_ID)` is a composite key.

Neither column alone uniquely identifies every record, but their combination does.

### 7. Unique Key

> A `UNIQUE` constraint ensures that values in a column or combination of columns are unique.

```sql
CREATE TABLE Student (
    Roll_No INT PRIMARY KEY,
    Email VARCHAR(100) UNIQUE
);
```
`Email` cannot have duplicate values.

A primary key can't contain `NULL`, while `UNIQUE` constraints may allow `NULL` depending on the DBMS and its rules.

### 8. Surrogate Key

> A surrogate key is **an artificially generated key that has no direct business meaning**.

```sql
Student_ID INT AUTO_INCREMENT PRIMARY KEY
```
The database automatically generates IDs such as `1`, `2`, `3`, etc.


### Summary of all 8 keys

| Key	            | Main purpose                                               |
|-----------------|------------------------------------------------------------|
| `Super Key`	    | Uniquely identifies a record; may contain extra attributes |
| `Candidate Key`	| Minimal super key                                          |
| `Primary Key`	  | Selected candidate key                                     |
| `Alternate Key`	| Candidate key not selected as primary                      |
| `Foreign Key`	  | Establishes a relationship between tables                  |
| `Composite Key`	| Uses multiple attributes together                          |
| `Unique Key`	  | Prevents duplicate values                                  |
| `Surrogate Key`	| Artificially generated identifier                          |

### key Hierarchy

<img width="345" height="430" alt="image" src="https://github.com/user-attachments/assets/092f32bb-d2ec-42ec-9e1c-10fd04d637a0" />


Q1. A minimal super key is called:
- [ ] A. Primary Key
- [x] B. Candidate Key
- [ ] C. Foreign Key
- [ ] D. Composite Key

A candidate key is a minimal super key; it has no unnecessary attributes.


Q2. A candidate key not selected as the primary key is:
- [x] A. Alternate Key
- [ ] B. Foreign Key
- [ ] C. Surrogate Key
- [ ] D. Super Key

The remaining candidate keys are called alternate keys.


Q3. Which key can contain duplicate values?
- [ ] A. Primary Key
- [x] B. Foreign Key
- [ ] C. Candidate Key
- [ ] D. Alternate Key

A foreign key can repeat because multiple child records may reference the same parent record.


Q4. A key made from two or more attributes is:
- [ ] A. Surrogate Key
- [ ] B. Alternate Key
- [x] C. Composite Key
- [ ] D. Unique Key

A composite key uses multiple attributes together to identify a record.


Q5. Which key is artificially generated by the database?
- [ ] A. Foreign Key
- [x] B. Surrogate Key
- [ ] C. Candidate Key
- [ ] D. Alternate Key

A surrogate key is generated for identification and has no direct business meaning.

</details>
<!------------------------>

---

Q 37. Which of the following is known as **a set of entities of the same type that share same properties, or attribures**?
- [ ] A. Relation set
- [ ] B. Tuple
- [x] C. Entity set
- [ ] D. Entity Relation Model

<details>
  <summary> <b> Entity, Entity Set, Attribute, ER Model </b> </summary>

<br/>

| Term	        | Meaning                              |
|---------------|--------------------------------------|
| Entity	      | A real-world object(one object)      | 
| Entity Set	  | Collection of similar entities(objects) | 
| Attribute	    | Property of an entity(object)        | 
| Entity Type	  | Definition or structure of an entity |
| Relationship	| Association between entities         |
| ER Model	    | Conceptual database design model     |

</details>
<!------------------------>

---

Q 38. Which of the following expression in SQL would **calculate the square root** of 16?
- [ ] A. `POWER(16,2)`
- [x] B. **`POWER(16,0.5)`**
- [ ] C. `POWER(16,1)`
- [ ] D. `MOD(16,2)`



<details>
  <summary> <b> SQL Functions <code>POWER(), SQRT(), MOD(), ABS(), ROUND(), CEIL(),  FLOOR() </code> </b> </summary>

<br/>

In SQL, the `POWER()` function raises a number to a specified exponent.
```sql
POWER(number, exponent)
```
To calculate the square root, use an exponent of 0.5 (½)
```sql
POWER(16,0.5)
```

| Function	| Purpose	                    | Example                     |
|-----------|-----------------------------|-----------------------------|
| `POWER()`	| Raises a number to a power	| `POWER(5,2)` = `25`         |
| `SQRT()`	| Calculates square root	    | `SQRT(16)` = `4`            |
| `MOD()`	  | Returns remainder	          | `MOD(10,3)` = `1`           |
| `ABS()`	  | Returns absolute value	    | `ABS(-10)` = `10`           |
| `ROUND()`	| Rounds a number	            | `ROUND(12.567,2)` = `12.57` |
| `CEIL()`	| Rounds upward	              | `CEIL(4.2)` = `5`           |
| `FLOOR()`	| Rounds downward	            | `FLOOR(4.8)` = `4`          |

</details>
<!------------------------>

---

Q 39. To which of the following the term **DBA** referred?
- [ ] A. Data Bank Administrator
- [x] B. **Database Administrator**
- [ ] C. Data Administrator 
- [ ] D. None of the above

<details>
  <summary> <b> DBA = Database Administrator = Person responsible for database management. </b> </summary>

<br/>

> A DBA is a person responsible for managing, maintaining, securing, and ensuring the availability of an organization's databases.

### Main responsibilities of a DBA

| Responsibility	      | Explanation                               |
|-----------------------|-------------------------------------------|
| Database installation | Installs and configures DBMS software     |
| Security	            | Controls user access and permissions      |
| Backup and Recovery	  | Creates backups and restores lost data    |
| Performance tuning	  | Improves database performance             |
| Data integrity	      | Ensures accuracy and consistency of data  |
| Maintenance	          | Monitors and maintains databases          |
| User management	      | Creates users and assigns privileges      |


### 2. Important DBA commands in SQL

`GRANT`: Gives privileges to users.
```sql
GRANT SELECT ON Student TO user1;
```

`REVOKE`: Removes privileges from users.
```sql
REVOKE SELECT ON Student FROM user1;
```

### 3. Types of DBAs

- 1. **System DBA**: Installation, configuration, upgrades and maintenance.
- **Database Architect**: Designs database structures.
- 2. **Application DBA**: Supports databases used by applications.
- 3. **Performance DBA**: Monitors and optimizes database performance.

</details>
<!------------------------>

---

Q 40. While creating a table, which contraint doesn't allow insertion of duplicate values in the table?
- [x] A. `UNIQUE`
- [ ] B. `DISTINCT`
- [ ] C. `NOT NULL`
- [ ] D. `HAVING`

<details>
  <summary> <b> Constraints in SQL </b>  </summary>

<br/>

> SQL **Constraints** are rules applied to table columns to control the type of data that can be inserted, updated, or stored.

They help maintain **data accuracy, consistency, and integrity**.

### 1. `NOT NULL`

> Prevents a column from storing `NULL` values.
```sql
CREATE TABLE Student (
    Name VARCHAR(50) NOT NULL
);
```
Every student must have a name.

### 2. `UNIQUE`

> Prevents duplicate values in a column or combination of columns.
```sql
CREATE TABLE Student (
    Email VARCHAR(100) UNIQUE
);
```
Two students cannot have the same email address.

### 3. `PRIMARY KEY`

> Uniquely identifies each record. <br/>
> It combines uniqueness and `NOT NULL` requirements.
```sql
CREATE TABLE Student (
    Roll_No INT PRIMARY KEY,
    Name VARCHAR(50)
);
```

### 4. `FOREIGN KEY`

> Establishes a relationship between tables and enforces referential integrity.
```sql
CREATE TABLE Department (
    Dept_ID INT PRIMARY KEY
);

CREATE TABLE Employee (
    Emp_ID INT PRIMARY KEY,
    Dept_ID INT,
    FOREIGN KEY (Dept_ID) REFERENCES Department(Dept_ID)
);
```
`Employee.Dept_ID` must match an existing department ID or be NULL, unless the column is declared NOT NULL.

###  5. `CHECK`

> Ensures that values satisfy a specified condition.
```sql
CREATE TABLE Student (
    Age INT CHECK (Age >= 18)
);
```
Only ages 18 or above are accepted.

### 6. `DEFAULT`

> Provides a default value when no value is supplied for a column.
```sql
CREATE TABLE Student (
    City VARCHAR(30) DEFAULT 'Chandigarh'
);
```
If no city is provided, the default value is used.

### Summary of all 6 constraints

| Constraint	  | Main purpose                          |
|---------------|---------------------------------------|
| `NOT NULL`	  | Prevents `NULL` values                |
| `UNIQUE`	    | Prevents duplicate values             |
| `PRIMARY KEY`	| Uniquely identifies each row          |
| `FOREIGN KEY`	| Maintains relationships between tables|
| `CHECK`	      | Validates a condition                 |
| `DEFAULT`	    | Supplies a default value              |

### Comparison

| Comparison	                    | Key difference                                                                  |
|---------------------------------|---------------------------------------------------------------------------------|
| `PRIMARY KEY` vs `UNIQUE`	      | Primary key can't be `NULL`; `UNIQUE` can allow `NULL` depending on DBMS        |
| `UNIQUE` vs `DISTINCT`	        | `UNIQUE` is a table constraint; `DISTINCT` removes duplicates from query results|
| `CHECK` vs `DEFAULT`	          | `CHECK` validates a condition; `DEFAULT` supplies a value                       |
| `FOREIGN KEY` vs `PRIMARY KEY`	| Foreign key references a key; primary key identifies a row                      |

Q1. Which constraint prevents `NULL` values?
- [ ] A. UNIQUE
- [x] B. NOT NULL
- [ ] C. CHECK
- [ ] D. DEFAULT

`NOT NULL` requires a value in the column.


Q2. Which constraint maintains referential integrity?
- [ ] A. PRIMARY KEY
- [ ] B. CHECK
- [x] C. FOREIGN KEY
- [ ] D. DEFAULT

A foreign key ensures referenced values correspond to an existing key in the referenced table, or are `NULL` if permitted.


Q3. Which constraint validates `Age >= 18`?
- [ ] A. DEFAULT
- [ ] B. UNIQUE
- [x] C. CHECK
- [ ] D. DISTINCT

`CHECK` enforces a condition on inserted or updated values.


Q4. Which constraint automatically supplies a value when none is provided?
- [x] A. DEFAULT
- [ ] B. NOT NULL
- [ ] C. FOREIGN KEY
- [ ] D. UNIQUE

`DEFAULT` supplies the configured value when the column is omitted or DEFAULT is requested.

Q5. Which constraint uniquely identifies every row and disallows `NULL`?
- [ ] A. UNIQUE
- [x] B. PRIMARY KEY
- [ ] C. CHECK
- [ ] D. DEFAULT

A primary key enforces uniqueness and NOT NULL.

</details>
<!------------------------>

---

Q 41. **A realtion in a relational database is also known as**:
- [ ] A. a data type
- [ ] B. an attribute
- [ ] C. a schema
- [x] D. **a table**

<details>
  <summary> a relation is also known as a table </summary>

<br/>

| Relational term	  | Meaning                                             |
|-------------------|-----------------------------------------------------|
| Relation	        | Table                                               |
| Tuple	            | Row                                                 |
| Attribute	        | Column                                              |
| Domain	          | Set of permitted values for an attribute            |
| Relation Schema	  | Structure or definition of a relation               |
| Relation Instance	| Actual data stored in a relation at a particular time|

</details>
<!------------------------>

---

Q 42. Which SQL clause is used to retrieve specific rows from a table?
- [ ] A. `SEARCH`
- [ ] B. `FETCH`
- [x] C. `SELECT` 
- [ ] D. `FIND`

<details>
  <summary> SELECT + WHERE Clause </summary>

<br/>

</details>
<!------------------------>

---

Q 43. Which command is used to remove a relation from SQL?
- [x] A. `DROP table`
- [ ] B. `DELETE`
- [ ] C. `PURGE`
- [ ] D. `REMOVE`

<details>
  <summary>  DROP table </summary>

<br/>

| Command	      | Purpose                      |
|---------------|------------------------------|
| `DROP TABLE`	| Removes the entire table     |
| `DELETE`	    | Removes records from a table |
| `PURGE`	      | Used in specific DBMS contexts, not the standard SQL command for dropping a table |
| `REMOVE`	    | Not a standard SQL command for removing a table |

- `DROP` -> Removes table structure and data.
- `DELETE` -> Removes rows.
- `TRUNCATE` -> Removes all rows but retains table structure.


</details>
<!------------------------>

---

Q 44. A database Management System is a type of software:
- [ ] A. It is a type of system software
- [x] B. It is a kind of **application software**
- [ ] C. It is a kind of general software
- [ ] D. Both A and C

<details>
  <summary> DBMS is a kind of application software. </summary>

<br/>

A Database Management System (DBMS) is generally classified as application software because it performs a specific task: **`creating`, `storing`, `retrieving`, `updating`, and managing databases.**

| System Software	                               | Application Software              |
|------------------------------------------------|-----------------------------------|
| Manages computer hardware and system resources | Performs specific tasks for users |
| Operating System	                             | DBMS                              |
| Device Drivers	                               | MS Word                           |
| Language Translators	                         | MySQL, Oracle, MS Access          |

Examples of DBMS
- MySQL
- Oracle Database
- Microsoft SQL Server
- PostgreSQL
- MS Access

</details>
<!------------------------>

---

Q 45. How can you **establish a connection between PHP and MySQL**?
- [ ] A. using the `connect()` function in PHP
- [ ] B. by including a PHP Library
- [ ] C. by embedding MySQL queries directly in PHP code
- [x] D. by using the `mysqli_connect()` function in PHP

<details>
  <summary> mysqli_connect() </summary>

<br/>

PHP can establish a connection with a MySQL database using the `mysqli_connect()` function.

Syntax
```php
mysqli_connect(host, username, password, database);
```

```php
<?php
$conn = mysqli_connect(
    "localhost",
    "root",
    "",
    "school"
);

if (!$conn) {
    die("Connection failed: " . mysqli_connect_error());
}

echo "Database connected successfully!";
?>
```
| Parameter	    | Meaning                                  |
|---------------|------------------------------------------|
|  `localhost`	| MySQL server address                     |
| `root`	      | Database username                        |
| `""`	        | Database password (empty in this example)|
| `school`	    | Database name                            |

Other ways to connect PHP with MySQL

PHP supports two commonly used approaches:
1. MySQLi - MySQL Improved Extension.
2. PDO - PHP Data Objects.
```php
$pdo = new PDO(
    "mysql:host=localhost;dbname=school",
    "root",
    ""
);
```

</details>
<!------------------------>

- `mysqli_connect()` -> Establish connection.
- `mysqli_query()` -> Execute SQL query.
- `mysqli_fetch_assoc()` -> Fetch a row as an associative array.
- `mysqli_close()` -> Close connection.

---

Q 46. The term **DFD** stands for:
- [ ] A. Data File diagram
- [ ] B. Data Flow document
- [x] C. **Data Flow diagram**
- [ ] D. None of the above

<details>
  <summary> DFD = Data Flow Diagram, It explains the flow of data within a system </summary>

<br/>

A Data Flow Diagram (DFD) is a graphical representation of how data moves through an information system.

It shows:
- Where data comes from.
- How data is processed.
- Where data is stored.
- Where data goes.

In simple words: DFD explains the flow of data within a system.

<img width="612" height="502" alt="image" src="https://github.com/user-attachments/assets/de394691-8d26-4ae9-87b8-5cf1d621d236" />


### Levels of DFD

| Level	                        | Description                                     |
|-------------------------------|-------------------------------------------------|
| **Context Diagram (Level 0)**	| Shows the entire system as one process and its interaction with external entities |
| **Level 1 DFD**	              | Breaks the main system into major subprocesses  |
| **Level 2 DFD**	              | Gives further details of Level 1 processes      |

<img width="767" height="592" alt="image" src="https://github.com/user-attachments/assets/716e935e-4635-46e5-a045-e66d60a918c2" />


<img width="1037" height="720" alt="image" src="https://github.com/user-attachments/assets/4701937e-ab70-488e-81b8-1c2c469a155f" />

<img width="1027" height="767" alt="image" src="https://github.com/user-attachments/assets/4409c82c-881d-49ca-aa8d-85aaf61c0ed7" />


### Data Flow Diagram vs Flowchart

| DFD	                                    | Flowchart                      |
|-----------------------------------------|--------------------------------|
| Shows flow of data	                    | Shows flow of control or steps |
| Focuses on data movement and processing	| Focuses on sequence and logic  |
| Does not show detailed program logic	  | Can show decisions and loops   |

### Important points about DFS
- DFD is used in Structured System Analysis and Design.
- It represents the logical flow of data.
- Arrows represent data flow.
- Circles/bubbles commonly represent processes.
- Rectangles commonly represent external entities.
- Data stores are represented by two parallel lines or an open-ended rectangle, depending on notation.
- DFD does not show the timing or sequence of program execution.


</details>
<!------------------------>

---

Q 47. The term **FAT** stands for
- [ ] A. File Allocation Tree
- [x] B. File Allocation Table
- [ ] C. File Allocation Graph
- [ ] D. All of above

<details>
  <summary> FAT =  File Allocation Table </summary>

<br/>

FAT is a file system used by operating systems to organize and manage files on storage devices such as hard disks, USB drives, and memory cards.

It maintains a table that helps the operating system locate the clusters where a file's data is stored.

The FAT keeps track of this cluster sequence so the operating system can locate the complete file.

<img width="1022" height="762" alt="image" src="https://github.com/user-attachments/assets/dfd54c72-70f6-466b-9ddf-05daa501a320" />

Which of the following is a commonly used variant of the FAT file system?
- [ ] A. NTFS
- [x] B. FAT32
- [ ] C. EXT4
- [ ] D. HFS+

**FAT32** is a widely used variant of the File Allocation Table file system, commonly found on USB drives and memory cards.
- NTFS - Commonly used by Windows.
- EXT4 - Commonly used by Linux.
- HFS+ - Used by older macOS systems.

</details>
<!------------------------>

---

Q 48. Which of the following can be used **to extract or filter the data and information from the data warehouse**?
- [ ] A. Data Redundancy
- [ ] B. Data Recovery tool
- [x] C. Data Mining
- [ ] D. Both Data Recovery and Data Mining

<details>
  <summary>  <b> Data Mining </b> </summary>

<br/>

### 1. What is Data Mining?

Data Mining is the process of extracting useful patterns, relationships, trends, and meaningful information from large amounts of data.

A data warehouse stores large volumes of historical and integrated data. <br/>
Data mining helps analyze that data to discover useful insights.

Example: Suppose **a supermarket has a data warehouse containing millions of sales records**.

Using data mining, it can discover:
- Which products are frequently purchased together.
- Which months have the highest sales.
- Which customers purchase particular products.
- Which products may have higher demand in the future.

> - Data Warehouse = Stores data.
> - Data Mining = Discovers useful information from data.
> - Data Recovery = Restores lost data.

Which technique is commonly used to discover hidden patterns in large datasets?
- [ ] A. Data Encryption
- [x] B. **Data Mining**
- [ ] C. Data Backup
- [ ] D. Data Redundancy

Data Mining discovers hidden patterns, trends, and relationships in large datasets.

- Data Encryption: Protects data by converting it into an encoded form.
- Data Mining: Finds useful patterns in data.
- Data Backup: Creates copies of data for recovery.
- Data Redundancy: Refers to unnecessary duplication of data.

</details>
<!------------------------>

---

Q 49. The term **Data** refers to:
- [ ] A. the electronic representation of the information(or data)
- [ ] B. Basic information
- [ ] C. **Raw facts and figures**
- [ ] D. Both A and B

<details>
  <summary> <b> Data: raw facts and figures </b> </summary>

<br/>

Data refers to **raw facts and figures** that have not yet been processed or organized into meaningful information.

Examples:
- 85 - raw data
- Student scored 85 marks - meaningful information in context.

> **Data = Raw facts;** <br/>
> **Information = Processed and meaningful data**

</details>
<!------------------------>

---

Q 50. A **report generator** is used to:
- [ ] A. upadte file
- [ ] B. print file on paper
- [ ] C. both of the above
- [ ] D. none of the above

<details>
  <summary> A report generator is used to <b>print file on paper</b>  </summary>

<br/>

A Report Generator is a software tool used to create formatted reports from data stored in a database or other sources. These reports can be displayed on screen or printed on paper.

> **Report Generator = Creates formatted reports.**

Which tool is primarily used to create formatted reports from database records?
- [x] A. Report Generator
- [ ] B. Compiler
- [ ] C. Debugger
- [ ] D. Device Driver

A Report Generator creates formatted reports from database records.

- Report Generator - Creates reports.
- Compiler - Translates source code into machine or target code.
- Debugger - Helps find and fix program errors.
- Device Driver - Enables the operating system to communicate with hardware.

</details>
<!------------------------>

---

Q 51. In the relational table, which of the following can also be represented by the term **attribute**?
- [ ] A. Entity
- [ ] B. Row
- [x] C. **Column**
- [ ] D. Both Row and Column

<details>
  <summary> Attribute = Columns </summary>

<br/>

- Attribute = Column (Roll_No, Name, Age, Marks)
- Tuple = Row (one complete student record)
- Entity = Real-world object (Student)
- Relation = Table (Student)
- Domain = Set of permitted values

In a relational database, what is a collection of tuples called?
- [ ] A. Attribute
- [x] B. Relation
- [ ] C. Domain
- [ ] D. Degree

A relation is a table consisting of rows (tuples) and columns (attributes).

</details>
<!------------------------>

---

Q 52. ________ are organized collection of data that make them easy to access and manage.
- [ ] A. Datatype
- [x] B. **Database**
- [ ] C. Data
- [ ] D. System

<details>
  <summary> Database </summary>

<br/>

</details>
<!------------------------>

---

Q 53. What do you mean by **one-to-many relationships**
- [ ] A. Many teachers may have many classes
- [ ] B. One class may have many teachers
- [x] C. One teacher can have many classes
- [ ] D. Many classes may have many teachers

<details>
  <summary> <b> Relationships in DBMS </b> </summary>

<br/>

A relationship in DBMS describes how two or more entities are associated with each other.

For example:
- A Student enrolls in a Course.
- A Teacher teaches a Class.
- A Customer places an Order.

Relationships are an important part of the **Entity-Relationship (ER) Model**.

### Types of relationships in DBMS

**1. One-to-One (1:1)** <br/>
One record of Entity A is associated with only one record of Entity B, and vice versa.

<img width="497" height="265" alt="image" src="https://github.com/user-attachments/assets/ea457e6e-7377-4b60-b2de-a5da0f545884" />

Example: 
- One person has one passport, and each passport belongs to one person.
- One person - One Aadhaar record (simplified example).
- One country - One capital city (simplified model).

**2. One-to-Many (1:M)** <br/>
One record of Entity A can be associated with many records of Entity B.

<img width="457" height="305" alt="image" src="https://github.com/user-attachments/assets/43ce3694-e742-4b70-a5c1-1d459c1774cf" />

Example: 
- One teacher can teach many classes.
- One department -> Many employees.
- One customer -> Many orders.
- One author -> Many books.

**3. Many-to-One (M:1)** <br/>
Many records of Entity A can be associated with one record of Entity B.

<img width="1062" height="422" alt="image" src="https://github.com/user-attachments/assets/6a0a1de8-b152-429d-ab9f-e70b7226a598" />

Example: Many employees work in one department.

> Note: **Many-to-one is the reverse direction of one-to-many.**


**4. Many-to-Many (M:N)**
Many records of Entity A can be associated with many records of Entity B.

<img width="1217" height="652" alt="image" src="https://github.com/user-attachments/assets/96ced13c-ad99-4a1b-8c38-c8565b4f66eb" />

Example:
- One student can enroll in many courses.
- One course can have many students.

In a relational database, this is generally implemented using a junction table (also called a bridge or associative table).

### Quick Summary

| Relationship	     | Meaning	     | Example             |
|--------------------|---------------|---------------------|
| One-to-One (1:1)	 | One <-> One	 | Person-Passport     |
| One-to-Many (1:M)	 | One  -> Many	 | Teacher-Classes     |
| Many-to-One (M:1)	 | Many -> One	 | Employees-Department|
| Many-to-Many (M:N) | Many <-> Many | Students-Courses    |

Q1. One student can enroll in many courses, and one course can have many students. Which relationship is this?
- [ ] A. One-to-one
- [ ] B. One-to-many
- [ ] C. Many-to-one
- [x] D. Many-to-many

Many-to-many Both sides can have multiple associated records, so it is many-to-many.

Q2. Many employees work in one department. From Employee to Department, what is the relationship?
- [ ] A. One-to-one
- [ ] B. One-to-many
- [ ] C. Many-to-one
- [ ] D. Many-to-many

Many-to-one Multiple employee records are associated with one department record.

Q3. Which table is commonly used to implement a many-to-many relationship?
- [ ] A. Temporary table
- [x] B. Junction table
- [ ] C. View
- [ ] D. System table

Junction table A junction table stores the foreign keys linking the two entities.

</details>
<!------------------------>

---

Q 54. Which of the following refers to the **data about data**?
- [ ] A. Directory
- [x] B. **Metadata**
- [ ] C. Sub data
- [ ] D. Warehouse

<details>
  <summary> Data about data is meta-data </summary>

<br/>

</details>
<!------------------------>

---

Q 55. Which of the following command is a type of **Data Definition Language(DDL)**?
- [x] A. `CREATE`
- [ ] B. `UPDATE`
- [ ] C. `DELETE`
- [ ] D. `MERGE`

<details>
  <summary>  Data Definition Language(DDL): CREATE </summary>

<br/>

</details>
<!------------------------>

---

Q 56. A large computer information system maintain many different computer files. Which amongst them is called a **perpetual file**?
- [ ] A. Specialize file
- [x] B. **Master file**
- [ ] C. Log file
- [ ] D. Update file

<details>
  <summary> <b> perpetual file =  master file </b> </summary>

### What is a perpetual file?

A perpetual file is a file that is maintained continuously and updated whenever transactions or changes occur.

In traditional data-processing terminology, a Master File is often called a perpetual file because it stores relatively permanent records and is updated periodically or continuously.

- Master file: stores ongoing, relatively permanent records.
- Log file: Records events, transactions, or system activities.
- Update file: Contains changes or transactions used to update the master file.

| File	                      | Purpose                            |
|-----------------------------|------------------------------------|
| **Master file**	            | Maintains current, ongoing records |
| **Transaction/Update file**	| Contains changes to be applied     |
| **Log file**	              | Records events or activities       |


Which file generally contains transaction details used to update a master file?
- [ ] A. Master file
- [x] B. Transaction file
- [ ] C. Backup file
- [ ] D. Program file

A Transaction File contains new or changed transaction records that are used to update the Master File.

</details>
<!------------------------>
