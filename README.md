## Data 
Any facts and figures about entity
## Information
Any data which helps us , which have certain meaning (eg-roll no, account_id)
## DataBase
A structured collection of data
# Database Management system(DBMS)
the System which manages the database , like retriving the data
## File system Vs Dbms
![img](https://github.com/user-attachments/assets/3dda83e9-0433-440b-b79a-9da60c23bcfb)

---
## View Level Of Database
- **Physical Level** :
  The internal schema details data storage and access on hardware (jaisa asliyat mein database hota hai)
- **Logical Level** :
   this level showcases data as entity sets and their relationships ( ye structure table ke form mein dikhta hai )
- **View Level** :
   displaying only a portion of the entire database focusing on user-interest areas (keval view level aisa level hai jo user dekh paata hai )
---
# Data Independence
 the capacity to change the schema at one level of a database system without having to change the schema at the next higher level
## Types
- **Physical level** :  the capacity to change the schema at one level of a database system without having to change the schema at the next higher level ( ek aisa independence , jahan par aap physical level ko change kar dete ho bina logical level ko distrub kiye)
- **Logical level** : Logical data independence is the ability to modify the conceptual schema without having to change the external schemas ( logical level ko change karte hai , modify karte hai bina view level ko change kiye)

## Instance
The collection of information stored in the database at a specific moment ( jo content hai table ke andar , vahi instance hai )
## Schema
The database schema refers to the overall design of the database, illustrating the logical structure and organization of data ( blueprint ya structure of table)
---
## Types of Database
- **Commercial Database** : baiscally aisa database jiska use mainly hum buisness sector mein use karte hai .
- **Multimedia Database** : ek aisa database jo text , audios ,videos , images ko store karta hai .
- **temporal databse** : ek aisa database jo aise data ko store karta hai , jo time ke sath change ho raha hota hai ( eg: stock trading)
- **Geological Database** : database jo geographical database ko store karta hai ..
---
## DBMS Architecture
isko padhke pass zaroor hoskte ho exam mein , but not really important.

![Screenshot 2025-01-12 165437](https://github.com/user-attachments/assets/a0299bdc-58be-4e24-837a-84bdd65b642d)
---
# ER Diagram 
## entity
 An entity is a thing or an object in the real world that is distinguishable from other object based on the values of the attributes ( har chiz jo rectangle mein hai )
 
 ![Screenshot 2025-01-12 165702](https://github.com/user-attachments/assets/948753ab-1098-47b3-adbd-11cebbf5ffe4)

## attributes
 Attributes are the units defines and describe properties and characteristics of entities ( har vo chiz jo oval ya ellipse ke andar likhi gyi hai )

![Screenshot 2025-01-12 170006](https://github.com/user-attachments/assets/07af381d-24d7-49f8-93b0-21a8e690a451)

## Types Of Attributes
- **Single valued** : Attributes having single value at any instance of time for an entity. E.g. Aadhar no, dob
- **Mutivalued** : Attributes which can have more than one value for an entity at same time.  E.g. - Phone no, email, address
- **Simple** : Attributes which cannot be divided further into sub parts. E.g. Ag
- **Composite** : Attributes which can be further divided into sub parts, as simple attributes

![Screenshot 2025-01-12 170342](https://github.com/user-attachments/assets/0131629a-a3ec-40f7-b825-353a13d48af0)
- **Stored** :Main attributes whose value is permanently stored in database. E.g. date_of_birth
- **Derived** :The value of these types of attributes can be derived from values of other Attributes. E.g. - Age attribute can be derived from date_of_birth and Date attribute

![Screenshot 2025-01-12 170807](https://github.com/user-attachments/assets/951723cb-7966-49a1-8577-c17ab120127b)
- **Descriptive** :Attribute of relationship is called descriptive attribute ( basically, which is in a relationship)

![image](https://github.com/user-attachments/assets/77587f98-dc80-4002-b360-6b487a32a5c4)
---
## Relationship
Do ya Do se zyada entities ke beech mein relationship 

![image](https://github.com/user-attachments/assets/82792f19-bc09-465e-9c67-71e31694d485)

## Degree Of A relationship
## Five Degrees Are There
- **Unary** : One single entity set participate in a Relationship ( ye entity bilkul thanos ki tarah hai , ye poora brahmand akeley hi jeet lenge 😂)

![Screenshot 2025-01-12 171702](https://github.com/user-attachments/assets/39996184-33c7-4b87-84b5-04a2f30fe0b7)
- **Binary** : Two entity sets participate in a Relationship. It is most common Relationship (eg - tum or tumhari bandi ki relationship )
- **Ternary** :  When three entities participate in a Relationship

![Screenshot 2025-01-12 172203](https://github.com/user-attachments/assets/c7a719f2-3388-45da-acfc-74ebf047e584)
- **Quaternary** :  When four entities participate in a Relationship

![Screenshot 2025-01-12 172452](https://github.com/user-attachments/assets/022424aa-b936-4115-bfd0-7d862de71ab6)
- **N-ary** :  where n number of entity set are associated
## Mapping Cardanilites
## four types :
- **one to one** : An entity in A is associated with at most one entity in B, and an entity in B is associated with at most one entity in A
- **one to many** : An entity in A is associated with any number (zero or more) of entities in B. An entity in B, however, can be associated with at most one entity in A
- **many to one** :  An entity in A is associated with at most one entity in B. An entity in B, however, can be associated with any number (zero or more) of entities in A
- **many to many** :  An entity in A is associated with any number (zero or more) of entities in B, and an entity in B is associated with any number (zero or more) of entities in A

![Screenshot 2025-01-12 173025](https://github.com/user-attachments/assets/44e6347d-c00a-4d59-b762-7f8637f3aefa)
we can use same ER diagram in all cardinalities (☝️)
## Strong And Weak Entity Set
## strong : 
An entity set is called strong entity set, if it has a primary key, all the tuples in the set are distinguishable by that key.
## Weak :
An entity set that does not process sufficient attributes to form a primary key is called a weak entity set ( basically jiske pass primary key nhi hai )
## Generalization 
Involves merging two lower-level entities to create a higher-level entity.  A bottom-up approach that builds complexity from simpler components.

![Screenshot 2025-01-12 173706](https://github.com/user-attachments/assets/97ec1960-61ae-4b8a-9221-02e7cf0b0097)
## Specialization 
A process where a higher-level entity is broken down into more specific, lower level entities ,This top-down approach delineates complexity into simpler components

![Screenshot 2025-01-12 173844](https://github.com/user-attachments/assets/0fc5b8e3-49d8-4c84-aaba-d82c023a5163)
## Aggregation
 A concept wherein relationships are abstracted to form higher-level entities, enabling a more organized representation of complex relationships

![Screenshot 2025-01-12 174021](https://github.com/user-attachments/assets/684a55da-667e-4d1b-a6e6-dbd5ec2dba3e)
---
# RDBMS(Relational Database Mangement System)
## Basics of RDBMS
- Har column jisko hamlog attributee bolte hai , use ab Domain ,arity bhi bol skte hai .
- Har row jise hum log tuple bhi bolte hai use ab hum cardinaltiy bhi bol skte hai .

![Screenshot 2025-01-12 174753](https://github.com/user-attachments/assets/a75ba9ea-af15-4a7c-99ee-1818238e4b67)
## Problems in Relational Database
- **Insertion Anomalies** : This occurs when it is difficult to add new data to a database without including redundant or irrelevant data
- **Deletion Anomalies** : This occurs when deleting a piece of data unintentionally leads to the loss of additional important data
- **Updation Anomalies** : This occurs when updating data leads to inconsistencies because the same data is stored in multiple places, and all instances are not updated
---
# Purpose of Normalization
- isi vajah se normalization hmlog padhenge taaki jo ye dikkat aarahi hai during insertion , deletion ,updation vo naa aaye ( anomalies : dikkat 😒)
- Normalization may be simply defined as refinement process,  creating tables and establishing relationships between those tables according to rules designed both to protect data and make the database more flexible
- 1NF<<<2NF<<<3NF<<<BCNF
- For normalization we need to use some tools , named as `functional dependency`
- iska aisa kuch khaas use nhi hai , as a skill but exam ke hissab se important hai.

# 1NF
- 1NF is the initial step of database normalization
- Atomic Values: Each cell in a table contains indivisible, atomic values. Means a Relation should not contain any multivalued or composite attributes
# 2NF
- R should be in 1 NF ( R is nothing but relation)
- R should not contain any Partial dependency 
# 3NF
- R should be in 2NF
- It must not contain any transitive dependency
# BCNF(BOYCE CODD NORMAL FORM)
-  α →β 
- α must be a super key
# 4NF
- It is in BCNF
- There must not exist any non-trivial multivalued dependency

![img 2](https://github.com/user-attachments/assets/77b3601c-2562-4303-ba03-5de0c0e73a72)
## Armstrong Axioms
- These are inference rules which used to infer all the functional dependencies in a relational database

![img  3](https://github.com/user-attachments/assets/550113db-2a66-48d4-92f9-690b5e3ef68d)
---
# Key 
## Super Key : 
Set of attributes using which we can identify each tuple uniquely is called Super key
## Candidate Key :
Minimal set of attributes using which we can identify each tuple uniquely is called Candidate key
## Primary Key :
A key which is of unique values and also not null 
## Foreign Key :
A foreign key is a column or group of columns in a relational database table that refers the primary key of the same table or some other table to represent relationship
## Composite key :
Composite key is a key composed of more than one column
## Secondary Key :
Secondary key is a key used to speed up the search and retrieval contrary to primary key, a secondary key does not necessary contain unique values

# LOSSY
Because of a normalization a table is Decomposed into two or more tables but ,jab ham unhe vapas jodte hai to hamar data pehle jaisa nhi rehta vo loss ho jaata hai 

---
# Query Language
It is nothing but a language which we use for retrieval , for retrieving the data , for updating , inserting etc..
## two things : 
- relational algebra
- relational calculus
- both are necessary condition for sql
## basic operations 

![Screenshot 2025-01-12 185026](https://github.com/user-attachments/assets/b78850a8-f71b-44a8-9ec8-6ad01d1a2aed)
![image](https://github.com/user-attachments/assets/34670821-8b76-43d1-85f6-cdc0e717a99f)

# SQL (Structure Query Language)
Structured Query Language is a domain-specific language (not general purpose) used in programming and design for managing data held in a relational database management system
## Classification Of Database Language
- **DDL(Data defintioon language)** :  DDL is set of SQL commands used to create, modify and delete database structures but not data.
 CREATE, ALTER, DROP, TRUNCATE, COMMENT, GRANT, REVOKE
- **DML(Data Manipulation Language)** :  A DML is a language that enables users to access or manipulates data as organized by the appropriate data model
INSERT, UPDATE, DELETE
- **DCL(Data Control Language)** : It is the component of SQL statement that control access to data and to the database
GRANT and REVOKE
- **DQL(Data Query Language)** : It is the component of SQL statement that allows getting data from the database and imposing ordering upon it
 SELECT
- **VDL(View Definition Language)** : VDL is used to specify user views and their mapping to conceptual schema
## for creating table:
```SQL
 CREATE TABLE Students (
 StudentID INT PRIMARY KEY,
 FirstName VARCHAR(50),
 LastName VARCHAR(50),
 Age INT,
 Email VARCHAR(100)
 );
```
## for inserting in tables
```SQL
 INSERT INTO Students (StudentID, FirstName, LastName, Age)
 VALUES 
(1, 'kushagra', 'Shukla', 20),
(2, 'Niharika', 'Singh', 22),
(3, 'Niharika', 'Shukla', 19)
```
## Deleting From Tables
```SQL
 DELETE FROM Students
 WHERE StudentID = 1;
```
# Joins
A Join allows you to combine rows from two or more tables based on a related column between them
## Types
- Inner Join
- EquiiJoin
- Natural Join
- Self Join
- Outer Join
  > left join
  > right join
  > full outer join
## Natural Join
A Natural Join automatically joins two tables based on columns with the same name and data type in both tables
## Self Join
A Self Join is when a table is joined with itself. This is useful when you want to compare rows within the same table
## Equii Join
An Equijoin uses the equality (=) operator to match rows between tables. It joins tables based on a condition that compares columns with equal values
## Inner Join
An Inner Join returns rows where there is a match in both tables. If there are no matches, no rows are returned
## left outer Join
The left outer join (left join) preserves tuples only in the relation named before (to the left of) the left outer join operation
## Right Outer Join
The right outer join (right join) preserves tuples only in the relation named after (to the right of) the right outer join operation
## Full Outer Join
The full outer join preserves tuples in both relations

---
## Alter VS Update
- **Alter** :
  . Used to change table structure
  . work on structure of table
  . eg: add a column,remove a column
- **Update** :
    . used to update data , modifies it
    . works on data stored in table
    . eg: update name,update salary
## Delete Vs Drop Vs Truncate
- **Delete**
  . used to delete any row or column in a table
  . but preserves table structure
- **Drop**
  . used to drop any table including its structure
  . removes data as well as structure
- **Truncate**
  . delete all rows from table
  . table structure is preserved
## Agreggate Functions
Nothing but functions which helps in Sql
- **Min()** :
```SQL
SELECT MIN(salary) FROM emp;
```
- **max()** :
```SQL
SELECT MAX(salary) FROM emp;
```
- **avg()** :
```SQL
SELECT AVG(salary) FROM emp;
```
- **sum()** :
```SQL
SELECT SUM(Amount) AS TotalSales
FROM Sales;
```
- **count()** :
```SQL
 Select count(*)from account;
```
- **ordering()** :
```SQL
Select distinct branch_name
 from branch 
where branch_city = 'Delhi’ 
Order by branch_name aesc;
```
- **string()** :
```SQL
 Select branch_name
 from branch 
where branch_name like ‘_ _ _ _ _ _’;
```
- **Group()** :
```SQL
 Select branch_name, avg(balance)
 from account 
Group by branch_name;
```

Thankyou for Reading :)

![img 4](https://github.com/user-attachments/assets/05fc2181-a71b-4716-82fc-692de3ccd84e)


  





  
