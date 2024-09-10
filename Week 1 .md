
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
    
  
  
     
