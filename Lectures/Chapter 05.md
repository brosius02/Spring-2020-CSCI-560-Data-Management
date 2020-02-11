# CSCI 560 Spring 2020
# Dr. Ning Zhang
# Chapter 05: Data Modeling and Design

# 1. Introduction

![28](../Resources/figure28.png)

+ Six most commonly used schemas
  - Relational
  - Dimensional
  - Object-Oriented
  - Fact-Based
  - Time-Based
  - NoSQL
+ Three levels
  - Conceptual
  - Logical
  - Physical
  - More details [here](https://www.guru99.com/data-modelling-conceptual-logical.html)
## 1.1 Business Drivers
+ Data models are critical to effective management of data, they
  - Provide a common vocabulary around data
  - Capture and document explicit knowledge about an organization's data and system
  - Serve as a primary communications tool during projects
  - Provide the starting point for customization, integration, or even replacement of an application
## 1.2 Goals and Principles
+ Confirming and documenting understanding of different perspectives, which facilitates:
  - Formalization: concise definition of data structure and relationships
  - Scope definition: boundaries for data context and implementation of purchased application packages, projects, initiaties, or existing systems
  - Knowledge retention/documentation: corporate memory regarding a system of project by capturing knowledge in an explicit form.
## 1.3 Essential Concepts
### 1.3.1 Data Modeling vs. Data Models
+ Data modeling
  - the understanding of the organizational data
+ Data models
  - a data model contains a set of symbols with text labels that attempts visually to represent data requirements as comminicated to the data modeler.
### 1.3.2 Types of Data
+ Category informaton
  - customers classified by market categories or business sectors
  - products classified by color, model
  - orders classified by whether they are open or closed

+ Resource information(reference data)
  - basic profile of resources needed conduct operational processes
    + product
    + customer
    + supplier
    + facility
    + organization
    + account
+ Business event information(transactional business data)
  - Data created while operational process such as
    + customer order
    + supplier invoice
    + cash withdrawal
    + business meeting
+ Detail transaction information(Big Data)
  - produced through point-of-sale systems
    + social media systems
    + other internet interactions
    + sensors in machines
    + personal devices
### 1.3.3 Data Modeling Components
+ Entities
+ Relationships
+ Attributes
+ Domains

#### Entities
+ An entity is a thing about which an organization collects information.
+ An entity can be thought of as an answer to a fundamental question
  - who
  - what
  - when
  - where
  - why
  - how
  
  
|Category|Definition|Examples|
|----|----|----|
|Who|Who is important to the business?|Employee, Patient, Player, Suspect, Customer, Vendor, Student, Passenger, Competitor, Author|
|What|What the organization makes or what service it provides? What is important to the business?|Product,Service, Raw Material, Finished Good, Course, Song, Photograph, Book|
|When|When is the business in operation?|Time, Date, Month, Quater, Year, Calendar, Semester, Fiscal Period, Minute, Department Time|
|Where|Where is business conducted?|Mailing Address, Distribution Point, Website URL, IP address|
|Why|Why is the business in business?|Order, Return, Complaint, Withdrawal, Deposit, Compliment, Inquiry, Trade, Claim|
|How|How do we know that an event occur?|Invoice, Contract, Agreement, Account, Purchase Order, Speeding Ticket, Packing Slip, Trade Confirmation|
|Measurement|Count, sum, etc. of other categories|Sales, Item Count, Payments, Balance|

+ Entity Aliases

|Scheme|Entity Alias|
|---|---|
|Common Use|Entity Type|
|Relational|Entity|
|Dimensional|dimension/fact table|
|object-oriented|class/object|
|time-based|hub/satellite/link|
|NoSQL|document/node|

|level of detail|Entity Alias|
|---|---|
|Conceptual|concept/term|
|Logical|entity or others depending on scheme|
|Physical|table|

+ Graphic Representation of Entities
  - Rectangles (or rectangles with round endges) with their names inside
  
  ![29](../Resources/figure29.png)

+ Definition of Entities
  - **they are core Metadata**
  - characteristics
    + Clarity
    + Accuracy
    + Completeness


#### Relationships
A relationship captures 
  - the high-level interactions between conceptual entities
  - the detailed interactions between logical entities
  - the constraints between physical entities
+ Relationship Aliases

|Scheme|Relationship Alias|
|---|---|
|Relational|Relationship|
|Dimensional|Navigation path|
|NoSQL|edge/link|


|level of detail|Relationship Alias|
|---|---|
|Conceptual|Relationship|
|Physical|Constraint/Reference|

+ Graphic Representation of Relationship
  - lines on the data modeling diagram
  
    ![30](../Resources/figure30.png)
    
    
+ Relationship Cardinality
  - caputures how many of one entity  participates in the relationship with how many of other entity
  - is reprented by the symbols that appear on both ends of a realtionship line
  - example: in the Student-Course relationship, the business rules are
    + Each Student may attend one or many Courses
    + Each Course may be attended by one or many Students
  
  
+ Arity of Relationships: the number of entities in a relationship
  - **Unary**(Recursive) Relationship: one entity
    + one-to-many describes a hierachy
      - child entities are on the many side
      - parent entities are on the one side
      
       ![32](../Resources/figure32.png)
      
    + many-to-many describes a network or graph

       ![33](../Resources/figure33.png)
       
  - **Binary** Relationship: two entities
  
      ![34](../Resources/figure34.png)
      
  - **Ternary** Relationship
    + example: **Student** can register for a particular **Course** in a given **Semester**
    
      ![35](../Resources/figure35.png)
  - Foreign Key
    + used in physical and sometimes logical relational data modeling schemes
    + example:
    
    ![36](../Resources/figure36.png)
    
#### Attributes
+ Definition:
  - an attribute is a property that identifies, describes, or measures an entity.
+ Graphic Representation of Attribute
  - Student include
    + Student Number
    + Student First Name
    + Student Last Name
    + Student Birth Date
    
+ Identifiers
  - An identifier(key) is a set of one or more attributes that uniquely defines an instance of an entity.
  - Construction-type keys
    + simple key: one attribute that uniquely identifies an entity instance.
    + surrogate key: an integer whose meaning is unrealted to its face value
      - surrogate keys serve technical functions and should not be visible to end users of a database.
    + compound key: two or more attributes that uniquely identify an entity instance.
    + composite key: one compound key and at least one other simple or compound key or non-key attribute
  - Function-type keys
    + super key: any set of attributes that uniquely identify an entity instance.
    + candidate key: a minimal set of one or more attributes that uniquely identify an entity instance.
    + primary key: the candidate key that is chosen to be the unique identifier.
    
  - Indenpendet entity vs. dependent entity
    + Indenpendet entity's primary key contains only attributes that belong to that entity(rectangles in diagram).
    + Denpendet entity's primary key contains at least one attribute from another entity(rectangles with round corners).
    
  - Identifying vs. Non-Identifying Relationships
    + An identifying Relationship is one where the primary key of the parent is migrated as a foreign key to the child's primary key.
    + An Non-identifying Relationship is one where the primary key of the parent is migrated as a non-primary key attribute to the child.
    ![36](../Resources/figure36.png)
    

#### Domains
+ A domain is the complete set of possible values that an attribute can be assigned.
+ We can restrict a domain with additional rules called constraits.
+ Domain can be defined in different ways
  - Data Type
  - Data Format
  - List
  - Range
  - Rule-based
### 1.3.4 Data Modeling Schemes

|Scheme|Sample Notations|
|---|---|
|Relational|Information Engineering(IE)<br>Integration Definition for Information Modeling(IDF1X)<br>Barker Notation<br> Chen|
|Dimensional|Dimensional|
|Object-Oriented|Unified Modeling Language(RML)|
|Fact-Based|Object Role Model(ORM or ORM2)<br> Fully Communication Oriented Modeling(FCO-IM)
|Time-Based|Data Vault<br>Anchor Modeling|
|NoSQL|Document<br>Column<br>Graph<br>Key-Value|



|Scheme|Relational Database Management System(RDBMS)|Multidimensional Database Management(MDBMS)|Object Databases|Document|Column|Graph|Key-Value|
|---|---|---|---|---|---|---|---|
|Relational|CDM<br>LDM<br>PDM|CDM<br>LDM|CDM<br>LDM|CDM<br>LDM|CDM<br>LDM|CDM<br>LDM|CDM<br>LDM|
|Dimensional|CDM<br>LDM<br>PDM|CDM<br>LDM<br>PDM||||||
|Object-Oriented|CDM<br>LDM<br>PDM||CDM<br>LDM<br>PDM|||||
|Fact-Based|CDM<br>LDM<br>PDM|CDM<br>LDM|CDM<br>LDM|CDM<br>LDM|CDM<br>LDM|CDM<br>LDM|CDM<br>LDM|
|Time-Based|PDM|||||||
|NoSQL|||PDM|PDM|PDM|PDM|PDM|



#### 1.3.4.1 Relational 
+ [A Relational Model of Data for Large Shared Data Banks](https://www.seas.upenn.edu/~zives/03f/cis550/codd.pdf)
  - Data could most effectively be managed in terms of two-dimensional **relations**
  - Objetvies
    + having an exact expression of business data
    + having one fact in one place(the removal of redundancy)
  - It is ideal for the design of operational systems, which require entering information quicky and having it stored accurately.
  - The most common form of notations is Information Engineering(IE).
  



#### 1.3.4.2 Dimensional 
+ Data is structed to optimize the query and analysis of large amount of data.
+ Dimensional data models capture business questions focused on a particular business process.

+ Example: Admission

![40](../Resources/figure40.png)

+ Relational vs. Dimensional
  - The relationship lines in Relational model captures **business rules**.
  - The relationship lines in Dimensional model captures **navigation paths** needed to answer business questions.

+ **Fact Tables**
+ **Dimension Tables**
+ **Snowflaking**
+ **Grain**
+ **Confirmed Dimensions**
  - built with the entire organization in mind instead of just a particular project
  - example: **Calendar** for both **student applicants** and **student graduates**
+ **Confirmed Facts**
  - standardized definitions of term across individual marts.
  - to deal with situations like: different names with the same concept and the same name but different concepts.


# Group Discussion 02/11/2020
## 1. Define a Relational Data Model based on the following entities and batabase state.

![40](../Resources/ch5-1.png)

![40](../Resources/ch5-2.png)


## 2. Discuss the concepts and process of Dimensional Data Modeling.

[Tutorial](https://www.zentut.com/data-warehouse/what-is-data-warehouse/)

#### 1.3.4.3 Object-Oriented(UML)
#### 1.3.4.4  Fact-Based Modeling(FBM)
#### 1.3.4.5 Time-Based
#### 1.3.4.6 NoSQL
# 2. Acitivities
## 2.1 Plan for Data Modeling
## 2.2 Build the Data Model
## 2.3 Review the Data Model
## 2.4 Maintain the Data Model

# 3. Tools
## 3.1 Data Modeling Tools
## 3.2 Lineage Tools
## 3.3 Data Profiling Tools
## 3.4 Metadata Repositories
## 3.5 Data Model Patterns

# 4. Best Practices
## 4.1 Best Practices in Naming Conventions
## 4.2 Best Practices in Database Design

# 5. Data Model Governance
## 5.1 Data Model and Design Quality Management
## 5.2 Data Modeling Metrics

