First lecture

Disadvantages of traditional file processing systems...
- uncontrollable redundancy 
- inconsistent data 
- inflexibility 
- limited data sharing 
- poor enforcement of standards
- low programmer productivity
- excessive program maintenance

An DBMS deal with these problems...
- Concurrency control and locking 
- Transaction processing
- Read-consistency

Data models 
- Hierarchical Data Model (IMS)
- Network Data Model (IDMS, TOTAL)
- Relational Data Model (Oracle, swl server, db2, MySql)
	- A relational DBMS expresses dat in terms of a relation or a table consistent of named columns with data organized into rows
	- uses primary keys to represent associations
	- terminology: relations (tables), columns, tuples(rows), domain, primary keys, foreign keys(link one table to another)
	- Normalization

Information categoreis for the E/R model
- entity-type = a category, set of entities with some commonalities
	- entity = distinct object(person, place, concept, or event), instance given an entity-type
- relationship type = set of associations among entities 
	- relation = instance of relationship type 
- attribute = property of an entity type or a relationship type 
	- attribute domain = set of possible attribute values 
	- examples: name , number
![[Pasted image 20240903102512.png]]

Design a DB
- Build an E/R model
- Each entity-type and relation-type corresponds to a table 
- For an entity-type (table), define its attributes
	- Direct characteristics, not derived
	- seperate fixed-number-of-parts attributes?
	- single data type 
	- think about attributes that are lists
	- Each attribute will be a column
	- Gaurantee that rows are unique
![[Pasted image 20240903102941.png]]
Customer and account are entity type
depositor is the relation type 
account number , customer name and other bubbles are attributes

Design Choice
![[Pasted image 20240903103123.png]]
![[Pasted image 20240903103222.png]]
It would be better to have 2 seperate tables to better distinguish customers that have the same name

Primary Key 
- A combination of columns which uniquely specify a row
![[Pasted image 20240903103544.png]]

Foreign key
- A field in a relational table that matches a candidate key of another table
![[Pasted image 20240903103710.png]]

Normalization
- Minimize redundancy and dependacy in tbales and rows
- Break down tables to ensure that each independent piece of information is in only one place
- Insertion, deletion, and modification or a row can be only in one table
- Drawbacks?
	  - its good for transaction, but bad for data analysis/data mining
	  - a

Client-Server Architecture  ![[Pasted image 20240903104225.png]]

![[Pasted image 20240903104454.png]]
Transaction: 2

![[Pasted image 20240903104803.png]]

![[Pasted image 20240903105235.png]]
![[Pasted image 20240903105756.png]]
![[Pasted image 20240903110100.png]]
![[Pasted image 20240903110221.png]]
![[Pasted image 20240903110807.png]]


![[Pasted image 20240903110855.png]]

