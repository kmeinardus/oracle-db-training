
# Database Foundations 1-1: Introduction to Databases

## What I Learned
- Databases are tools designed to organize, store, and manage data efficiently.
- Various database types, such as Hierarchical, Network, and Relational, are suited to different data structures and uses.
- Databases streamline data management, making it easier to access and update information.

# Database Foundations 1-2: Introduction to Database

## What I Learned
- **Data** - collected facts about a topic or item
- **Information** - the result of coombing, comparing, and performing calculations on data
- Data in, information out
- **Database** - organized collection of data put together as a unit. Place where data is stored and retrieved, managed by a DBA (Database Administrator)
#### Relational Databases
-Stores information in tables with rows and columns
  - **Table** - collection of records
  - **Row** - called a record (or instinct)
  - **Column** - called a field (or attribute)
#### Database Management System
- Software that controls the storage, organization, and retrieval of data
  - **Elements**
    - *Memory and storage management* (kernel code)
    - *Data dictionary* - repository of metadata
    - *Query language* - enables applications to access the data
#### Key Computing terms
  - **Hardware** - physical parts of a computer
  - **Software** - instructions to tell hardware what to do 
  - **Operating system** - software that directly controls the hardware (ex Windows)
  - **Application** - performs specific task
  - **Client** - workstation used by end users
  - **Server** - accepts work requests from clients requiring more power. Retrieves data from database, converts into useful info, sends info back to client
#### Cloud Computing
   - Internet based processing
   - Three main Categories:
     - **IaaS** - Allows you to rent cloud based servers, storage, operating systems, etc
     - **PaaS** - Gives access to an online environment for developing and testing software without any setup or management cod
     - **Saas** - Delivers software direct from the internet. Users usually access it through a web browser
    
# Practice for Database Foundations 1-2: Introduction to Database

## Task 1 - Student on-line information and registration system
### **Important Data**
  - **Student Data**
    - Student Name
    - Student ID
    - Student DOB
    - Enrollment Status 
  - **Course Data**  
    - Course Name
    - Course Department
    - Course ID
    - Course Dates
    - Teacher Name
    

## Task 2 - Library management system
### **Important Data**
  - **Member Data**
    - Member Name
    - Member ID
    - Contact Information
    - Billing Address
  - **Book Data**  
    - Book Title
    - Book Author
    - Book ID
  - **Staff Data**
    - Staff Name
    - Staff ID
    - Staff Job Description 
  - **Loan Data**  
    - Loan Start Date
    - Loan End Date
    - Loan ID
    - Loan Late Cost
   
# Practice for Database Foundations 1-3: Types of Database Models

## Exercise 1: Identify the Database Models

### Task 1a.
  - ***Hierarchical Model***
    - Data is organized in a tree-like structure
    - The data is stored as records that are connected to one
another through links
### Task 1b. 
  - ***Network Model***
    - A database model that can be regarded as a flexible way of representing objects and their relationships
    - A network database comprised of a collection of records connected to one another through links. (Boxes = Fields, Lines = Links)
    - Each record is a collection of fields, each of which contains only one data value
    - A link is an association between two records
### Task 1c.
  - ***Object-Oriented Model***
    - A entity is modeled as an object
    - Every object has a state (the set of values for the attributes of the object) and a behavior (the set of methods that operate on the state of the object)
    - The relationship between the objects is through sharing of access
    - An object must belong to only one class as an instance of that class
    - You can derive a new class (subclass) from an existing class (superclass)
### Task 1d.
  - ***Relational Model***
    - Data is represented as a collection of tables
    - Each column represents attributes that belong to the table
    - Each row represents an instance of the table
    - Each table is the visual representation of columns and rows
    - Every table has a field or a set of fields that uniquely dentifies the row
### Task 1e.
  - ***Flat File Model***
    - A flat file database is a database designed around a single table
    - Flat file databases are generally in plain-text form, where each line holds only one record.
    - The fields in the record are separated with delimiters, such as tabs and commas.



# Practice for Database Foundations 1-4: Business Requirements
 ## Business Rules and Constraints

### 1. LibBook Digital Library

  #### Business Rules:
  1. **Membership Types**:
     - **Student Membership**: Free of charge.
     - **Individual Membership**: Fee required; includes basic privileges.
     - **Faculty Membership**: May be introduced later; fee required.
     - **Corporate Membership**: Fee required; includes additional privileges.

  2. **Membership Changes**:
     - Membership type can be changed only if sufficient justification is provided.

  #### Constraints:
  1. **Membership Fee**:
     - **Corporate Membership**: Must have a fee.
     - **Individual Membership**: Must have a fee.
     - **Student Membership**: Must be free of charge.
  
  2. **Membership Change Justification**:
     - Any change in membership type must be supported by sufficient justification.

  ### 2. Star Care Hospital

  #### Business Rules:
  1. **Doctor Identification**:
     - Every doctor is assigned a unique ID that starts with "DC".
  
  2. **Experience Requirement**:
     - Doctors must have a minimum of seven years of working experience.
  
  3. **Patient Registration**:
     - Every patient must register with the hospital on their first visit.
  
  4. **Patient Identification**:
     - A unique patient number starting with "PT" is assigned upon registration.
  
  #### Constraints:
  1. **Doctor ID Format**:
     - IDs for doctors must start with "DC".
  
  2. **Experience**:
     - All doctors must have at least seven years of experience, with no exceptions.
  
  3. **Patient Number Format**:
     - Patient numbers must start with "PT".
  
  4. **Registration Requirement**:
     - Patients must complete the registration process on their first visit.
    

# Practice for Database Foundations 2-1 : Relational Databases

## Exercise 1: Analyze the features of a Relational Database

#### 1. Identify the Possible Tables and Associated Fields

**Scenario: Book.com**

Book.com is an online virtual store where customers can browse and select books. Based on this scenario, the database could include the following tables and fields:

- **Books**
  - **Fields**: Book ID, Title, ISBN, Year, Price, Author ID, Publisher ID

- **Authors**
  - **Fields**: Author ID , Name, Address, Homepage URL

- **Publishers**
  - **Fields**: Publisher ID , Name, Address, Phone Number, Website URL

- **Warehouses**
  - **Fields**: Warehouse ID , Code, Address, Phone Number

- **Stock**
  - **Fields**: Stock ID, Warehouse ID, Book ID, Number of Copies

- **Customers**
  - **Fields**: Customer ID, Name, Address, Email ID, Phone Number

- **Shopping_Carts**
  - **Fields**: Shopping Cart ID, Customer ID, Cart Item ID

- **Cart_Items**
  - **Fields**: Cart Item ID, Shopping Cart ID, Book ID, Quantity

- **Orders**
  - **Fields**: Order ID, Customer ID, Billing Address, Shipping Address, Shipping Option, Payment Info, Email Notification

#### 2. Identify the Tables and Associated Fields

**Scenario: ABC Ltd Sales and Stock Control**

ABC Ltd is setting up a relational database system for managing sales and stock control. The database could include the following tables and fields:

- **Customers**
  - **Fields**: Customer ID, Name, Address, Email ID, Phone Number

- **Orders**
  - **Fields**: Order ID, Customer ID, Order Date, Status

- **Order_Items**
  - **Fields**: Order Item ID, Order ID, Product ID, Quantity, Unit Price

- **Products**
  - **Fields**: Product ID, Name, Description, Preferred Supplier ID, Quantity in Stock, Reorder Level

- **Suppliers**
  - **Fields**: Supplier ID, Name, Address, Phone Number

- **Invoices**
  - **Fields**: Invoice ID, Order ID, Invoice Date, Total Amount

- **Payments**
  - **Fields**: Payment ID, Customer ID, Invoice ID, Payment Amount, Payment Date


    
# Practice for Database Foundations 2-2: Conceptual and Physical Data Models
### 1. Provide five reasons for creating a conceptual data model.

1. **Captures Business Requirements**: A conceptual data model captures the functional and informational needs of a business, ensuring that the model reflects both current and potential future needs.

2. **High-Level Understanding**: It provides a high-level view of the data and its relationships without delving into implementation details, making it easier for stakeholders to understand the system's requirements and design.

3. **Entity Identification**: Identifies important entities (objects that will become tables in the database) and the relationships among them, which is crucial for understanding how different parts of the business interact.

4. **Focus on Business Needs**: Addresses what is conceptually ideal for the business without being constrained by physical or technical limitations, allowing for a clearer vision of what the data model should achieve.

5. **Foundation for Further Models**: Serves as the basis for creating more detailed logical and physical data models, ensuring that the foundational business requirements are correctly translated into more technical specifications.

### 2. List two examples of conceptual models and physical models.

#### Examples of Conceptual Models

1. **Entity-Relationship Diagram (ERD)**: A high-level diagram that illustrates entities and their relationships without specifying details like attributes or primary keys.

2. **Business Process Model**: A diagram or model that shows how different business processes interact with data entities, focusing on the flow of information rather than the technical implementation.

#### Examples of Physical Models

1. **Relational Schema**: A detailed representation of tables, columns, primary keys, and foreign keys that defines how data is physically stored and accessed in a relational database.

2. **Database Implementation Script**: SQL scripts or DDL (Data Definition Language) statements used to create tables, indexes, views, and other database objects in a specific database management system (DBMS).

# Practice for Database Foundations2-3 : Entities and Attributes


## Academic Database (School Management System) ERD

## Entities and Attributes

### Identified Entities

1. **School/University**
2. **Department**
3. **Course**
4. **Student**
5. **Faculty**
6. **Parent Information**
7. **Attendance**
8. **Exam**
9. **Academic Session**

### Entity Relationship Diagram (ERD) Structure

## Exercise 2: Identify and Add Attributes

### Attributes and Optionality

| Entity               | Attribute                 | Optionality |
|---------------------|---------------------------|-------------|
| **School/University** | School ID                 | *           |
|                     | Name                      | *           |
|                     | Location                  | °           |
| **Department**      | Department ID             | *           |
|                     | Name                      | *           |
|                     | Head of Department        | °           |
| **Course**          | Course ID                 | *           |
|                     | Title                     | *           |
|                     | Credits                   | *           |
|                     | Department ID             | *           |
| **Student**         | Student ID                | *           |
|                     | Name                      | *           |
|                     | Date of Birth             | *           |
|                     | Email                     | °           |
|                     | Phone Number              | °           |
| **Faculty**         | Faculty ID                | *           |
|                     | Name                      | *           |
|                     | Department ID             | *           |
|                     | Email                     | °           |
|                     | Phone Number              | °           |
| **Parent Information** | Parent ID                 | *           |
|                     | Student ID                | *           |
|                     | Name                      | *           |
|                     | Email                     | °           |
|                     | Phone Number              | °           |
| **Attendance**      | Attendance ID             | *           |
|                     | Student ID                | *           |
|                     | Course ID                 | *           |
|                     | Attendance Date           | *           |
|                     | Status                    | *           |
| **Exam**            | Exam ID                   | *           |
|                     | Course ID                 | *           |
|                     | Exam Date                 | *           |
|                     | Total Marks               | *           |
| **Academic Session** | Session ID                | *           |
|                     | Year                      | *           |
|                     | Start Date                | *           |
|                     | End Date                  | *           |




# Practice for Database Foundations 2-4 : Unique Identifiers

## Database Foundations: Unique Identifiers

### Exercise 1: Identify the Unique Identifier and Corresponding Primary Keys

#### 1. Unique Identifier for a Song
To find a particular song in a whole collection, a unique identifier could be:
- **Song ID** (a unique number or code assigned to each song).

#### 2. Unique Identifiers for Students
To identify a single student from the classroom, the following attributes could serve as unique identifiers:
- **Student ID** 
- A combination of **first name**, **last name**, and potentially **date of birth** could also serve as unique identifiers, but it’s less reliable than a single unique ID.

#### 3. Unique Identifiers for Entities
- **Entity: STUDENT**
- **Attributes:** student ID, first name, last name, address
  - **Unique Identifier:** Student ID

- **Entity: MOVIE**
- **Attributes:** title, date released, producer, director
  - **Unique Identifier:** Movie ID or A combination of **title** and **date released** 

- **Entity: LOCKER**
  - **Attributes:** size, location, number
  - **Unique Identifier:** number

### Exercise 2: Identify the Unique Identifiers and Add to the ERD

#### Unique Identifiers for the Academic Database

1. **Entities and Unique Identifiers:**

| Entity               | Unique Identifier      |
|---------------------|------------------------|
| School/University    | School ID              |
| Department          | Department ID          |
| Course              | Course ID              |
| Student             | Student ID             |
| Faculty             | Faculty ID             |
| Parent Information   | Parent ID              |
| Attendance          | Attendance ID          |
| Exam                | Exam ID                |
| Academic Session    | Session ID             |

#### Candidate Unique Identifiers


| Entity               | Candidate Unique Identifiers                            |
|---------------------|-------------------------------------------------------|
| **Student**         | - Student ID (unique number assigned to each student) <br> - Email Address (assuming uniqueness) <br> - First Name + Last Name + Date of Birth (less reliable) |
| **Movie**           | - Movie ID (unique identifier for each movie) <br> - Title + Date Released (can be unique for specific films) |
| **Locker**          | - Locker Number (typically unique within a location) <br> - Size + Location (could be unique depending on context) |
| **Course**          | - Course ID (unique identifier for each course) <br> - Title + Department (may be unique within a specific department) |
| **Faculty**         | - Faculty ID (unique identifier for each faculty member) <br> - Email Address (assuming uniqueness) |
| **Parent Information** | - Parent ID (unique identifier for each parent) <br> - Combination of Student ID + Parent Name (could be unique) |
| **Attendance**      | - Attendance ID (unique identifier for each attendance record) <br> - Combination of Student ID + Course ID + Date (may be unique) |
| **Exam**            | - Exam ID (unique identifier for each exam) <br> - Course ID + Exam Date (may be unique for specific courses) |
| **Academic Session** | - Session ID (unique identifier for each academic session) <br> - Year + Term (may be unique depending on institution) |


# Practice for Database Foundations 2-5 : Relationships

## Exercise 1: Identify relationships from the ERD

### Tasks
1. Read the relationship. Which text corresponds to the diagram?
   - **Answer:** b. Each EMPLOYEE must be assigned to one and only one DEPARTMENT. Each DEPARTMENT must be responsible for one or more EMPLOYEEs.

2. Read each relationship in the model below. For each relationship, write the ERD statement and your comments. Use your knowledge of normal people and towns in your comments.
   - **Answer:**
       - each person must be born in one or more towns
       - many people must be living in a town
       - a town bay be the hometowm of many people
       - many people may visit many towns
       - Many towns must be visited by many people
       - a person may be mayer of a town
       - a town may be goverend by a person 


# Practice for Database Foundations 2-6 : Entity Relationship Modeling (ERDs)
Practices

## Exercise 1: Identify the components in the ERD

### Scenario 1: Company Departments and Employees

#### 1. Entities and Attributes
- **Entities:**
  - Department
  - Employee
  - Project
- **Attributes:**
  - **Department:**
    - Department Name 
    - Supervisor 
    - Department Number 
  - **Employee:**
    - Employee Name 
    - Employee Number 
  - **Project:**
    - Project Name 
    - Project Number 

### Scenario 2: Salon with Hairstylists and Clients

#### 1. Entities and Attributes
- **Entities:**
  - Hairstylist
  - Client
- **Attributes:**
  - **Hairstylist:**
    - First Name (Mandatory)
    - Last Name (Mandatory)
    - Address (Optional)
    - Phone Number (Optional)
    - Social Security Number (UID, Mandatory)
  - **Client:**
    - First Name (Mandatory)
    - Last Name (Mandator, optional for walk ins)
    - Phone Number (Mandatory, optional for walk ins)
    - Client ID (UID, Mandatory)
    - Hairstylist Preference (Optional)

#### 2. ERD Relationships:
- **Hairstylist ↔ Client:**
- A hairstylist may see multiple clients
- a client may be seen by only one hairstylists.

### Scenario 3: Teachers, Courses, and Classes

#### 1. Entities and Attributes
- **Entities:**
  - Teacher
  - Course
  - Class
- **Attributes:**
  - **Teacher:**
    - First Name 
    - Last Name 
    - Address 
    - Phone Number 
    - Email Address 
  - **Course:**
    - Course Code 
    - Course Name 
  - **Class:**
    - Class ID 
    - Day 
    - Time 
    - Classroom 

#### 2. ERD Relationships:
- **Teacher ↔ Class:**
  -  A teacher can teach one or more classes
  -  Each class is taught by one teacher.
- **Course ↔ Class:**
  - Each course may be taught in multiple classes
  - Each class is associated with one course.



# Practice for

# Practice for


# Practice for


# Practice for

Practice for
  
     
