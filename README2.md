Introduction to information systems (WSI) Lectures

# [1](https://www.google.com/url?q=https://gakko.pjwstk.edu.pl/edux/7542/lessons/62108/chapter/25888&sa=D&source=editors&ust=1714064099677980&usg=AOvVaw0tlrRygRi0poLKkT0s7DWX) [Lesson II – Introduction to the relational databases](https://www.google.com/url?q=https://gakko.pjwstk.edu.pl/edux/7542/lessons/62108/chapter/25888&sa=D&source=editors&ust=1714064099678312&usg=AOvVaw3-g6gxmy2ZiK8iMgYp2lOo)

[15.03.2024 11:45 | Number of chapters: 8](https://www.google.com/url?q=https://gakko.pjwstk.edu.pl/edux/7542/lessons/62108/chapter/25888&sa=D&source=editors&ust=1714064099678667&usg=AOvVaw1IkUlf7Q1KQz-_ErHPhDcp)

# New skills

The goal of this lecture is to explain the problem of storing data, especially within relational databases. This issue will be studied in depth in future semesters during lectures like “Relational Databases”  and “Database Systems” . After studying the five following database related lectures student should be able to explain terms like “data”, “information”, “logical database structure”, know the basics of designing the relational database structure and the basics of SQL query syntax.

The first lecture is dedicated to explaining the need of storing data in today’s world and pointing out the currently used technologies and data models.

### Learning outcome

*   Student understands the ubiquity of data stored in various ways depending on the technology used,
*   Student understands the need of introducing data structure when storing data,
*   Student is able to list the database examples from the everyday life,
*   Student understands the existence of various data models and can explain in detail at least two of them.

# Database – what’s that?

The term „database” in the sense of a system for collecting and storing data dates back to the ancient times. People have always strived for recording their knowledge. The main purpose of this activity was the possibility of drawing conclusions on the basis of possessed information. The basic idea of this mechanism hasn’t changed at all.

### Do you see this sign:

(![image](https://gakko.pjwstk.edu.pl/public/7164/WSI_3.png)

### Remember where and inform the others.

All we need to know is:

*   How to store this information?
*   How to make it available?
*   For whom should we make it available?

While the answer on the third question depends mainly on one’s intentions, the answers to the first and the second questions are strictly dependent on the technology at our disposal. Moreover the technology used can influence the data accessibility and therefore the usability of our solution. Hence our conclusion is: the ability to store information and the extent of its accessibility are determined by the technology we use.

### How was data stored in ancient times?

We can say that one of the important aspects of human history was the way of recording and storing data. Only few were known and all of them were determined by the technology available at that stage of human development.

### Ways of storing data archaic from our perspective

Clay tablets, cuneiform writing  – 4 000 BC till 4 century

(![image](https://gakko.pjwstk.edu.pl/public/7164/WSI_4.png)

Papyrus, handwriting  – 3 000 BC until the first century

(![image](https://gakko.pjwstk.edu.pl/public/7164/WSI_5.png)

Parchment, handwriting and print  – 3rd century BC till 17th century

### …and a little closer to our times

### Finally a few modern technologies

Paper  – discovered in China in 8 BC and used until today around the world

Print  – method of duplication of text with a stamp, known for thousands of years. Modern printing is done using a moveable type invented during the medieval times. The zenith of its development falls on the first half of the 20th century.

(![image](https://gakko.pjwstk.edu.pl/public/7164/WSI_6.png)

First modern printing machine  was constructed significantly later (in second half of 19th century) as an aid for handwriting.

![](https://gakko.pjwstk.edu.pl/public/7164/WSI_7.png)

### … and what was the result of storing this data?

After many years of acquiring and storing data we managed to collect an enormous amount of data.

Library of Congress  – the biggest library in the world. 142 mln of various documents (29 mln of books, 4.8 mln of maps and atlases, 12 mln of photos, 6 mln of microfilms, 3.5 mln of music documents, 0.5 mln of films). Library consists of 856 km of shelfs in three buildings. There are 22 reading rooms, 5 thousands employees (source: Wikipedia).

And there are so many other, smaller libraries containing a lot of data.

What’s our conclusion then? We have enormous collections of data recorded using various old, “classical” technologies. This, however leads to serious problems, such as: how can you find the information you need in this enormous data set using the old technologies? Or how can we make sure that the information coming from two different sources is consistent? And finally, how to decide which information is “true” and which is “false”?

### Computer – revolution in technology

…of course not only in the data storing technology. And it did not happen overnight.

Atanasoff-Berry Computer, ABC  – machine used for solving linear algebraic equitation. The first machine was built using 270 electron tubes. It used binary numbers and wasn’t programmable. USA 1939.

Z3 – (relay successor of mechanic Z3) – Germany, 1941  – the computer was able to perform four types of operations and extract the roots from binary numbers, the clock frequency was 5 1/3 Hz, the memory capacity up to 64 words (each consisting of 22 bits ), the program memory consisted of an eight channel punched tape. Only one model was built and it was subsequently destroyed by the Allied forces. It was used for the endurance calculations of wings in the aircraft industry.

Colossus  – Great Britain – the first one was built on 14th of April in 1941. Altogether 11 models were built. It was used for breaking the code of German encryption machine called (Lorenz machine).

ENIAC  – USA 1943 – 1945 (27 tons, 18 000 electron tubes, 140 square meters). It didn’t have operational memory. It was programmed by manipulating switches and cables. Afterwards it also used punched cards.

As we can see the beginnings weren’t so easy. But what has the computer brought to the technology of storing data? There are two basic technology advancements we should point out:

*   The drop in prices of mass storage (tapes, drives, CD) allowed for storing vast amounts of data on very little space and with little cost.
*   The ability to search through data in relatively short time.

![](https://gakko.pjwstk.edu.pl/public/7164/WSI_8.png)

But along with these possibilities certain challenges appeared. Various data structures were needed for efficient data storage in order to make a full use of the computer. This is the beginning of the databases in the modern meaning.

### Control questions

Do you think that the computer is necessary for storing data?

Yes

No

Check the answer

Did the concept of data storage appear in the second half of the 20th century?

Yes

No

# Database – basic information

We often use terms “data”  and “information”  interchangeably. But what do they really mean? Are they interchangeable?

Information  and data  –both terms are used for describing the reality or more precisely a part of it, but they are not synonyms.

Data  – these are values that can be transformed and processed (by computer or by our mind). We can assume that data is something that we can save and record in various ways (numbers, text, image files etc.).

Information  – this term generally means data along with its semantics which is the key to proper interpretation. Lack of interpretation can render data useless.

Let’s assume that in front of us we have a page with Japanese symbols. This is our data. But can we read and understand the information contained within each symbol? We probably could if we knew the Japanese language. Otherwise we can’t. Just to be clear I have no idea about Japanese language.

Data is one of company’s (or institution’s, organization’s) main assets, next to its capital, employees and infrastructure. It allows the company to operate and interact with business environment but, just like other assets, it requires maintenance and management. The data management is realized through the information system  which satisfies the need for information about certain part of our business domain. Database is usually a part of this system which is responsible for storing, security and management of the data and its accessibility.

We can identify here a conceptual dualism. By “database” we mean:

*   Database Management System (DMS) – data structure, security, rules about its accessibility (DBMS)

Or

*   Data Collection (DC)

The database has become a standard way of introducing structure and rules into the process of data management. These structures and rules evolve together with the information technologies. In the next part of this lecture, under the term “database”, we will mean the term ”Database Management System”.

### Control questions

Can you tell what number it is? - 1101

Yes

No

Check the answer

Can a school library be called a "database" according to/as explained in the aforementioned definitions?

Yes

No

Check the answer

Can student’s notes from lectures be called a “database”?

Yes

No

Check the answer

# More on database

### What do we expect from a DBMS?

We generally expect database to securely store our data and allow it to be easily queried by the authorized users. In practice we demand the following:

*   Durability  – data should be stored for specific amount of time. Usually we don’t know how long this period will be. Time should not affect the data.
*   Data must be accurate  – data must reflect the reality as accurately as possible and the structure must allow for data updates whenever changes occur.
*   Replication control  – database must guarantee control over the redundant data in order to avoid ambiguity.
*   Structure design  – database should be structured in accordance with specific data model.

As it soon turns out the technological progress has rendered the last two demands somewhat outdated and consequently they are often rejected by modern database specialists.

I would like to turn your attention to the term “redundancy”, which describes superfluous data used to record some kind of information. It can lead to a situation when we obtain different and often contradictory answers when we use different data sets to describe the same thing. Of course this is an unwanted situation, although in practice it is inevitable to some degree. If it happens we would like to know how to control it.

### What do we require from a modern DBMS?

Any modern database must fulfill many different requirements which are necessary for functioning as part of information system, such as:

*   Concurrent data access  – database must be able to handle many concurrent operations on the same set of data while maintaining data consistency. Can we imagine banking, airport control or ticket booking systems which cannot handle securely hundreds or thousands of concurrent clients trying to access them?
*   Data security  - this is a multi-faceted issue. Security can be considered from many different viewpoints. Data is valuable, its acquisition is usually costly and its loss may be devastating for a company (e.g. banking systems).
*   Independence of the data and the processes using it  – this property has a big impact on the possibility of the future development of an information system and of a widespread use of databases as part of it. One database can be accessed by many processes, run by different applications on various platforms. The DBMS should be able to handle them independently of their platform or technology.

We should always remember that the costs of fulfilling of each aforementioned requirements are proportional to the quality of the solutions adopted . On the other hand cheaper solutions may turn out to be much more costly on the long run!

# Does information always have value?

We can conclude that information has value if it is:

*   Correct  – it contains true information about specific subject. It is obvious that keeping the false information does not make sense. Of course it does not mean that all of the information stored in a database are always correct. The reasons behind it may vary – starting from errors in data model structure or errors during writing or reading process, finishing with a deliberate act of data manipulation.
*   Accurate  – information should be neither too accurate nor too general. Storing and searching the database is costly. From this we can conclude that storing too detailed data can generate unnecessary cost. On the other hand absence of important data can render information to be inaccurate or false. This is why the phase of designing the correct database structure is so important, especially the decisions we make about the level of detail that we want to store.
*   Available  – time required to access the information must be adequate to the importance of data. Of course “time of access” is a relative term. One hour may be the proper time frame for generating a company annual balance sheet but it is surely unacceptable for checking the train timetable. Incorrect database structure and incorrect methods of acquiring data can prevent access to data in a reasonable time. In this kind of situation changing the hardware configuration (e.g. adding more RAM) wouldn’t help in a long run and would generate additional costs.

### Databases are everywhere

Considering why databases have become such an important part of information technologies we should point out two main aspects: formalizing of the database concept and emergence of consistent data model, on which a number of applications were developed, allowed to solve a number of problems caused by:

*   A ubiquity of information,
*   Creation of various data sets with increasing level of volume and complexity,
*   The widespread need for availability of data with lower access time,
*   Easy and widespread possibility of generating new data sets.

Of course the Internet and its popularity has had a big influence all over the world as Web 2.0 became more popular – every Internet user is now both the consumer and the producer of data.

We can assume without hesitation that every IT - related project nowadays uses some kind of database, either internal (integral part of the project) or external (which shares its data through a specific interface). Moreover it is possible that one IT project uses multiple databases or that one database is used by multiple IT projects.

The field of database systems represents nowadays one of the largest and most active segments of software market (which means good earning possibilities). Creating and management of databases involves almost all branches of the modern IT:

*   Operating systems,
*   IT theory,
*   Artificial Intelligence,
*   Logic,
*   Programming languages,
*   Multimedia,
*   Software engineering.

### Control questions

What does the term “redundancy” mean?

Storing data which is contradictory.

Lack of data, which prevents acquiring the correct information.

Unnecessary/redundant data in the database.

Check the answer

Does the information access time decide about the quality of IT solution?

No, time required to access the required information is irrelevant if we are able to acquire it.

The information access time is one of the main parameters determining the quality of the DBMS.

Check the answer

# Data models – what is it?

Data model is a data storage structure which allows us to anticipate where and in what form data will be stored and how it will be queried and read. In a relatively short span of IT technology evolution a few models have emerged, the most important of which is the relational database model. In fact, the database history can be split into the period before this data model and afterwards.

## “Classical” data models

### The card index model

Data is stored in records within one or more tables of identical structure. The records can be sorted and filtered. Each table is an independent document without the possibility to cooperate with the others. The phone book in a mobile phone or tables in Excel or Word are good examples of this model.

### The hierarchical model

In this model the data is stored in the form of records linked by forming a parent - child relation structure. Each record has one parent. If record has more than one parent it must be copied to keep the aforementioned rule. Removing the records means deleting all off its descendants. This model should be familiar from our file system. In order to operate on data we can use traditional programming languages like C, Pascal or others.

Searching through data in a hierarchical database requires looking through all of the descendant records. An example of this database model can be found in a family tree. In the world of IT we can find this model in our file systems.

### The network data model

This model is an extension of the hierarchical data model. It allows to add pointers which allow for sharing “branches” of the data tree structure among records. Relations between records are defined by creating the collections of data which thus model an owner - member relationship. Each record can enter multiple relationships.

### The relational model

The relational data model represents a radical change in comparison to the classical database models whose functioning is based on the concept of file and records (lines) written in it. The relational model turned out to be a great success as it gave a solution to many important problems. It introduced a lot of well thought out solutions which were a turning point in developing highly scalable database solutions (e.g. SQL language, advanced “engines” for processing data). Because of that it has become a reference point for further development of the database solutions.

On the other hand the relational model is more than 40 years old. This is a long time in the IT industry. Nowadays there are more modern approaches to solve similar problems.

### Object databases

The concept of object databases emerged when it became necessary to work with non-objective data structure in objective programming languages. The “objects” in object database represent real life entities and they possess certain identity. Object type (class) defines complex data type which can contain other data types or collections of data types. Data structure is characterized by strong encapsulation (inner structure of the object is not visible to the user). Moreover, the knowledge of this structure is not necessary for using the specific object. The object inherits the structure, properties and methods from its class. In spite of the beauty of such solution (in terms of the IT theory) it hasn’t become as popular as the relational data model due to the enormous cost of replacing already working relational solutions with object databases. On the other hand it doesn’t seem to solve one of the most important problems of the modern IT technology which is processing very large volumes of data (the “Big Data” problem).

However there are some solutions developed by object databases which have been introduced into the relational databases resulting in structures called object - relational solutions.

### Modern data models

Actually this is the end of the history of “well-defined” data models. Modern technologies (Internet, cloud-related technologies) force us to develop other approaches to data processing. Instead of the “data model” we now prefer to talk about the “Database Management System”.

All of the classical data models assumed the existence of predetermined, rigid structure for storing data. This approach was very convenient especially when it comes to data querying. However it doesn’t work well when faced with challenges of modern world like common Internet access and the Web 2.0 philosophy.

The main problem is the need for processing very large volumes of unstructured data in small time frame, for example the data generated by social sites like Facebook, Twitter, and internet search engines (Google) or services used for storing data in the cloud. The solutions for this problem are database management systems (or data models) which deliberately abandon various requirements of the traditional data models, like the control of replication or uniform data model (there is a few more but we will leave it for now).

The DBMS’s which perform these tasks are called the NoSQL Databases (Not Only SQL).

### Graph databases

A graph database is based on the concept of a graph. Each node represents an object and the data associated with it. Graph’s edges (named and directed) represent relations between objects. Typically this kind of database is used for modelling of social networks.

### Semantic Web

This concept (it can hardly be called a data model) assumes the emergence of a technology and standards which allow machines and programs to search and process data based on its semantics. In this case we treat Internet and its resources as “the database”.

### Map Reduce

Again it is difficult to call this a data model. Here we deal with the concept of storing and concurrently processing of large volumes of data within big data clusters. It comes down to dividing the problem into various smaller ones which then can be split among different clusters. The results from the clusters are returned and merged together into one global solution. This concept has already a few implementations and is currently in the development stage.

# A short history of databases

*   1961  – Integrated Data Store IDS  (author: Charles Bachman for General Electric) – first DBMS, first implementation of the network data model
*   Started in 1966 , first-ever run in 1968  – Information Management System IMS –  Created by the IBM consortium along with the Rockwell and Caterpillar for the purpose of managing the technical documentation of Saturn V rocket ship and Apollo capsule. Realized according to the hierarchical data model (is still in use).
*   1970  – dr Edgar Codd (IBM employee at that time), proposed basic principles of relational data model in the article “A Relational Model for Larged Shared Data Banks”
*   1969  – the first specification of the network data model known as CODASYL . There have been many implementations loosely based on this specification. The ISO/ANSI standardization was created in 1968 but it gained no practical significance.
*   First half of 1970s  – first prototype of SQL query language called Sequel  (authors: Donald Chamberlain and Robert Boyce) was created in IBM’s laboratory in San Jose. However the name had to be changed to the Structured Query Language (SQL)  due to the naming issues with a British company called Hawker Siddeley.
*   1974  – first relational database management system and first implementation of SQL – System R  in IBM . In the beginning it was treated as a research project. Their first commercial client was Pratt & Whitney in 1977.
*   1976  – Peter Chen created the concept of the entity data model (ERD, ERM) as the methodology for designing and analyzing database structure. It has become the base of the future CASE solutions and repositories. However it hasn’t been standardized so far.
*   1977  – the company called Software Development Laboratories  was crated. In 1979 it was renamed to Relational Software Inc.  and in 1982 it was renamed once more to Oracle Systems Corporation . The company started to work on a database system compatible with Codd’s relational data model. In 1979 they introduced their first commercial database solution called ORACLE 2.
*   1983  – IBM introduced system called DB2  which was the successor of System R . It was the first fully commercial relational database. In the beginning it was used only with the mainframe computers produced by the IBM .
*   1986  – the first standard of the SQL language (ANSI)
*   1987  – the first standard of the SQL language (ISO)
*   Next versions of the ANSI/ISO standard: 1989, 1992 (SQL2), 1999 (object - relational data model), 2003, (SQL:2003, XML databases), 2006 (SQL:2006, usage of SQL with XML), 2008 (SQL:2008).

### Further development of databases

1990s – the database theory was expanded to include the following aspects:

*   Multilayer architecture
*   Distributed data
*   Concurrent access methods
*   Internet as a data access technology
*   Data warehouses and OLAP (On-Line Analysis Processes)

Databases are used in new technologies:

*   Storing and sharing multimedia
*   Storing documents (including XML data)
*   GIS (Geographical Information Systems)
*   Utility systems – ERP (Enterprise Resource Planning) and MRP (Management Resource Planning) – packages like SAP, Baan, Oracle, PeopleSoft, Siebel, CRM (Client Relationship Management)

# Summary

In the second lecture we presented the history of databases and their importance in the modern information technologies, and thus in many branches of economy and administration. We introduced different concepts of data models including the relational data model. In the next lectures we will discuss the relational data model in detail.

# [2](https://www.google.com/url?q=https://gakko.pjwstk.edu.pl/edux/7542/lessons/62109/chapter/25896&sa=D&source=editors&ust=1714064099699058&usg=AOvVaw1v4gCqauJJWZiVsZcYgZgD) [Lesson III - Relational database model](https://www.google.com/url?q=https://gakko.pjwstk.edu.pl/edux/7542/lessons/62109/chapter/25896&sa=D&source=editors&ust=1714064099699423&usg=AOvVaw2nCslZ3faL7ehjslDxABXU)

[15.03.2024 11:45 | Number of chapters: 9](https://www.google.com/url?q=https://gakko.pjwstk.edu.pl/edux/7542/lessons/62109/chapter/25896&sa=D&source=editors&ust=1714064099699733&usg=AOvVaw1C4mw_YVCXXCUB3BGOEmnz)

# New skills and knowledge

In this lecture we will present the idea of a relational database and elementary examples of data structures in the relational model. We will also present so-called Codd’s 12 rules, which constitute the basic assumptions of the relational model. After this lecture student should grasp the general idea of this model. I would like to emphasise that this lecture contains the basic knowledge necessary for understanding the relational model and for further learning of this subject.

### Learning outcome

*   Student knows who was the inventor of the relational database model,
*   Student understands the concept of data storage in a logical table structure and the idea of recording the relationship between data written in many different tables,
*   Student can define the concepts of a primary key and a foreign key and understands their function in the relational database model,
*   Student knows and understands the notion of a relation as a mathematical model of a database table,
*   Student understands the notion of the pseudo-value NULL and knows the results of algebraic, text and logical operations using NULL.

# The origin of the relational database model

Edgar Frank Codd was the founder of the relational database model. A short biographical note from Wikipedia is enclosed below

Edgar Frank “Ted” Codd  (19.08.1923-18.04.2003) was an English computer scientist, famous for introducing the relational database model. He studied maths and chemistry at University of Oxford. During the Second World War he served as RAF pilot. In 1948 he moved to New York to work for IBM as a mathematical programmer. In 1953 (at the time of McCarthy’s commission) he moved to Ottawa, Canada. A decade later he returned to the USA and received his doctorate in computer science from the University of Michigan in Ann Arbor. After that he moved to San Jose, California, to work for the IBM. During 1960’s and 1970’s he worked out his theory of data arrangement, issuing his fundamental paper “A Relational model of Data for Large Shared Data Banks” in 1970. To his disappointment, IBM proved slow to exploit his suggestions until the commercial rivals such as Oracle (formulated by Larry Ellison and based on Codd’s ideas) started implementing them. Codd also coined the term OLAP (Online analytical processing) and wrote “the twelve laws of online analytical processing”. He also had a contribution to the cellular automata theory. Codd received the Turing Award (computer science “Nobel Prize”) in 1981.

![image4](../Images/image4.png)

Initially the relational model was sceptically received as other data storage systems had already been in use. The Integrated Data Store developed on the basis of the network data model by General Electric, and IBM-made Information Management System, based on the hierarchical model were already available. Nevertheless, its popularity grew in time and soon the relational database model became the most popular.

Today, despite the emergence of next generation models (the objective and the semantic ones) applications implementing the relational models still dominate the market. This is due to its simplicity and flexibility, high quality of the relational model-based DBMSs as well as large amounts of data already stored in relational databases. We do observe though a tendency to include some features of the objective models into the relational model, giving rise to the so-called objective-relational database model.

# Relational database model, the first elementary example

In the next lectures and during other database related courses the relational database model will be presented in more detail. In this lecture the basic principles of this model will be presented using an elementary (but representative) example.

The basic principles of relational database model are:

*   All data is written in the form of tables
*   A table contains columns which include data of a specific type
*   A table cell (on the intersection of row and a column) contains a single, atomic, indivisible value

These three conditions are enough for now.

### Relational model: the first elementary example

### Assumptions

Let us assume that we want to record information about courses and lecturers at our school. We assume that each course has only one lecturer, but every lecturer can be responsible for many courses.

We need to guarantee unambiguous identification for every lecturer and every course and we also have to attribute every lecturer the courses taught by him or her.

In accordance with the above formulated postulate that all the data must be written as tables, we will start by creating a table of LECTURERS .

This table will include each lecturer’s personal and professional data – name, surname and his or her scientific degree. Every row (record) will include the data of one lecturer. In order to be able to distinguish between the data of each lecturer independently from their names and surnames (which can in principle be the same for different people!), each record (and thus also the lecturer) is identified by an additional field (i.e. a column) named Lecturers\_Id. It is essential that each lecturer has an unambiguous, unique identifier, because in the relational model a row can only be identified by the values stored in the columns. Since we have assumed that the lecturers’ names and surnames are not unique we need to include a column whose value uniquely identifies a row.

![image74](../Images/image74.png)

We now need to prepare the COURSES  table. This table will include the courses data: the name of the course, its code and the Lecturers\_ Id. Note that its value doesn’t describe any feature of the course itself, but rather represents the relation between the course and its lecturer, whose data can be accessed in different table using the Lecturers\_Id.

![image34](../Images/image34.png)

Adding an unambiguous key for each row to the table LECTURERS  allows us to connect rows from the tables LECTURERS  and COURSES . Thus there is no need for each row to include all the data (name, surname, degree) of the course’s lecturer. In fact this would lead to redundancy: one piece of information (the lecturer’s data) would be stored in many places.

The value of the Lecturers\_Id will appear in the COURSES  table as many times as many courses the lecturer is responsible for. On the other hand, each course is connected with at most one lecturer and the “Data warehouses” course is not connected to any elements of LECTURERS , which simply means that the course has no lecturer assigned yet.

### Control questions

Can we have 9999 in the index for the Lecturers\_Id table in the elementary example above?

Yes, we can

No, we can't

Check the answer

Which option for the row “Data warehouses” would be better: leaving a cell LECTURERS\_ID empty, or filling it with a value not appearing in Lecturers\_Id column in LECTURERS table?

It is better to leave the cell empty.

It is better to fill in the cell with arbitrary value.

Check the answer

# Primary, alternate and foreign keys

Each table must have an unambiguous index which is called the primary key . It represents one or more columns, whose values unambiguously identify the row (record). The primary key value must be specified and unambiguous.

An alternate key  (called also candidate key or just key) has the same uniqueness property as the primary key, but there is only one primary key and there can be several alternative keys.

In the COURSES  table Code  is the primary key, while Name  is an alternate key. These keys specify the course uniquely in a natural way if we assume that no 2 courses can have the same name or code. In the LECTURERS  table Lecturers\_Id  is the primary key. The family name, the first name or the degree on the other hand cannot be the primary keys, as their values can repeat. It is even possible for all 3 values to repeat. Thus, we have introduced an additional column Lecturers\_Id which describes no physical feature of the lecturer, but which is used as a unique identifier of a lecturer.

A foreign key is one or more column whose value is the primary key identifying a row in another table.

In the COURSES  table the LECTURERS\_ID  is a foreign key whose values come from the primary key column of the LECTURERS  table. For example the value 235 in the “Relational databases” lecture points to the row in the LECTURERS  table which contains the information about a lecturer whose surname is Kowalski, whose name is Jan and who holds a PhD. This information may simply be interpreted as:

“The ‘Relational databases’ lecture has been assigned to a lecturer named Dr Jan Kowalski”.

### Control questions

How many primary keys can table in relational database have?

Up to 1

Only 1

Possibly more than 1

Check the answer

Does a relational database need to have a foreign key?

Yes, there must be at least one.

No, there are tables which do not have any foreign key.

Check the answer

Is it possible for the foreign key value to be indefinite?

Yes, if we assume this is allowed.

No, the foreign key value must be specified for each table row.

Check the answer

Can a foreign key have an arbitrary value?

Yes, as long as it is consistent with the data type in the column.

No, we can only use values which have previously been used as primary keys of the appropriate table.

Check the answer

Can the value of the primary key remain indefinite?

Yes, if we assume from the beginning that we allow it.

No, its value has to be set in every row of the table.

# Relational database model: elementary example 2

### Assumptions

Let us modify our assumptions from the previous elementary example. Let us assume now that we need to record data about the courses and the lecturers. Just like before, one lecturer can teach several courses, but unlike the previous example one course can be taught by more than one lecturer.

The database needs to be able identify uniquely all lecturers and all courses, find all lecturers responsible for each course and all courses assigned to a given lecturer.

Let us use the data of two lecturers and their courses for our database example: dr Jan Kowalski teaches PPJ, ASD and SBD, and dr Konrad Piotrowski teaches AUG, ASD and RBD.

The table below shows how tables LECTURERS  and COURSES  can be linked.

![image35](../Images/image35.png)

As we can see, our case is now more sophisticated. In order to link the courses with their lectures we would have to write multiple values into the Lecturers\_Id column of the table. If we implemented this solution it would mean that we break the atomic rule, which is one of the most important rules in relational model.

Let us try to implement another solution for our case. Let us then record pairs of records (a lecturer and a lecture) registering this way links between them. Note that we do not need the full records as each record is identified by its primary key. Thus, writing just pairs of primary keys we store sufficient amount of information to link lecturers and their courses.

![image68](../Images/image68.png)

Our current scheme is shown below:

![image87](../Images/image87.png)

In order for the scheme to be clear the linking arrows have been left out. As you can see, we managed to record the full information about the links between the lecturers and the courses they hold in a separate table. In a table storing this data (called the junction table) each lecture primary key appears as many times as many lecturers hold it and, conversely, each lecturers primary key appears as many times as many lectures he is assigned to. And what is the primary key in a junction table? Note that the code and the Lecturers\_Id taken together must be unique. Repetition of these values would result in redundancy (repeating the same information). Thus the primary key of the junction table is defined as the sum of the 2 foreign keys.

One final remark: I would like to point out that that thanks to the junction table we have effectively returned to the situation from our 1st example: now each record in the junction table is linked with one table record and one COURSES  table record.

### Control questions:

Can we solve abovementioned case without using associative/junction table?

No, it is not possible.

Yes, this is possible by entering more than one value of the foreign key in the appropriate column.

Check the answer

Is it possible to omit the value in one of the columns of a junction table?

Yes, you can omit one.

No, no column can be omitted.

# Database – why have we chosen the relational model?

In maths we define a relation as a subset of the Cartesian product of two sets.

Discrete mathematics – short revision

The Cartesian product of two sets A and B is a set of all ordered pairs (x,y) such that x is an element of A and y is an element of B.

A × B = {(x,y):x ∈ A and y ∈ B }

The Cartesian product is not commutative : A×B ≠ B×A

For example:

A={a,b,c} B={1,2,3,4}

A×B = {a1, a2, a3, a4, b1, b2, b3, b4, c1, c2, c3, c4} B×A = {1a, 1b, 1c, 2a, 2b, 2c, 3a, 3b, 3c, 4a, 4b, 4c}

Thus:

A relation on sets A and B is any subset of the Cartesian product A×B, while a relation on B and A is any subset of B×A.

The end of discrete mathematics revision

But how is this connected with the main topic of this lecture, i.e. databases? It’s easy to see that the representation of a relation built on two sets is a 2-dimensional table made of 2 columns and as many rows as many elements of relation we have. Obviously a relation on n sets can be represented by a table with n columns. This concept is the basis of the relational database model: all data are stored in two-dimensional tables.

The set of 13 rules (numbered from 0 to 12) which need to be fulfilled when designing a relational database management system (DBMS) as well as the database model has been published by Edgar Codd in his article “A Relational Model of Data for Large Shared Data Banks” published in 1985. It is known as the “Codd’s 12 Rules” .

Before we discuss some of the rules in detail we need to introduce two important notions.

### Database levels of abstraction

A database can be considered on various levels of abstraction:

1.  The external (view) level:  this is the way ordinary users see the data in a database. What he or she sees is usually very different from the data structure on the logical level (i.e. the table structure). What we mean here is the access to the database via client applications, usually using a GUI, for example via a web browser.
2.  The logical (conceptual) level:  this is the collection of tables linked by relations as well as all other objects guaranteeing the integrity of the data and its connection to the physical record on a disk. We focus on this level in this lecture, because it is the level on which the database designers and developers operate.
3.  The physical level:  the collection of files in a file system in which the data is physically stored. This level is interesting to a rather limited number of users, consisting of the system administrators.

### Constraints

The constraints are rules whose functions is to guarantee the logical correctness of the data stored in the database. They are defined already in the database designing phase and they are later enforced by the DBMS. We will discuss this in detail further on.

### Control questions

Can the Cartesian product of two sets contain 2 identical elements?

Yes

No

Check the answer

Do we need to consider the files arrangement on the servers’ disks while designing a database?

Yes

No

Check the answer

# View – a useful tool for working with RM (relational model)

In the example above it was possible to store data about courses and their lectures in a simple and clear way. It is however much more difficult to read the data about the relations between the records in the LECTURERS and the COURSES table.

In example 1 we described the relations between lecturers and their courses where we assumed that one course can be taught by only one lecturer, whereas a lecturer can teach several courses. Accessing information stored in these tables is quite simple. If we want to read data about lecturers and their courses, we need to read data from tables. This can be achieved using the links between the rows (records), the primary key values in LECTURERS table and the foreign key values in the COURSES table.

The relations between the lecturers and the courses are even more difficult to read in Example 2. Recall that we have assumed that ONE lecturer may hold many courses and at the same time ONE course may be simultaneously held by many lecturers. Our solution was to create an additional table just for the relations between courses and lecturers. In this additional junction table we store pairs of foreign keys linking the lecturer with the appropriate course. But this means that in order to find out which lecturer holds which course we need to read data from three tables: the lecturer’s data from LECTURERS, the course data from COURSE and the data about the relation between them from the junction table. This is somewhat cumbersome.

As you can see, the RM is not particularly user-friendly when it comes to reading the data. We need to read three separate tables and link the appropriate records with the corresponding primary and foreign keys if we want to find out who teaches which course. This process may be simplified if we use objects called VIEWS created as the result of reading the current state of data.

We present an example of a view containing courses names and lecturers data.

![image26](../Images/image26.png)

A view presents data in a way they are seen by the users (and not the database designers). Views provide data (from one or more tables) which are suitable for presentations. The same data can be presented in different layouts by various perspectives.

The content of a standard view is calculated by the system from the underlying tables. Usually the result of this operation is not permanently stored in the database. What is recorded is the view’s definition (a ‘recipe’ how to prepare it). Although views do not store data, they are often called ‘’virtual tables” as they ‘’provide data’’ for database objects and processes in the same way as it is done through the tables. Moreover, the result of the data reading is the same for the end user irrespective whether it was read from a view or from the tables themselves. The end user doesn’t usually know if the provided data come from the table or from a view.

In some cases it is more convenient to store the content of a view in the database and use it instead of performing complicated searches which might overload the server. This kind of view is called the MATERIALIZED VIEW . Not all DBMS’s create and store materialized views. Note that although a materialized view is physically stored the same way as a table, there is a significant difference between them. The data in a database are “alive”: the records may be modified, rows may be added or removed. The data in tables are always up-to-date. The data in a materialized view on the other hand constitute a snapshot of the database from a given moment. If the data in the database changed after the materialized view had been made the view remains unaffected. It’s important to realize that.

### Control questions

Can we use a non-materialised view to store data?

Yes, we can store data in non-materialised view as well as in tables.

No, a view cannot store data.

Check the answer

On which database abstraction level are views used?

Logical level

Physical level

External level

Check the answer

*   abase objects.
*   DML  (Data Manipulation Language) – set of instructions for writing, modifying and deleting data.
*   DQL  (Data Query Language) – set of instructions to read data from databases.
*   DCL  (Data Control Language) – set of instructions for authorizing and de-authorizing users to access and manipulate data.

The SQL language structure will be presented in more detail in the next lectures and other database related courses. It is important to remember that SQL in its basic form is not a programming language. It does have extensions allowing to use variables, conditional statements, loops, recursion and exception handling. Note however that while the SQL syntax is almost identical in all of its implementations, the extensions are quite different in many aspects. Another big difference between SQL and other programming languages is its declarative character: in SQL we define what operation we need to be executed, but the way it is done is decided by the DBMS. In other words: we decide what needs to be done, but we leave the decision about the way it is done to the DBMS.

## Rule 10

## Integrity independence.

Integrity constraints specific to a particular relational data base must be definable in the relational data sublanguage and storable in the catalogue, not in the application programs.

The DBMS must guarantee the possibility to define the integrity constraints and enforce them. Defining database constraints must be possible on the DBMS level, independently from the applications using it. Their modification must be possible at all times without the need to update the applications. Fulfilling this rule guarantees that the constraints defined once and stored in one place will be obeyed by all processes accessing the database.

### Control questions

Which of these objects constitutes the logical data structure in a relational database?

A file

A view

A table

A folder

Check the answer

You are looking for one piece of information in a database. Is it enough to know the column’s and table’s name to find it?

Yes

No, one more information is needed.

Check the answer

You are looking for one data in relational database. Is it necessary to know the name of the file where these data are stored?

Yes

No

Check the answer

What is the result of this operation: X\*3 + 12 for X as NULL (pseudo value)?

12

15

NULL

0

Check the answer

What is the result of FALSE AND NULL logical operation?

TRUE

FALSE

NULL

Check the answer

What is the result of FALSE OR NULL operation?

TRUE

FALSE

NULL

Check the answer

What is the result of TRUE OR NULL operation?

TRUE

FALSE

NULL

Check the answer

# Final remarks

This is probably the most important lecture of the whole WSI course concerning the relational databases. We presented the concept of the relational database model, which is built on the relation algebra, briefly outlined here, and the logical idea of recording data in tables. We have also introduced a new notion: the NULL pseudo value modifying the standard logical operations. We will encounter this notion repeatedly in the field of databases, so it is very important to understand what role NULL plays in the elementary logic. Finally the Codd’s rules (only a few presented here, the full list will be discussed on the RBD course) form the axiomatic basis for the relational data model. We need to understand them in order to understand the field of relational databases.

# [3](https://www.google.com/url?q=https://gakko.pjwstk.edu.pl/edux/7542/lessons/62110/chapter/25905&sa=D&source=editors&ust=1714064099719621&usg=AOvVaw3ZGziaYetkoApwMlRB96bM) [Lesson IV - Designing database structure](https://www.google.com/url?q=https://gakko.pjwstk.edu.pl/edux/7542/lessons/62110/chapter/25905&sa=D&source=editors&ust=1714064099719928&usg=AOvVaw1ngkhpNS2XCP6JVEQblBLa)

[15.03.2024 11:45 | Number of chapters: 5](https://www.google.com/url?q=https://gakko.pjwstk.edu.pl/edux/7542/lessons/62110/chapter/25905&sa=D&source=editors&ust=1714064099720281&usg=AOvVaw0oyhpC7Csh_BTJ6lCWpkZp)

# Introduction

In the previous lecture we learned about the concept of the relational data model. This model assumes that all the data is stored in the logical structures of tables. Its mathematical description comes from the relational algebra. The outline of this model was presented in the second lecture. In the fourth lecture we will discuss the problem of designing a relational database. In particular, we will answer the questions: why do we need to design database structures? How does the design process look like? What tools and notations do we use in the designing process? And finally - how do we create a database using a given model? During the WSI course we will present an outline of these topics. We will discuss them in depth during database related subjects like RBD, SBD and APBD.

### Learning outcome

*   Student knows the stages of the database design process, understands the role of these stages and knows what each of these stages involves.
*   Students knows what do we use the CASE tools for (especially in the context of databases).
*   Student understands the terms: “entity” as a representation of a real object and the model of a table in a relational database.
*   Student knows and understands the terms: entity, attribute, attribute domain, entity key.
*   Student understands the meaning of a relation as an ordered list of entities, the “parent” entity and the “child” entity.
*   Student is able to use the CASE tools to create a simple database diagram model consisting of a few entities.
*   Student is aware of various database diagram notations and knows the notation used in MS Visio.

# Draft of the database design process

In the database design process we can distinguish three main stages or three perspectives defining this process:

### The Concept design stage

At this stage we must define the demand for the project. We can say that this is the marketing stage in which we should decide what functions our customer needs and what his budget limitations are.

The drafts appearing at this stage are rather vague – they do not contain any details and do not choose any specific technology, but they need to be understandable for the customer and allow him to make corrections. We can compare it to the process involved in the process of designing and building a car.

### The Logical design stage

At this stage we transform the draft into a logical model. We create the model structure, specific solutions for the problem defined at the concept stage which will fulfil the client’s business needs. We design all the segments of the whole solution and define the connections between them. This time we can compare it to an architectural project with general plans but without the technical plans.

### The Implementation stage

At this stage we transform the draft into a technological model. We take into account all the constraints due to the available technology, but we must also fulfil all the conditions outlined in the logical design.

… and then we create the prototype, debug it, implement the solution and we can work on the next improved version.

As we mentioned earlier a database is usually a part of the whole information system – an important part but not the only one. Because of that it is important to consider the database design rules in the context of the whole system. On the other hand the process of creating the whole system must be preceded by a precise analysis which will give us answers to the following questions:

*   What is the subject of our project?
*   What is the purpose of our project, what kind of problems can be solved or improved by using our system?
*   What functions will need to be carried out within our project?
*   Who will be using these functions?
*   What kind of information will be stored in our database so that all the aforementioned conditions will be met?
*   What is the predicted cost of this solution?

From the database designer’s point of view the next to the last question concerning functionality of the future database is the most important one. However the answer to this question depends on the answers to the other questions.

The problems discussed above belong to the analysis stage  of the designing process.

Then comes the project stage , in which the future system documentation is written. We should also make a detailed description of the system’s functions and define its users (“actors”). At the same time we should outline the structure of the database in a way which guarantees the possibility to record all the required data. We should also define all the integrity constraints, guaranteeing the logical consistency of data.

The documentation of the system functions and the definition of the actors is often presented in the form of a use case diagram .

On the other hand, the implementation model of a database can be represented by the entity relationship diagram .

The third and final stage is the implementation .

This description should be sufficient to explain what the entity diagram is and what role it plays in the design process. This role will be explained further on.

# What is an entity relationship diagram (ERD)?

An entity relationship diagram  is a model which can represent a part of reality needed for the system and also the database structure. Just like every model it represents a simplification of the real or database object it describes. At the stage of preliminary analysis the objects needed for our database are identified. The role of the entity diagram is to create models of these objects and relationships between them. The graphic character of the diagram makes it easier to understand the database structure. It is important to understand the relationships between the database objects which can often be quite complicated.

The use case diagram presented in the previous lecture was basically the input data for graphical user interface (GUI). The entity relationship diagram has a different function as it is a model of the data structure. Thus, it puts aside client’s perspective of our application, or deals with it in a small extent.

There is a list of requirements for a proper entity relationship diagram. It should

*   Unambiguously present users’ requirements for the data stored in it,
*   Allow to check if the analyst fully grasped the users’ requirements and the character of the environment in which the system will be utilized,
*   Be much simpler from the database itself , as it puts aside the implementation details, which must be later developed by the database designer so that our database can exist and carry out its tasks.

### CASE (Computer Aided Software Engineering) tools

CASE tools are specialized programs which aid the designing of the information systems and allow to create various types of diagrams useful in the design process. The CASE tools provide graphic tools to design and draw diagrams on screen. The tools used to create the entity relationship diagrams must take into account the specific details of various database servers, for example the available data types. They should be (and usually are) able to translate the graphical version of the diagram into an SQL script. The script can then be run in the appropriate DBMS environment in order to generate all the database objects and integrity constraints.

In our lectures diagrams are made in Microsoft Visio for Enterprise Architects 2003.

### Entity

Entity  (lat. Entia ) – an entity is a singular, independent object which can be described and whose description can be stored in database. In the world of databases, the term entity is used to describe (model) things (objects phenomena, relationships etc.) about which we will collect data in our database. Every entity has a name that must be unique for a given database.

The definition of an entity consists of the attributes (characteristics, properties) which are sufficient to unambiguously distinguish an entity from the other ones.

We must distinguish the notion of entity as a class of objects and as an instance of this class, i.e. a single instance of the object (single copy) of a given type. For example the “PERSON” entity as a type defines attributes necessary to describe a certain group of people. Only after we substitute specific values for its attributes we obtain an instance of this entity which will represent a particular person. It should be emphasized that if the entity is used to describe a selected class of objects (in our example a specific group of people), each single object of this class (in our case each specific person) must be described with the same attributes. Note that it may be hard in practice to describe two different groups of people, e.g. a group of prisoners and a group of preschoolers, with the same attributes.

But the principle: Entia non sunt multiplicanda praeter necessitatem  (novacula Occami) - entities must not be multiplied beyond necessity  – known as the Occam's razor … also relates to the databases!

Entities are usually represented graphically as rectangles. The graphical representations of entities vary (slightly) according to the notation adopted by the specific CASE tool.

![image89](../Images/image89.png)

### Attribute

It is crucial to correctly choose the attributes for describing an entity. Note that attributes represent certain abstract features or characteristics, not the specific values. The attribute of the Student  entity is Name , not a specific value (say “Smith”) the attribute can take. The attribute should describe the entity rather than its relations with other entities, for instance in an airline’s database the attribute Seat\_number  should be an attribute of the Airliner  entity, not Passenger , despite the fact that the passenger sits on a specific seat during the flight. In the same way the place won by an athlete in a competition is neither an attribute of the entity Athlete  or Competition , but most preferably the Competition\_results  entity.

Consider now the entity as a model for future table in the database. It is clear that the attributes  are nothing else but the models for the future columns , specifying their names. If we also define their domains, i.e. we specify the data types we will use to store the values of the attribute, we will define the domains of the columns table.

### First Normal Form (1NF)

The concept of the “First Normal Form” (1NF) was formulated as one of the Codd’s rules. It is the first condition we must meet when we normalize the database structure. Its purpose is to eliminate any anomalies in the data insertion, modification and deletion as well as any uncontrolled data redundancy. The whole normalization process and the subsequent normal forms will be thoroughly discussed during the relational databases course in the future semesters.

An entity (and thus also its corresponding table) is in the first normal form if:

*   It describes one type (one class) of objects; e.g. the information about the car owners and their cars IS NOT  stored in a single entity that contains attributes of both the owners as well as the cars,
*   Its attribute values are elementary (atomic , indivisible) - each column represents a scalar (atomic) value rather than an array, list or anything that has its own structure; e.g. the Person  entity DOES NOT  include an attribute called Names  which contains all the person’s names stored in a list.
*   It does not contain collections (i.e. repeating groups of information); e.g. in order to store the information about sportsmen we DO NOT ADD  to the Athlete  entity an attribute called Medals  containing all the medals won by him or her.
*   It has a key, i.e. a set of attributes whose values distinguish each row from the other ones.
*   The order of the attributes should not encode any information, i.e. any change in the order of attributes should have no influence on the information content; e.g. in order to record information about the competition results we DO NOT  create an entity called Result  with attributes Athlete 1, Athlete 2, Athlete 3, ...

The above definition of the 1NF  is a bit of an over-interpretation of the original one. The latter consists only of the first three points, but I allowed myself to extend it slightly for the sake of the further argument. All the information above is true and correct .

### Key

The term "entity key"  describes a set of entity's attributes whose values are unique (unambiguous) for its every instance. Similarly, the term "table key"  describes a set of columns whose values will be unique (unambiguous) for every row in the table. Obviously it is possible that these sets contain only one element. Each table (entity) may contain none, one or more sets fulfilling the uniqueness condition, for example the Social security number  or the PESEL  can be the key in the Person  entity or the Registration\_number  in the Car  entity. However if there is no attribute with the uniqueness property in the entity we need to add an artificial attribute (column in the table) that meets this requirement. This is usually an attribute of integer type. The table column will then contain integers which uniquely identify the instances. But it can also be an attribute of the text type – e.g. the lecture code in the studies curriculum.

If the entity has more than one set of attributes whose values meet the requirement of uniqueness for every instance of the entity, then you should arbitrarily choose one of them to act as the primary key. If the entity has only one set, then there is no dilemma involved - it automatically becomes a primary key . Thus, we can identify a few keys in the entity, but only one of them can be used as our primary key.

Every CASE tool allows us to select the attribute (or multiple attributes) as the primary key during the design phase of our diagram. The illustration below shows this process in MS Visio.

![image22](../Images/image22.png)

### Data types – attributes domains

Data types or attribute domains are sets of values which can be stored by variables in the table columns. The principal types of data which we will encounter in every DBMS is the numeric type, the text type and the date type. For each of these types specific implementations provide a number of subtypes. For example: for a numeric type there is the two-byte integer and the four-byte one, the floating point number stored in four or eight bytes etc. Therefore we should find out what types are available before we start working in the specific DBMS environment.

When we speak about the entity-relationship diagram as a model of the future database we operate on the level of abstract concepts. On the other hand, on the database level we are closer to the concrete implementation. Hence, at the conceptual level (entity-relationship diagram) we are talking about the domain types as a general concept. However when we implement the database in a specific DBMS we use the types of data specific to the database solution.

CASE tools usually offer a choice of one of these approaches - either operate on universal data types not associated with a particular DBMS or choose data types implemented in the specific DBMS. MS Visio distinguishes between these two specifications of the data types. We can choose platform independent data types ( Portable Data Type ) or database specific data types ( Physical Data Type ).

The following illustration shows the selection process of the attribute’s domain (data type) from the drop-down list representing the physical data types (Oracle Server).

![image19](../Images/image19.png)

### Relationship

The relationship is defined as an ordered list of entities in the relational model. Individual entities can appear on the list multiple times. Each relationship defines a certain dependence between the sets of copies (instances) of the entities belonging to it. This correlation is called the instance of the relationship. In other words an instance of the relationship is the relationship between the entities instances. For example, the relationship between the Person  entities and the Car  entities can be described as the OwnerOfTheCar . Every instance of the Person  entity will be able to have a relationship with an instance of the Car  entity thus creating information about the cars and their owners.

The relationship can be formally represented using the relational notation: Z(E1 ,...,En) which means: entities E1 , ..., En  are included in the Z  relationship

You can also describe the relationship verbally, e.g.:

*   An employee works in a department  (relationship between the Employee and the Department entity)
*   An employee has a specific function in the project  (relationship between the Employee and the Project entity)
*   The company produces goods  (relationship between the Company and the Goods entity)

In practice, when designing a database, we define relationships through their verbal description.

### Binary relationship

Binary relationship  is a relationship that exists between two entities. It is represented graphically as a line connecting two frames (entities). An instance of a binary relationship  is a two argument relation in the Cartesian product of the entities instances collections.

The graph below shows the relationship between the Student  and the City  entities . This relationship can be described as follows: every student was born in a city, each student in ONE city, but… many students could have been born in ONE city.

![image49](../Images/image49.png)

After defining the relationship in the CASE tool (in our case MS Visio), the primary key from one entity forming the relationship is transferred to the entity on the other side of the relationship. This way we can create a foreign key .

In the first lecture we described the example of the Course  and Lecturer  tables and a relationship between them: for each course there is one teacher responsible, but one teacher may be responsible for several courses . In that example, the ID of a lecturer was placed in the Courses table and served as the indicator in order to determine which teacher is responsible for that item. A similar case is shown in the example above. The city ID (i.e. primary key of the City  entity) is placed in the Student  entity in order to indicate his or her place of birth. One instance of the Student  entity is associated with one instance of the City  entity, thus creating a single instance of a relationship.

Let us go back to the definition of the relationship as an ORDERED list of entities. The relationship in our example can be described as follows: ONE student was born in ONE city, but in ONE city MANY students could have been born. This definition is not symmetric! For each student you can specify one city where he or she was born, but for each city we can potentially find many students who were born in it. A relationship of this kind is called a one-to-many relationship. Here the entity City  is located on the ONE  side of the relationship and entity Student  on the MANY  side. We also use other names: Student  represents the child entity and City  represents the parent entity .

When we define a relationship in a CASE tool, an attribute is automatically added to the entity on the “many” side, containing the value of the primary key of the other entity. Thus we have added a foreign key  to the entity attributes. It will serve as a pointer linking the rows on the “many” side with one row on the “one” side of the relationship.

In our example MS Visio has automatically created in the Student  entity the attribute IdMiasto  (labeled FK1 - foreign key), defining the relationship between the instances of the Student  entity with the instances of the City  entity.

# Working with MS Visio

In the previous section we discussed the concept of an entity and an entity relationship. I tried to convey the meaning of these terms. However, as mentioned above, the practical process of creating the entity relationship diagrams is made using specialized CASE tools. In this section we present the Microsoft CASE tool called MS Visio. We discuss here a version of the MS Visio for Enterprise Architects included in the MS Office 2003, because it is the last version of this program equipped with full functionality we expect from a CASE program. We will also present the newer version MS Visio 2007, unfortunately already deprived of some of its functionality, but sufficient for the learning purposes within the WSI course. The MS Visio 2010, available for the students under the academic license at [https://software.pjwstk.edu.pl/](https://www.google.com/url?q=https://software.pjwstk.edu.pl/&sa=D&source=editors&ust=1714064099735460&usg=AOvVaw3-AYW-o4-iAxLXfCOi3vwh) , is almost identical. The latest version of MS Visio 2013, on the other hand, is not suitable for the tasks we will deal with during this course.

Below are short videos in the MP4 format presenting the basics of working with the MS Visio. These materials are not intended to teach you every detail of creating the entity relationship diagrams, but rather to demonstrate how to use this tool.

### Running MS Visio 2003

In links below are video files which present MS Visio use, which should be attached to the lectures. Z:\\PBD\_nagrania\\Uruchomienie Visio

### Running MS Visio 2010

Z:\\PBD\_nagrania\\Uruchomienie Visio 2010

### Creating entities with MS Visio

Z:\\PBD\_nagrania\\Tworzenie encji w MS Visio

### Creating relationships with MS Visio

Z:\\PBD\_nagrania\\Tworzenie związków w MS Visio

### But what do we need these diagrams for?

In this chapter we presented the process of designing a database by creating the entity relationship diagrams. We have already said that the entities and their relationships can be thought of as models of some parts of the real world, but at the same time they represent the structure of the future database. But do we obtain from such diagrams something more than just a convenient image of the database structure? Graphic representation of the tables and relationships makes it easier to work with the future database, but is it everything we get? It turns out that the CASE tools have one more (very important) function. Namely, they can generate a DDL script which creates a database. What is a DDL (“Data Definition Language”) script? This is a set of SQL text commands, and in fact also a subset of commands used for creating the database objects. The database server is able to interpret these commands and create a database whose structure has been designed in the form of the entity-relationship diagram.

Unfortunately, among the tools implemented by the currently available student version of the Visio 2010 there is no DDL generation tool. It is included in the MS Visio for Enterprise Architects (Visio 2003) and is available on the computers in PJATK laboratory. MP4 video below shows how to generate the DDL script of the entity relationship diagram in the MS Visio 2003.

### Generating DDL script from the MS Visio

Z:\\PBD\_nagrania\\Generowanie skryptu DDL z MS Visio

### Other notations used for creating entity relationship diagrams

As previously mentioned, there is no standard for the notation used in the entity relationship diagrams. You could say that every CASE tool introduces its own notation, although most of them are quite similar. However, the notation used in MS Visio (called relational) is quite distinct and rare. Below we present a few examples of the most commonly used notations. The first diagram was made in a relational notation, while the other ones were created in various notations different from the one used in MS Visio.

### Relational notation

We first encountered the relational notation while working with MS Visio - this is the basic notation used in this tool. The designations used are simple, yet the diagram contains little information in the graphic layer.

![image53](../Images/image53.png)

### IDEF1X notation

The same diagram made in MS Visio, but with the IDEF1X notation. Try to figure out what the signs mean. They will be thoroughly discussed in a different course called “Relational Databases”.

![image2](../Images/image2.png)

Once again, the same diagram made in the IDEF1X notation, but with a different CASE tool called Erwin. Unlike the previous ones it can represent an ambiguous relationship (many - to - many) on a diagram without decomposing it into two unambiguous relationships and an associative entity. Of course this will have to be done later at the implementation stage.

![image6](../Images/image6.png)

### Crow’s Foot notation

The name of this notation comes from the symbol of the "many" side of the relationship - the symbol of three lines which is similar to the imprint of a crow’s foot. This example was done using the IBM's Relational Data Architect.

![image64](../Images/image64.png)

# Summary

This lecture is an introduction to the design process of an information system, with particular emphasis on the design of the database. We emphasized the role of the CASE tools in the design process as well as the role of the entity-relationship diagram as a model of the future database. We presented and discussed the basic ERD elements: the entity, the attribute and the relationship and showed examples of the simple entity relationship diagrams in several different notations. The whole issue of the relational database design will be discussed in detail in a different course called “Relational Databases”.

# 4 Lesson V – SQL - relational database language

15.03.2024 11:45 | Number of chapters: 10

# New skills and knowledge

One of the Codd’s rules defining the requirements for the relational database model was introducing a complete language which, independently from other programming languages, would perform all the database operations. The Structured Query Language (SQL) was created in order to meet these requirements. The basics of this language will be presented in this lecture. After this lecture student should be able to: write simple commands for data reading, add a new record to the table, change data of the existing table. The student should also know the basic syntax of the commands which create and alter the table structure.

In the current lecture we will discuss the following topics:

1.  The origins of SQL
2.  The structure of SQL
3.  Data types according to the SQL standard
4.  The SELECT commands,
5.  The commands from the DDL and DML sublanguages.

Remember that the aim of this lecture is to give an overview of the topic. The details will be discussed more thoroughly in the courses called: Relational Databases and Database Systems.

### Learning outcome

*   The student can explain the role of the SQL language as a specialized language for relational databases, which is not a programming language
*   The student can name 4 sublanguages of SQL and can describe their application
*   The student can distinguish the data types provided by the language standard and point out the differences in their implementation in various database servers
*   The student knows how to use the basic version of the SELECT command together with the FROM and WHERE clauses and can write a simple SELECT command in a known and simple data structure made of at most two tables.
*   The student can use the DDL commands (CREATE, ALTER, DROP) and the DML commands (INSERT, UDATE, DELETE) in their basic scope.

# The origins of the SQL language

Earlier database models, such as the network or hierarchical models, were based on the notion of a file as a named collection of records. The traditional programming languages, like COBOL, PL/I or C, were sufficient for operating on these data structures. The appearance of the relational data model (Edgar C. Codd “Relational model of data for large shared data banks”, 1970) sparked the interest in specialized, “relational” languages which were supposed to implement the theoretical framework in concrete applications. The most advanced research was conducted in IBM, partially due to the fact that the relational database concept emerged in the IBM labs in San Jose. In 1974 the group led by Donald Chamberlin presented the Structured English Query Language, also known under the acronym SEQUEL. Its first, prototype implementation created by IBM appeared in 1974-1975 and was known as the SEQUEL-XRM. It was followed by another version of the language called SEQUEL/2 and in 1977 the SYSTEM R implementation was launched. The name SEQUEL/2 had to be dropped because of legal issues (the name was a trademark of a British aircraft company De Haviland) and the language was renamed SQL. The name soon lost its original meaning as an abbreviation and became the name of a new language.

The ANSI (American National Standards Institute) standard for SQL, which appeared in 1986, was based on the IBM dialect. The ANSI standard was adopted later by ISO (International Organization for Standardization) as the world standard in 1987. Since then SQL has been standardized a number of times and implemented in many DBMS with varying degree of ANSI standard conformity. To some extend each of these implementations uses its own dialect which differs in details from all others, although all of them remain similar in basic constructions.

The most popular DBMS’s implementing the relational database model are ORACLE, DB2, PostgresSQL, MS SQL Server, Sybase, MySQL. Each of them implements its own dialect of SQL, none of them satisfies all of the ISO standard requirements and no 2 are identical.

In the next part of the lecture and in the examples we will mostly work with the Microsoft implementation from the MS SQL Server 2008 R2 (called simply MS SQL further on). For comparison we will sometimes compare it to the ORACLE 11g implementation (ORACLE in short). If we do not discuss differences between the two, then this means that the differences are either insignificant or non-existent.

# The SQL language structure

Due to its name the SQL language is described as a QUERY database language. It is a simplified description, as this language also contains database COMMANDS. In this lectures QUERIES and COMMANDS will be used as synonyms.

The SQL is a declaratory language, which means that DBMS decides about the physical details of storing and operating on the data. The SQL is used only for database operations. Strictly speaking it is not a programming language, as it does not include the necessary programming structures (variables, conditional instructions, loop instructions). However the SQL implementations usually contain these structures because of their usefulness. We can thus distinguish the pure SQL and its procedural extensions. We will discuss two of those extensions further on: the PL/SQL (the procedural language of the ORACLE DB) and Transact SQL or T-SQL (the procedural language of MS SQL Server).

The SQL language structure. Queries – we distinguish four subsets of commands:

*   SQL DML  – Data Manipulation Language
*   SQL DDL  – Data Definition Language
*   SQL DCL  – Data Control Language
*   SQL DQL  – Data Query Language

### DQL – Data Query Language

The set of commands for reading the data from the database. All commands begin from the SELECT word and their execution doesn’t influence the state of data.

### DML – Data Manipulation Language

The set of commands responsible for data operations.

*   INSERT – entering new data (records) into the database
*   UPDATE – updating (changing) the existing data
*   DELETE – deleting data (records) from the database

### DDL – Data Definition Language The set of commands responsible for manipulating database objects.

*   CREATE – creating a new database object
*   ALTER – changing the structure of the existing object
*   DROP – deleting an existing object from the database

### DCL – Data Control Language The set of commands responsible for granting access to the database operations.

*   GRANT - granting access to a given database objects
*   REVOKE – revoking access to a given database objects
*   DENY – denies operations on a database object

### Control questions

Is it possible to change the database structure using SELECT instruction?

No

Yes

Check the answer

Which of the commands can alter data recorded in a database?

SELECT

ROLLBACK

UPDATE

GRANT

DELETE

# Data types in SQL

As we have mentioned, in the relational data model it is assumed that each column of a data table contains data of a fixed type. The SQL standard defines the basic data types, but the implementations sometimes depart from the standard in details.

### The SQL general data types

*   CHARACTER (n)  – fixed length string of characters
*   CHARACTER VARYING  – variable length string of characters
*   INTEGER  – an integer number
*   NUMERIC  - floating point number

Each implementation follows the general guidelines of the SQL standard, but each of them does it in its own way. We present below the data types for MS SQL Server 2012 and ORACLE 11g. Note that the MS SQL 2012 version contains a number of significant changes (not only concerning data types) in comparison to versions 2000 and 2005. We will not discuss data types which are not contained in the standard and are unimportant for us in this lecture, like BLOB or ROWID and other data types which are not so much used on the elementary level. Students interested in this topic may look it up on the software producers webpages ( [http://technet.microsoft.com](https://www.google.com/url?q=http://technet.microsoft.com/&sa=D&source=editors&ust=1714064099748657&usg=AOvVaw3-td0it3Sb5rINyc_K-Pdi) , [http://docs.oracle.com](https://www.google.com/url?q=http://docs.oracle.com/&sa=D&source=editors&ust=1714064099749084&usg=AOvVaw12DDmA9QTBTyqtLSMwcJ8r) ).

### Names of the SQL data types Character string data types

*   CHARACTER(n)  – string of fixed length n
*   VARYING CHARACTER(n)  – string of variable length, with maximum length n
*   BIT(n)  – string of a fixed bit length n
*   VARYING BIT(n)  - string of variable bit length, with maximum length n

Integer numeric data types

*   INTEGER – decimal or binary integer, signed
*   SMALLINT - decimal or binary integer, signed

Floating point numeric data types

*   NUMERIC(p,q)  – signed decimal number made of p digits in total, with the decimal point after q digits counting from right
*   DECIMAL(p,q)  – signed decimal number made of p digits before and q digits after the decimal point
*   FLOAT(p)  – floating point number (written in exponential notation)

Time and data types

*   DATE
*   TIME
*   TIMESTAMP
*   INTERVAL – specifies a time interval

The descriptions above have been taken from the standard description. In practice we work with types implemented by each database server. They differ from the standard in details. Therefore before you start working on a database on a given server you should find out what data types it supports. At the end of this lecture we give a detailed description of data types used by ORACLE and MS SQL.

# An example of the database – Emp, Dept and Salgrade tables

All examples of the SELECT command included in this lecture will be presented using the database consisting of the three tables: EMP , DEPT and SALGRADE , whose structure is presented in the graph below.

![image66](../Images/image66.jpg)

This simple graph presents a simplified structure of a company. The EMP table stores the company’s employees data, DEPT table stores the departments’ data and SALGRADE table describes the salary structure of the company.

The EMP table

*   Empno Int Primary Key -  employee’s number
*   Ename Varchar - employee’s surname
*   Job Varchar - employee’s position
*   Mgr Int Foreign Key - the employee supervisor’s number (a recursive relationship)
*   Hiredate Date - date of employment
*   Sal Int - salary (monthly)
*   Comm Int - the provision (annual)
*   Deptno Int Foreign Key - employee’s department number

![image79](../Images/image79.jpg)

The DEPT table

*   Deptno Int Primary Key - department number
*   Dname Varchar - department name
*   Loc Varchar - department location (the city)

The SALGRADE table

*   Grade Int Primary Key - classification number
*   Losal Int - the group’s minimum salary
*   Hisal Int - the group’s maximum salary

![image73](../Images/image73.jpg)

I would like to point out that the SALGRADE table is not connected via a primary-foreign key pair with EMP and the pair Losal - Hisal is just the salary brackets. In order to see in which group somebody’s salary (SAL) lies we need to find out into which Losal - Hisal bin the salary fits.

# SELECT instruction

The SELECT instruction is used for reading data recorded (or not recorded…) in the database, without changing its structure or content.

The SELECT instruction consists of a few “clauses” appearing in a strictly specified order and beginning with a keyword. The first clause, beginning with the keyword SELECT, and second clause, beginning with the key word FROM, are obligatory and therefore they must appear in the command syntax at least once (they can appear many times).

The SELECT instruction defines:

*   the sources for data reading in the database,
*   the conditions the data must satisfy in order to appear in the result,
*   in what form the result should be returned to the user.

Most language standards require SELECT (and every other instruction) to end with a semicolon “;”, although MS SQL treats this requirement as optional.

The SELECT instruction syntax

SELECT \[ DISTINCT \] wyrażenie (, ...)

FROM nazwa\_tabeli (, ...)

\[ WHERE warunek\]

\[ GROUP BY wyrażenie (, ...)\]

\[ HAVING warunek\]

(...)

\[ ORDER BY wyrażenie (, ...)\];

Every clause (except ORDER BY ) can appear in the instruction syntax more than once. SELECT and FROM clauses must appear at least once.

### SELECT instruction SELECT clause

SELECT clause structure SELECT \[ DISTINCT \] expression (,…) FROM table\_name (,…) (…);

The SELECT clause defines the data which are going to be read from the database and the way they will be presented. It can involve the column names, expressions (also referring to the column names) and constants unrelated to the database content. The expressions should be separated by commas. The column names should be prefixed with the table name: Table\_name. Column\_name If the column names are unambiguous then the name of the table preceding column name can be omitted. By unambiguous we mean here that the column name appears only in one table among those from which SELECT is reading the data.

### SELECT instruction FROM clause

The FROM clause defines the sources from which the data will be read. These can involve tables, views and other SELECT instructions. The names of tables, views and SELECT instructions (written in bracket) are separated by commas. In this lecture we will only discuss how to read data from a single table. Reading data from a view is not much different.

### SELECT instruction – elementary examples

We want to list the names, salaries and positions of the company employees: SELECT Ename, Sal, Job FROM Emp; The result is shown in the table below:

![image101](../Images/image101.jpg)

If we want to see the whole table we use: SELECT \* FROM EMP; or TABLE EMP; The last instruction is contained in the SQL standard, but not implemented in either ORACLE or MS SQL Server.

### SELECT instruction ORDER BY clause

The query’s results can be sorted either as ASCENDING (the default ordering, also abbreviated as ASC ) or DESCENDING ( DESC ). SELECT \[ DISTINCT \] phrase \[\[ AS \] alias\] (,…) FROM table\_name \[ WHERE condition\] ORDER BY phrase1 \[ ASC | DESC \] (,…); The ORDER BY clause can occur only once and it should always be placed at the end . The clause’s list can include expressions, also involving table names and their aliases as well as expression numbers in the order of their occurrence in the SELECT command. Sorting can be done according to more than on expression. The sorting hierarchy results from the order of the expressions on the list. The ASC word (pointing the default sorting direction) can be omitted in command’s syntax.

### SELECT instruction WHERE clause

The WHERE clause is the third clause in the SELECT syntax. It is optional - it does not have to appear. It allows to limit the records returned by the SELECT command using a logical condition. Only those records for which the condition is TRUE are returned, those with FALSE or NULL are eliminated from the result. Example. We want to list the names, positions and salaries of all the employees from department 10. SELECT Ename, Job, Sal FROM Emp WHERE deptno = 10; The command’s result is presented below:

![image9](../Images/image9.jpg)

### SELECT instruction – reading from multiple data sources

According to the SQL syntax if the data is supposed to be read from multiple tables (sources), the names of the tables, separated by commas, need to appear in the FROM clause. This was a theoretical introduction. Let us now see how it works in the SQL language. We will begin with an experiment. We will read the result below in order to find out the names and locations of departments for every employee. SELECT Ename, Dname, Loc FROM EMP, DEPT; The result is a bit surprising. There are 14 records in the EMP table and 4 records in the DEPT table and the query’s result includes 56 records. Let us analyze the result in more detail. According to this result each employee’s name appears 4 times in the table and is linked with the name and the location of every department. Thus, every department is displayed together with all the names of the employees. As a result we got the Cartesian Product of on the sets of rows of EMP and DEPT . Is this result correct? No, although it contains true information. The true records are those which line the employee’s name with the name and location of the department where he or she works. Since in our result all employees’ names are linked with all departments and locations we can be sure that the result contains the correct records as well. We just need to find them. Every record in the DEPT table includes the primary key in the form of the number in the Deptno column. If the employee works in a department then the record in the EMP table contains the Deptno value (foreign key) which points to the department in which he or she works. So if we want to read only the correct records we need to include the following condition ensuring that the Deptno value is the same in both tables: EMP.DEPTNO = DEPT.Deptno This way the SELECT command will omit those records for which EMP.Deptno <> DEPT.Deptno  or EMP.Deptno is NULL .

### Control questions

Which clause defines the data sources (tables) which should be read by the SELECT command?

SELECT

FROM

WHERE

ORDER BY

Check the answer

How many times can the clause ORDER BY appear in the SELECT command?

It needs to appear exactly once.

It can appear multiple times.

At most once.

Check the answer

What will be the number of records for the command SELECT \* FROM T1, T2; where T1 and T2 are the tables names including respectively 5 and 3 records?

0

3

5

15

Check the answer

What will be the result of the command below? SELECT ename FROM emp WHERE 1=1;

Empty set.

All names read from the EMP table.

Check the answer

What will be the result of the command below? SELECT dname FROM dept WHERE deptno = deptno;

Names of all departments read from the DEPT table

The command’s syntax is incorrect

The set is empty

Check the answer

If the SELECT command contains more than one table in the clause FROM:

The command’s syntax is incorrect.

The user should define a way the tables should be linked

Check the answer

# DDL – Data Definition Language

DDL is a subset of the SQL language which is responsible for database object operations such as creating, deleting and changing their structure. The DDL language includes three sets of commands beginning with the key words:

*   CREATE – create new object
*   DROP – delete object
*   ALTER – change the structure of the object

By a database object we mean tables, views, indices, procedures, triggers, databases and other objects. In this lecture we will only discuss operations on tables and integrity constraints. The concept of a view will be presented in the next lecture. The SBD course (another database-related course) will also discuss procedures. I would like to point out that the set of objects for which one can use the command CREATE depends on the implementation.

### Creating a new table

Commands for creating a new table: CREATE TABLE  table\_name ( Column\_name\_1 Data\_type \[Integrity\_Constraints\], Column\_name\_2… );

The table name  cannot exceed 30 signs ( ORACLE ), 128 signs ( MS SQL Server ). The column number  is also limited – up to 1000 ( ORACLE ), MS SQL Server  assumes that the table row length does not exceed 8060 bytes. The names of the tables, columns and other objects can only contain Latin letters, underscores and digits. Some dialects allow also letter with diacritics or spaces, but it is recommended not to use them.

### Creating a table – the integrity constraints

One way to introduce the integrity constraints, called the declaration in a single line, has been presented below: CREATE TABLE  table\_name ( Column\_name\_1 Data\_type Integrity\_constraints, …); Example: CREATE TABLE  Person ( PersonId INT PRIMARY KEY , Name VARCHAR (20) NOT NULL , Surname VARCHAR (50) ); Constraints are declared in the same line in which their column has been declared. Note however that this is not always possible. Another method is to declare constraints “outside the line” using the CONSTRAINT keyword. It allows to name the constraint: Example: CREATE TABLE  Person( PersonId INT , Name VARCHAR (20), Surname VARCHAR (50), CONSTRAINT PK\_Person PRIMARY KEY  (PersonId), CONSTRAINT UQ\_Person UNIQUE (Surname) ); If the constraints are not explicitly named, the DNBS will name them automatically. The examples were presented in the MS SQL Server  dialect. The ORACLE syntax is basically the same, except for the data type names.

### Changing the table scheme – the columns

Adding a new column to an existing table, changing the column’s data type, deleting the column MS SQL Server and Standard ALTER TABLE   Table\_name   ADD column\_name Data\_type; ALTER TABLE   Table\_name   ALTER COLUMN   column\_name Data\_type; ALTER TABLE   Table\_nsme   DROP COLUMN   column\_name; ORACLE ALTER TABLE   Table\_name   ADD (column\_name Data\_type); ALTER TABLE   Table\_name   MODIFY (column\_name Data\_type); ALTER TABLE   Table\_name   DROP COLUMN   (column\_name); The brackets are optional in the ORACLE syntax

### Deleting the table

DROP TABLE   table\_name;

If other tables have foreign keys referring to the table we want to drop and no referential action other than ON DELETE NO ACTION has been declared then the operation will fail.

### Control Questions

Command ALTER is used for:

Deleting the table from the database

Adding a new table to the database

Changing the data in the existing table

Changing schema (structure) of an existing table

Delete the data from the existing table

Check the answer

The word CONSTRAINT for the instruction CREATE TABLE:

Is optional

Is used for defining the integrity constraints

Must appear if we want to name the integrity constraints

Should not be used, as DBMS gives names for constraints

Check the answer

There are two tables in the database: T1 and T2. T1 includes the column t2 which is a foreign key from table T2. There are records in the T1 table which contain non-null values in t2. What will be the result of the command below? DROP TABLE T2;

Table T2 will be deleted

Records in T2 not referred to in T1 will be deleted.

The command will return an error.

Check the answer

# DML – Data Manipulation Language

The DML is the subset of the SQL language commands responsible for the operations on the database structure. These are: adding new records to the tables, modification of the existing data and deleting the records from the tables. Three kinds of commands are used: INSERT – add new record to the table DELETE – delete an existing record UPDATE – change data in an existing record

### Inserting data into the table

Basic (full) syntax:

INSERT INTO  table\_name (list of column names)

VALUES (values\_list);

Simplified syntax:

INSERT INTO  nazwa\_tabeli

VALUES (values\_list);

The number, types and order of the columns in the INSERT clause should match the list of values in the VALUES clause. The only columns which may be omitted are those which allow the NULL value, those which have a DEFAULT value defined, those whose value is calculated or realized by the auto-numbering mechanisms.

If we use the simplified syntax then the list needs to match the order and the types of data from all table columns, just like it was defined in the CREATE TABLE  command.

Example:

INSERT INTO  Emp (empno, ename, job, sal, deptno, comm)

VALUES (1001, ‘ WHITE ’, ‘ SALESMAN ’, 2500, 20, NULL);

MS SQL Server allows inserting more than one record in the INSERT operation:

INSERT INTO  Emp (empno, ename, job, sal, deptno, comm)

VALUES (1002, ‘ GREEN ’, ‘ CLEARK ’, 3100, 10, NULL),

(1003, ‘ YELLOW ’, ‘ MANAGER ’, 2500, 10, 200),

(1002, ‘ PINK ’, ‘ SALESMAN ’, 2200, 30, NULL);

This solution is not implemented by the ORACLE . Values in the VALUES clause   can include: the constants, the functions or the phrases.

The source for the INSERT instruction can be the SELECT instruction reading the values from the other tables. The SELECT instruction can also include the phrases.

Example:

INSERT INTO  Salary\_Budget (Year, Month, Sum)

SELECT 2011, 12, Sum (sal + NVL (comm, 0))

FROM EMP

In this case we already have the Salary\_Budget  table, and its columns’ structure is compatible with the SELECT instruction reading records, which will be written to the Salary\_Budget  table.

### Modifying the data in the existing table

UPDATE     table\_name

SET     column\_name = expression1 , ...  

\[ WHERE   condition\];

eg. to increase the salary of all salesmans by 10%:

UPDATE Emp

SET Sal=Sal\*1.1, Comm = 1000

WHERE Job = ‘ SALESMAN ’;

Omitting the WHERE condition will cause the modification of the data in all table records.

### Deleting data from the table

DELETE FROM table\_name

\[ WHERE condition\];

e.g. in order to delete all employees without the specified position:

DELETE FROM Emp

WHERE Job is NULL

Omitting the WHERE condition will cause deleting all the records from the table.

### Control Questions

Will the following command be executed: INSERT INTO emp (ename, sal, job) VALUES (‘PINK’, 1200, ‘ROBBER’);

No, because the company does not employ criminals.

No, because not all columns of EMP are filled

No, because we have not assigned any value to the empno column

Check the answer

Will the following command be executed: DELETE FROM dept;

Yes, all records from the dept table will be deleted.

No, because some of the rows of DEPT are referred to by rows of EMP.

Check the answer

The SALGRADE table contains 5 rows identified by the values 1-5 in the GRADE column. How many rows the will be changed by the command UPDATE salgrade SET Losal = Losal + 50 WHERE grade!=10 ?

All rows.

None.

One.

Check the answer

# Basic data types in the MS SQL Server and in the ORACLE MS SQL Server Exact numeric types

*   INTEGER or INT a sign integer type; range from-2^31 to 2^31
*   NUMERIC (p,\[s\]) or DECIMAL (p,\[s\]) a floating point number, where p defines signs’ number, s the number of signs after the comma; range from -2^31 to 2^31
*   MONEY a floating point number type representing the currency values; range from -922 337 203 685 477.5808 to 922 337 203 685 477.5807

Approximate numeric types

*   FLOAT (n) approximate floating point number, range from -1.79E+308 to -2.23E-308, 0 and from 2.23E-3+8 to 1.79E+308,
*   REAL approximate floating point number, range from -3.40E+38 to -1.18E-38, 0, 1.18E-38 to 3.40E+38.

Date and time types

*   TIME , format: hh:mm:ss\[.nnnn\], range 0.00 – 23.59.59.9999
*   DATE , format: YYYY-MM-DD; range: 0001-01-01 to 9999-12-31
*   DATETIME , fornat: YYYY-MM-DD hh:mm:ss; range: 1753-01-01 - 9999-12-31

Character strings:

*   CHAR (n): string of constant length, up to n characters; format: 1-8000 ASCII characters
*   VARCHAR (n): string of variable length, up to n characters; format: 1-8000 ASCII characters
*   nCHAR (n): string of constant length, up to n characters; format: 1-4000 UNICODE characters
*   nVARCHAR (n): string of variable length, up to n characters; format: 1-4000 UNICODE characters
*   VARCHAR (max): string of variable length; format: ASCII characters up to 2GB.

ORACLE

Exact numerical types

*   NUMBER (p,s): integer or floating point number, where p – maximal total number of digits (up to 38), s – number of digits after the decimal point
*   INTEGER or INT : integer, same as NUMBER(38)

Date and time types

*   DATE : stores the year, month, day, minutes and seconds

Strings

*   CHAR (n): string of constant length, up to n characters; format: 1-2000 ASCII characters
*   VARCHAR2 (n): string of variable length, up to n characters; format: 1-4000 ASCII characters
*   nCHAR (n): string of constant length, up to n characters; format: 1-2000 UNICODE characters
*   nVARCHAR2 (n): string of variable length, up to n characters; format 1-4000 UNICODE characters

# Summary

In this lecture, the last one dedicated to the relational databases, we have discussed the origins of the SQL language and its structure. We have given only an overview of SQL, enough to present what the language can be used for and what its basic instructions are. We have omitted a number of details, so the content of this lecture should be considered an introduction to the topic of SQL, which in turn will be discussed in greater detail in the two next semesters during the RBD and SBD courses.

# [5](https://www.google.com/url?q=https://gakko.pjwstk.edu.pl/edux/7542/lessons/62112/chapter/25920&sa=D&source=editors&ust=1714064099790569&usg=AOvVaw0Ucv6_XbWLfxOobO1zIUG6) [Lesson XI - Structure of a worksheet (spreadsheet), formatting and data entry in Excel](https://www.google.com/url?q=https://gakko.pjwstk.edu.pl/edux/7542/lessons/62112/chapter/25920&sa=D&source=editors&ust=1714064099790957&usg=AOvVaw3YtUTMPJF3m4cgsjEsmjoU)

[15.03.2024 11:46 | Number of chapters: 6](https://www.google.com/url?q=https://gakko.pjwstk.edu.pl/edux/7542/lessons/62112/chapter/25920&sa=D&source=editors&ust=1714064099791408&usg=AOvVaw2mULnL_-4ncgsCnjVyEnYp)

# Introduction In this lesson you will learn about the structure of an Excel worksheet and the basics of formatting and data entry. The application is widely used in companies and institutions, as well as by home users. It is mainly used to make calculations (e.g. expenditures) listed in a tabular form. In this use there are applied many logical functions (Lesson 3) mathematical, financial and database functions that are available in the program. Of a great importance is also semi-automatic copying of the created formulas using different variants of addressing (relative addressing, absolute addressing, mixed addressing). Excel is also used to create many types of charts (which we will learn about in lesson 2)which are useful e.g. in physics, mathematics and economics. It also contains a system of reports compilation in which the so-called pivot tables are used, used in the performance of business intelligence (Lesson 4).

### Learning outcome On having mastered the material of this lesson, the student should be able to easily enter and format data in Excel worksheets, make calculations (using operators and functions) and use semi-automatic duplication of the created formulas using different variants of addressing (relative addressing, absolute addressing, mixed addressing).

# Structure of an Excel worksheet (spreadsheet) and entering and selecting data

### Structure of a worksheet

Each document in Excel consists of worksheets .

An Excel worksheet (spreadsheet), is a two-dimensional grid with columns and rows . The column names are letters of the alphabet (A, B, C, …)and the rows are numbered chronologically (1,2,3 and so on).

The worksheet consists of cells i.e. small boxes, into which we can enter data. Each cell has its own address. We create it giving the name of the column and of the row in which the cell is located.

In the picture below cell A1 is selected.

![image107](../Images/image107.png)

The address of a cell is always displayed on the left of the Formula Bar

### Data entry

In Excel, we enter data directly into the cells. We click in the selected cell and begin typing. Entered digits will automatically move to the right side of the cell, and the text to the left. If we want to enter a decimal, we separate the integer from tens by a comma (never a dot!). This applies when we use the operating system with the Polish regional settings.

![image62](../Images/image62.png)

### Selecting cells

Before copying or formatting cells we have to select them. The cells can be selected as follows:

*   to select one cell click in it
*   To select one or more columns of cells, click on the column letter(s).
*   To select one or more rows of cells, click on the row number(s)
*   To select a group of contiguous cells, click in a corner cell and, with the left mouse button depressed, drag the cursor horizontally and/or vertically until all of the cells you want selected are outlined in black.
*   To select multiple cells that are not contiguous, press and hold the Ctrl key while clicking in the desired cells.

### CHECKING THE KNOWLEDGE:

In the picture below a cell is selected:

B2

2B

Check the answer

![image31](../Images/image31.png)

# Formatting cells

In this lesson we will discuss the issue of cell formatting.

### Basic formatting.

There are two ways of formatting the contents of the cells. The first is to select the cells and in the formatting window choose the "Main Tools" tab, then we can change the visual and aesthetic part of the worksheet by selecting the appropriate formatting category tab from the existing formatting group ("Font", "Alignment", "Number" etc.)

![image97](../Images/image97.jpg)

The second way is to right-click in the selected cells and select Format Cells window. There are different formatting options available on different tab groups.

The first tab is Number and contains categories for the type of data that is in the cell. Select one of these to set the appropriate cell format.

![image21](../Images/image21.jpg)

Applying different number formats, you can change the way of displaying numbers without changing them. The format of a number does not affect the actual value of the cell used in Excel to make calculations.

This value is displayed in the formula bar .

![image17](../Images/image17.png)

The following list contains information about available formats of numbers in the Number tab.

![image10](../Images/image10.png)

![image51](../Images/image51.png)

![image36](../Images/image36.png)

![image54](../Images/image54.png)

![image78](../Images/image78.png)

![image57](../Images/image57.png)

![image12](../Images/image12.png)

![image13](../Images/image13.png)

![image108](../Images/image108.png)

![image27](../Images/image27.png)

On the Alignment tab we set Orientation and Text Alignment

![image25](../Images/image25.jpg)

On the Font tab we set: Font name, Font style, Size, Color and whether you want the text to be underlined.

![image45](../Images/image45.jpg)

The fourth tab is Border. The Border tab provides a variety of border styles, To apply borders select the cells and then right-click and select Format Cells → Border. Select the border style and color first; then select the side or sides of the cell to receive the border.

![image44](../Images/image44.jpg)

To change the background color of a single cell or range of cells, select Format Cells → Fill or Patterns depending on the version of Excel.

![image1](../Images/image1.jpg)

### CHECKING THE KNOWLEDGE:

![image104](../Images/image104.png)

1\. What types of formatting were used in the above picture:

Numbers -> Percentage, Font -> Arial

Numbers -> Currency, Border -> outline, Fill

Numbers -> Fraction, Border -> outline, Fill

Check the answer

### Conditional Formatting

Conditional formatting allows you to automatically format cells, when they fulfill a certain condition. We can e.g. change the font color depending on what grade point average the student has obtained and thus select students with an average of more than 4.75.

To apply conditional formatting should be:

*   select the cells you want to format
*   select Format → Conditional Formatting
*   determine what condition are to be fulfilled
*   set the appropriate formatting
*   if there are more conditions, click the Add button
*   If all conditions have been added, click the Format button

![image76](../Images/image76.jpg)

### Example

There is often a need to highlight in the table some maximum or minimum values. This can be done by sorting the table, however, Microsoft Excel 2013 allows you to award the largest or smallest value without sorting.

At XYZ company an employee has to highlight the top 10 sales results.

First, you select the cells whose fragments you want to highlight. Then you choose Conditional Formatting in the Main Tools . In the menu that appears, you choose the option Top/Bottom Rules .

![image81](../Images/image81.jpg)

Click the Top 10 elements ... and in the window that appears, choose a value of 10 and the kind of distinctions.

![image86](../Images/image86.jpg)

At the same spreadsheet denote the color blue 30% of the smallest value. You choose the option Bottom 10% ... in the menu Top/Bottom Rules . In the window, enter the value 30, and select the desired way of formatting. Since we do not have to choose blue color fill, select Custom Format  ...

![image37](../Images/image37.jpg)

![image7](../Images/image7.png)

In the Font tab, Color option select a bright, visible on a dark blue background color. Then go to the Fill tab, where you choose the right color for the background.

![image14](../Images/image14.jpg)

After approval of the changes by pressing OK you get a fully formatted spreadsheet.

![image24](../Images/image24.jpg)

# Calculations, operators and functions

### Performing calculations

Calculations performed using Excel formulas. To enter a formula proceed as follows:

*   click on the cell in which the formula is to be entered
*   enter the formula (action) starting from the "="
*   type the formula using cell references
*   approve the formula of the Enter key

When you perform all calculations in Excel it is recommended to use cell references. This makes it easier and faster to make adjustments, and speeds up the job when we have a few similar calculations.

The formula appears in the formula bar , and the result in an   active cell .

![image83](../Images/image83.png)

If you want to make amendments to the previously entered formula, click the cell in which the formula appears and make changes in the formula bar.

The formula can be copied between the cells in the example below to get, in rows two and three, the product from columns A and B enough to "catch" the element and stretch it down. More advanced rules to copy formulas will be presented in point 5.

![image48](../Images/image48.png)

The cells can enter a formula using mathematical signs and pointing to the cells to be used in these calculations.

It is important to introduce the formulas which begin with the =

A collection of the most important operators and functions Excel spreadsheet:

|     |     |
| --- | --- |
| Operator | Explanation |
| +   | Adding |
| \-  | Subtraction |
| \*  | Multiplication |
| /   | Divide |
| \=  | Equal |
| <=  | Less than or equal |
| \>= | Greater than or equal |
| <>  | Different |
| ^   | Exponentiation |
| SQRT(x) | Returns the value of a positive square root |
| POWER(number;power) | Raises the number to the power |
| SUM() | Returns the sum the from the cells or range in brackets. Example SUM(A1:A10) or SUM(A2;D3;G5) |
| PRODUCT() | Returns the product the from the cells or range in brackets. Example PRODUCT(A1:A10) or PRODUCT(A2;D3;G5) |
| SUMSQ () | Displays the sum of the squares of the cells or range in brackets |
| EXP(x) | Returns e raised to the power of number. The constant e equals 2.71828182845904, the base of the natural logarithm. |
| LN(x) | The natural logarithm of x. x > 0 |
| Log10(x) | Displays the logarithm |
| Log(number, base) | Returns the logarithm of the specific basis |
| PI() | Returns the value of π |
| RADIANS(angle) | Converts degrees to radians |
| DEGREES(kąt) | Converts radians to degrees |
| Sin(), Cos(), Tan() | Sine, Cosine, Tangent (function arguments must be given in radians) |
| Ctg = 1/TAN() | Cotangent |
| FACT (n) | n!, n > 0 |
| COMBIN(n;k) | Displays the number of combinations of k - of element of a set of n - element |
| COUNTIF(range, criteria) | Counts the number of cells within the range that meet the given criteria |
| SUMIFS(sum\_range, criteria\_range1, criteria1, \[criteria\_range2, criteria2\], ...) | Adds all of its arguments that meet multiple criteria |

### Examples

We already know the basic operators and functions of Excel. Now let us discuss a few practical examples:

![image50](../Images/image50.png)

In Excel to calculate the root of grade 4 of 7 belong to convert it first to another character, because Excel does not provide a feature that allows you to calculate the root level 4 (during practical tasks often is the case, why should then remember the lessons of mathematics in school and properly transform equation).

2\. Calculate the cos of 27 degrees. As we know the arguments of trigonometric functions in Excel, should be given in radians. In that case, solution to the problem should look like this: a)Transform 27 degrees to radians, b)Put the result of the trigonometric function. Solution : Cos (radians(27)) 3. In how many ways can a 16 person group set in a series of pairs? To calculate the result of this task should use the so-called permutations of a set: 16! Solution : FACT(16) 4. In how many ways can you select a 6 person volleyball team from a 16 people group? It is indeed one of the most difficult tasks, therefore let's we apply the so called Newton's symbol:

![image80](../Images/image80.png)

5\. How to calculate:

![image88](../Images/image88.png)

Solution : sqrt(sin(radians (25))+ 2)/(cos(radians(45)+2) 6. XYZ company employee was asked to count the total sales of the three products. You enter data to Excel Sheet by selecting the cell and typing data directly  in the cell  or in the  formula bar  (indicated by arrows in the figure below).

![image60](../Images/image60.png)

 After setting the active cell D8 let's enter in the cell the formula summing sales of these three products. This can be done in many ways, for example by typing in D8 to the formula = SUM ( D5: D7 ), or by entering = SUM ( and selecting the interesting range of the mouse ), but the best standing on the field select the icon of the sum, which is on the card  'Formulas'. The values you are searching for will be automatically summarized. The spreadsheet should look like as it is shown below. In this way we can also introduce other functions - financial, logical and others.

![image91](../Images/image91.png)

### Checking knowledge:

1\. In how many different ways can you select 3 people to go to the cinema out of a 7 person group? What formula will you type in Excel?

COMBIN(7;3)

COMBIN(7,3)

COMBIN(3;7)

# The relative and absolute addresses

As it has been mentioned earlier cell ADDRESS  is a pair that specifies clearly a cell in the spreadsheet. It arises from the number of column and row sheet. The columns are numbered with successive letters A, B, C, and the rows - consecutive numbers 1,2,3; eg. a cell in the upper left corner of the sheet has the address A1. Addresses of the cells act as variables in formulas (formulas called) entered into the worksheet cells. As a result, the change in value in 1-wszej cell can be automatically reflected in the other cells. you can distinguish three types of addresses spreadsheet cells, typed into formulas - their type is indicated by the $ sign: Absolute - in this addressing the specific cell address is important, not its position relative to other data. Add the cell address $ signs in front of the letter of the column and before the letter indicating the row eg.  $A$1 . As a result, the cell address will not change. Such addressing is used, for example when the value of a cell refers to a number of data: Example 1:

An employee at XYZ has the task to calculate the price of goods in PLN in terms of Euro. Solution: You will get this value by multiplying the price of the goods in Euro (B4:B12) by Euro exchange rate (in cell B1). To all the values in column B multiplied by this one particular cell must address it as an absolute address: formula takes the form: = B4 \* $B$1 . You can copy such a form without any changes.

![image40](../Images/image40.jpg)

Relative - Addressing is used by the program as default. Addressing utilizes the relative position of the cells relative to each other and not their specific addresses. It is taken into account the position of the cell in which it is entered formula containing the address. Sheet remembers the location of the cells whose addresses appear in the formula, relative to the cell containing the formula. $ Character does not occur . Example 2: In columns A and B are the data series, in column D we obtain the products of the two pairs of the series. Solution: To do this, in the cell D1, enter = A1 \* B1 , this formula can be copied to other cells in column D. This is possible thanks to this the program at that addressing only checks the relative position of the cell with the formula to each other, so the formula is copied down to the next cell will use a modified version of the formula as =A2\*B2 and so on.

![image103](../Images/image103.jpg)

Mixed - Address mixed cell is a combination of an absolute and relative address. It is used when the values have to refer to a particular column or row. If we mean to indicate a specific example of the column address will be the character $A1 , and in the case of a particular row becomes A$1. This distinction is important in the transfer (copying) formulas between cells. This part of the address, which is not subject to change should be preceded by a $; eg. the absolute address cell A1 has the form $A$1 , and copying formulas with the address he remains always the same. In the mixed address only one part is preceded by a $ and does not change when you copy a formula. Example 3 In column A the data to be multiplied by the value of the other two columns. Solution: To make such an operation should be time to enter a formula into cell D1 = $A1 \* B1 and then copy it without modification to the other cells down or right, use addressing mixed in the form of: $=A1\*B1

![image59](../Images/image59.jpg)

### CHECKING THE KNOWLEDGE:

Which of the following formulas satisfies receiving the following multiplication table in two movements, copying the formula - the formula enter into the B2 and then copy to the right and the whole row down.

A \* B $ 2 $ 1

$ A2 \* B $ 1

A \* B $ 2 $ 1

$ \* $ A2 B1

$ A $ 2 \* B $ 1

$ A2 \* $ B $ 1

Check the answer

![image96](../Images/image96.png)

# Summary

In the above lesson we presented the basis for the introduction and formatting data in Excel spreadsheets, making calculations (using operators and functions) and the use of semi-automatic copying using different kinds of addressing (relative addressing, absolute addressing, mixed addressing). It should serve as a good kickstart in learning Excel spreadsheet.

[](https://www.google.com/url?q=https://gakko.pjwstk.edu.pl/edux/7542/lessons/62112/chapter/25920&sa=D&source=editors&ust=1714064099831425&usg=AOvVaw2xEoAxZXPyqlMcJNxIp_ki)

# [6](https://www.google.com/url?q=https://gakko.pjwstk.edu.pl/edux/7542/lessons/62113/chapter/25926&sa=D&source=editors&ust=1714064099831931&usg=AOvVaw3zRvWr1OB990xl6Iz4z8vx) [Lesson XII - Charts in Excel - Basics](https://www.google.com/url?q=https://gakko.pjwstk.edu.pl/edux/7542/lessons/62113/chapter/25926&sa=D&source=editors&ust=1714064099832313&usg=AOvVaw35bOX1v7tpzNyRxyWiCE1l)

[15.03.2024 11:46 | Number of chapters: 5](https://www.google.com/url?q=https://gakko.pjwstk.edu.pl/edux/7542/lessons/62113/chapter/25926&sa=D&source=editors&ust=1714064099832747&usg=AOvVaw28NsW7F4dRIk5E0pu1vLCr)

# INTRODUCTION

Often we need to illustrate our calculations with a chart- particularly when it is about different kinds of analyses and computer simulations. One chart is better than a thousand numbers. This lesson will provide step- by –step directions how to create basic charts in Excel.

### Learning effects

Once the material of this lesson has been mastered, the student should be able to create basic Scatter or Pie Charts in Excel based on entered or acquired data.

# SCATTER CHART

\[FILM\]

We need to create a table with data

In today's class we will work on a task for mathematical analysis class. The result of our work will be a common, standardized chart of five math functions.

We have a given function formula: y = 2x 2  - 3x - 2 x € <- 20 20>

1\. The first step is to create a table with data which Excel will use to create a chart. 2. Fill in the table with a series of number values for x-s - dragging like while copying formulas:

![image72](../Images/image72.png)

up to 20. . .

3\. Fill in the values for y 1:

![image41](../Images/image41.png)

Then we drag the formula to the bottom, so that Excel calculates y for all x-s.

Creating and editing the chart

4\. Having a ready table select values of all y-s and on the "INSERT" tab choose "SCATTER CHART ":

![image90](../Images/image90.png)

To draw charts of mathematical functions usually SCATTER CHART is used(position II or III). In this example we will apply position II. Click on the second position and the chart will be created. 5. Unfortunately, the chart we have created is incorrect so we need to change the values of the data series. First, to make our work easier we need to move the chart to another worksheet. To do this, right-click on the chart and from the context menu select "MOVE CHART":

![image56](../Images/image56.png)

Select "Worksheet 1" and click "Ok". Automatically we will get moved to the second spreadsheet. 6. Now dragging the corners of the chart to the sides we can stretch it to full screen. This way it will be more comfortable. Then right-click on the chart and from the context menu choose "Select data". You will be moved to the first worksheet and the window "Select Data Source” will appear :

![image75](../Images/image75.png)

7\. Select the "y 1" s and click the "Edit" button. 8. "Edit series" window will display.

![image52](../Images/image52.png)

9\. First select in the first text box "Name of series." We need to enter the name for the series. To do this, select the cell B1 (there we have entered the name of the series as "Y1"). So click on the graphical icon at the end of the form box and switch to the first worksheet (you can do this by clicking on the appropriate tab in the lower left corner of Excel window). 10. Now select cell B1 and again click on the icon at the end of the form box.

![image69](../Images/image69.png)

11\. The next step is to provide the values of X series. At the beginning we go to the form box and click the icon at the end. Now select all values of X (from -20 to 20). And again, click on the icon at the end of the text box. Then click twice "OK". The chart will display correctly now.

![image32](../Images/image32.png)

Add values of another function to the existing chart

12\. At the beginning we have to add one more column to the existing table. We will call it y2:

![image42](../Images/image42.png)

13 .The next step is to calculate y, according to the function formula. Let’s say the formula is this: y2 = (x-1)/(x+2) It should be noted that the argument of the function -2, does not belong to the domain. Later you will find out what to do about it. 14. Enter the appropriate formula in the cell C2 and drag it to the bottom so that Excel calculates the values of y2 for all x-:

![image70](../Images/image70.png)

15\. In the cell C20 the message "# DIV / 0!" is displayed which means that you cannot divide by 0. To get the chart drawn correctly, the cell C20 should be left empty, delete its contents by using "Delete" button. If while executing the tasks, messages "Number" or "DIV / 0!" are displayed , we delete them leaving a given cell empty. 16. Having prepared the table, right-click on the graph and select from the context menu the option "SELECT DATA ...". 17. Then click "Add" button and following the same pattern as for correcting data in the previous exercise, give the name of the series (cell C1), select the value of all x-s (from -20 to 20). 18. In the box "Values of Y series" delete everything that is typed and select all values of y2. Double click "Ok". 19. It’s done now! We have added to the chart another data series called "y2". 20. Now to make the chart look better you move the mouse cursor on the axis and right-click. From the context menu choose "FORMAT AXES". 21. In the text box "minimum" enter value "-7" and in the text box maximum enter value "7"

![image99](../Images/image99.png)

22\. Click "OK". The chart is ready:

![image95](../Images/image95.png)

# Exercises

To the created example add data series of function with a formula as below and move to the folder TASKS BY ...:

Homework

1.  y3 = (sin^2 x)/x
2.  y4 = (tg(x))/(x+1)
3.  y5 = ?(x-2)

### Checking knowledge:

The data for the chart are taken from:

all selected cells

Selected cells, but only those in which there is a number

From cells with content (to be explained to students)

Check the answer

### Pie chart

We were asked to prepare a pie chart with information about the most popular browsers in the world according to their percentages expressed in integral numbers - data for 2011. The leading browsers in the world are as follows (December 2011 according to the StatCounter website) Internet Explorer - 38,64%. Google Chrome - 27,27%. Mozilla Firefox - 25.29%. Safari - 6.08%. Opera - 1.98% Others - 0.74% Select the table and on the 'Insert' tab select the Pie chart and subtype 'Pie chart 2-D'. 2-D Pie Charts are clearer, unfortunately due to the attractive form of 3-D Pie charts they have become much more popular and the audiences expect them.

![image38](../Images/image38.png)

Finding products using small squares with their colors in the legend is very tiring, and when there are a lot of elements or if someone finds it hard to differentiate similar colors it becomes almost impossible impossible. Click on a '+', uncheck the 'Legend', select the 'Data Labels', then click an arrow at the 'Data labels' first select the 'End of an external' and 'More options ...'.

![image30](../Images/image30.jpg)

In the 'Format Data Labels' mark: - 'Category Name' - so that we know which part of the pie applies to a given product. - 'Percentage' - here there is calculated and given an approximate percentage of the total figure Uncheck: - 'Value' - in order to eliminate unnecessary decimals There is a default option 'Show lines leading' - useful for large quantities of pie slices, so that the lines leading the clippings labels are connected. Both messages displayed on the labels are separated by new line marks, and we can change it in the 'Separator' menu. In this window, it is also possible to change the position of labels and change the format of numbers.

![image3](../Images/image3.jpg)

As in all charts we can also use the styles and colour palettes, which are available when you click the Brush icon.

![image46](../Images/image46.jpg)

A colour slice can be changed by clicking on it twice individually (with a break between clicks) which will result in the selection (small circles), then click it with the right button and choose the colour changes which are visible on the chart when you move the mouse cursor over the colours.

![image71](../Images/image71.jpg)

To eject the selected clipping simply select it and drag it from the centre of the chart. It is used to draw the attention of the recipient precisely on this passage. After bolding the data labels and writing the title, the chart will look like in the figure below.

![image61](../Images/image61.jpg)

In order to get rid of the graph frame right click it, and choose the command 'Format chart area ...'

![image92](../Images/image92.jpg)

In the 'Format the Chart ' window choose 'No Line'. Close the window.

![image65](../Images/image65.jpg)

At any time we can change the chart type by right clicking and selecting 'Change the chart type ...'.

![image8](../Images/image8.jpg)

Now let’s choose a 3-D pie chart.

![image33](../Images/image33.jpg)

For 3-D charts, there are many styles, you have to adjust yourself the right one for the job.

![image5](../Images/image5.jpg)

By right clicking the chart and selecting 'Rotate 3-D' we will be able to choose how to position the chart, which will highlight the fragment we want.

![image82](../Images/image82.jpg)

WARNING: Increasing Prospects makes the graph less clear, and the section which is at the bottom seems larger than it actually is.

![image84](../Images/image84.jpg)

### CHECKING THE KNOWLEDGE:

Graphs can be displayed:

Only in the spreadsheet where the data comes from

Only in the data spreadsheet and chart spreadsheet

You can view ae graph in each of the existing spreadsheets and make it a spreadsheet of the chart

Check the answer

### Summary

In the lesson we presented the basics of creating charts in Excel. Once you have mastered the material you should be able to create charts in Excel. This of course does not cover the whole subject of charts therefore we encourage self-experimentation.

[](https://www.google.com/url?q=https://gakko.pjwstk.edu.pl/edux/7542/lessons/62113/chapter/25926&sa=D&source=editors&ust=1714064099844559&usg=AOvVaw3G_R3CvDglQebok4kR9CfA)

# [7](https://www.google.com/url?q=https://gakko.pjwstk.edu.pl/edux/7542/lessons/62114/chapter/25931&sa=D&source=editors&ust=1714064099845003&usg=AOvVaw26J_nOFrOIJ7xjKr76XaU4) [Lesson XIII - Introduction to Excel logical functions](https://www.google.com/url?q=https://gakko.pjwstk.edu.pl/edux/7542/lessons/62114/chapter/25931&sa=D&source=editors&ust=1714064099845320&usg=AOvVaw1Shk9ng67XbmthP5xB3mYw)

[15.03.2024 11:46 | Number of chapters: 6](https://www.google.com/url?q=https://gakko.pjwstk.edu.pl/edux/7542/lessons/62114/chapter/25931&sa=D&source=editors&ust=1714064099845724&usg=AOvVaw3G40l7tG-rdLYaPNTIXUNW)

### Introduction

The logical functions in Excel are extremely useful, and often indispensable in everyday work. It is hard to imagine a serious spreadsheet e.g. without built-in IF function. The logical functions are primarily used to check whether the values entered in the worksheet’s cells meet the conditions. Only rarely are they used alone, most often they are nested in formulas, being arguments for other functions (often they return a table of numerical values as a parameter for mathematical or statistical functions).

### Learning effects

Once the material of this lesson has been mastered, the student should be able to easily solve the basic problems associated with the use of logical functions in Excel. For example : "Create a formula that will grant a discount on monthly tickets or not, according to the following principles: People who are entitled to discounts need to meet two conditions simultaneously: a) be retired b) their monthly income per capita cannot exceed 600 zł " \[FILM\]

### Basics of logical functions

TRUE() This function has no arguments, it always returns the logical value TRUE. You can also enter this value directly into a cell or formula. FALSE() This function has no arguments, it always returns the logical value FALSE. You can also enter this value directly into a cell or formula. Both of these functions seem to be absolutely unnecessary in Excel and have been introduced in order to comply with other spreadsheets. IF() This function checks the logical condition specified in the first argument of the function. If the condition is fulfilled (TRUE) then the value of the second argument is returned, and if not (FALSE) - the value of the third argument is returned. The syntax of the IF function () is presented below: • logical-test - to check the logical condition of a value or expression, the result of which can be calculated as a logical value (TRUE or FALSE). The logical condition often uses logical comparison operators such as =,>, <,> =, <=, <> to show the values of cells. For example, B2 = 9 is a logical expression; if the value entered into cell B2 is actually number 9, this expression will be evaluated to TRUE, in any other case, the expression will have the logical value FALSE • value\_if\_true - the second argument of the function is the value returned when the first argument logical\_test is met. If our logical test is the expression B2 = 9 and in the cell B2 there is in fact number 9, then the result of the function - the value of the second argument - may be a text message "in this cell there is number 9". This is an optional argument that can be omitted by placing two semicolons after the first argument. Omitting it indicates that it is a default argument, whose resulting value is TRUE • value\_if\_false - the third argument of the function is the value returned when the first argument logical\_test returns the value FALSE. If our logical test is still the expression B2 = 9, and in cell B2 there is a different value (number, text, error, logical value) or the cell is empty, the result of the function (the value of the third argument) can be a text message "the value of this cell is different from number 9". Leaving the argument empty will result in returning the value FALSE. Two optional arguments CANNOT be omitted at the same time, at least one of them should be determined The use of IF function is presented below

![image67](../Images/image67.jpg)

\=IF(B2 = $ 9; "in this cell is number 9"; "the value of this cell is different from the number 9") The result of the function is presented depending on the value of the cell on the left side of the formula. Only in one case, the logical expression is true. Excel does not apply automatic conversion here and properly distinguishes numeric values from the text, that’s why number 9 that is preceded by an apostrophe is treated as text (logical condition returns FALSE, while the formula - the text that is included in the third argument of the function value\_if\_false).

### Examples of logical function IF ()

The first example shows the logical condition with statistical function. Apart from the comparison operator that has been mentioned above we use here statistical function AVERAGE (). The task is to reward students who have obtained the average grade of at least 4.50 in the given subjects - they are entitled to a scholarship for their academic performance.

![image85](../Images/image85.jpg)

The formula in cell F4 checks the average of four subjects and it looks like this: =IF(AVERAGE ($B4:$E4)>= 4.5; "yes - "&TEXT(AVERAGE($B4:$E4);"0.00"); "no - "&TEXT(AVERAGE ($ B4: $ E4), "0.00")) The most important in this case is the logical condition, that is checking whether the average of the four subjects is higher than or equals 4.50. If this happens, the formula returns the text "yes –“ and shows the average grade for the student, otherwise it returns the text "no -" together with the average grade. Another way is to create two separate columns: average grade, and information about the scholarship (in this case, it is possible e.g. to sort by average). The second example shows nesting of the function IF (). Some logical problems can be solved only after multiple nesting of this function e.g. when the need to allocate the grade according to the value range in which the score is. Below there is a table in which students were assigned grades according to the number of points obtained in the exam. The formula for cell C4 is: = IF ($ C4> 18; "very good"; IF ($ C4> 14; "good"; IF ($ C4> 10; "satisfactory", "unsatisfactory")))

![image15](../Images/image15.jpg)

It is worth to remember a few important things: • The IF () can be nested up to 7 times in a formula in Excel 2003. For Excel 2007 you can nest it up to 64 times, but the formula will not work correctly in the earlier versions of Excel, so it is advisable to use up to 7 nestings in a single formula. In case of our formula the function IF ()has been nested three times. • The second instruction of IF function () is simultaneously an argument value\_if\_false for the first instruction of the function (view 4). Similarly, the third instruction of IF function () is an argument value\_if\_false for the second instruction and so on.

![image29](../Images/image29.jpg)

• The formula checks the first logical condition and stops when it returns TRUE (as a result it returns the value of the second argument). If the returned value is FALSE - the formula moves to the second condition etc. In our example (score = 11), the first condition $ C5> 18 is false, the second $ C5> 14 also returns FALSE. Only the third $ C5> 10 is met - the result of the formula is thus the word "sufficient".

• For any number of points lower than 11 each of the three conditions returns FALSE. In such situation (in another case)the formula returns the word "unsatisfactory".

### The AND () function - Expansion function IF ()

### AND()

The AND () works in conjunction with IF (), extending its operation. IF () in basic form operates only one logical condition, while the AND () allows you to enter up to 30 logical conditions. To perform function as a result of TRUE, it is necessary that each of the conditions, function arguments, he was satisfied. If at least one of the accepted conditions is FALSE, the function returns a result of FALSE. AND () it is therefore, in other words, the product of (a conjunction) conditions. Be very careful to keep all function arguments logical values using other types of values, as very simply, you can generate an error. Using arguments and empty text is permitted only in particularly justified cases - only if the second argument is a reference to an empty cell or one that contains text, the formula will work - the data entered in the parameters manually generate this error #VALUE !. The following table is presented on the basis of which in a very useful function can be used, AND (). The task concerns the selection of candidates for the position of Analyst in our company. In total, it reported seven people who were tested in various fields. The assumption is that we are interested in people who are very familiar with English, Excel, and have obtained at least 15 points in our test checking the knowledge of controlling. If the candidate meets all these conditions, it is admitted to the second stage of recruitment; otherwise eliminated.

![image77](../Images/image77.jpg)

The formula contained in the H4 as follows: = IF(AND($C4>14; $D4="yes";$F4="yes");"Stage II", "Not applicable") • For the first person formula returns the text '' Void '' because it was not satisfied with the conditions of the other very good knowledge of English. Although the other two conditions have been satisfied - AND function () returns a result of FALSE, and the function IF () converts a specific text message.

### The OR () function - Expansion function IF ()

### OR()

The OR () - like function AND () - interacts with function IF (), allowing for a more extensive tests. If you want the function to pay as a result of TRUE, it is required that at least one of the conditions, function arguments, he was satisfied. If all of the accepted conditions are FALSE, the function returns a result of FALSE. OR () it is therefore, in other words, the sum of (alternative) conditions. Using arguments and empty text it is handled by a function similarly to the function AND (). The following tables present the same as for the AND () but with different results. This time we carry out recruitment for the position of Specialist. Database, because the eligibility criteria for the next stage are different. The candidate this time must meet two conditions: be fluent in Access, and at least one of the two languages.

![image16](../Images/image16.jpg)

The formula contained in the H4 as follows: = IF(AND($G4="yes";OR($D4="yes";$E4="yes")); "Stage II";"eliminated") • Here we have a combination of conjunctions and alternative conditions. Conjunction is that the candidate must meet two conditions, an alternative that requires a good knowledge of any foreign language.

### CHECKING THE KNOWLEDGE:

![image105](../Images/image105.png)

a) =IF(AND(G12="yes";E12<=600);"discount";"without discounts") b) =IF(AND(G12<600;OR(E12="yes";F12="yes")); "discount", "no discount") c) = IF (AND(G12<=600;OR(E12="yes"; F12="yes")),"discount","no discount") - AND at the beginning because we have to choose options A and B and then oR (students or retirement) and G12<=600 (not to exceed 600 zł)

### Summary

In addition to the IF function () all logical functions return as a result of the logical type TRUE / FALSE. The IF () can be used in many different ways: by means of nesting you can check a number of different conditions; treating each cell in the range as a parameter to a function of mathematical, statistical or information, you can make calculations (eg. to count or sum up) only in those cells that meet certain criteria. Functions AND () and OR () operate on individual cells and allow you to develop logical tests, which are very often used in the making of advanced formulas. We encourage you to own adventure with logic functions.

Test In the attached file SXXXXX-WSI-INTERNET-TEST-EXCEL-LOGICAL-FUNCTIONS.xlsx Scoring max 10 0.5 + 1 + 2 + 2 + (9 \* 0.5)

[](https://www.google.com/url?q=https://gakko.pjwstk.edu.pl/edux/7542/lessons/62114/chapter/25931&sa=D&source=editors&ust=1714064099852767&usg=AOvVaw1CgLS4F4wjsP7_gMf58xmF)

# [8](https://www.google.com/url?q=https://gakko.pjwstk.edu.pl/edux/7542/lessons/62115/chapter/25937&sa=D&source=editors&ust=1714064099853247&usg=AOvVaw0-o_RkUI_9SS7J6x1IrBB9) [Lesson XIV - Pivot tables basics](https://www.google.com/url?q=https://gakko.pjwstk.edu.pl/edux/7542/lessons/62115/chapter/25937&sa=D&source=editors&ust=1714064099853572&usg=AOvVaw2mDu0QnmAdDQNiYGjNiWFC)

[15.03.2024 11:46 | Number of chapters: 4](https://www.google.com/url?q=https://gakko.pjwstk.edu.pl/edux/7542/lessons/62115/chapter/25937&sa=D&source=editors&ust=1714064099854001&usg=AOvVaw0X6KAIDWgR5xI8bdVkK-yk)

### Introduction

Excel pivot table is a powerful analytical tool. The main functionality of pivot tables that is used, is the possibility of a quick, easy and transparent summary and analysis of large data sets. However it is not the only functionality of pivot tables

### Learning outcomes

Once the student has mastered the material of this lesson, they should be able to easily create pivot tables according to the set purpose (e.g. What is the sales figure by certain regions and years?) out of the given data file (e.g. sales volume) and modify the created tables as needed.

### Pivot Table out of data file

2 Source data - Excel i movie

To create a Pivot Table we will use the file "PivotTable-Data.xlsx" After opening the file the content is displayed as it is shown below.

![image23](../Images/image23.jpg)

The data have been generated in such a way that each row contains information about the sale, purchase, plan, price, quantity and margin. To these data there are assigned: branch, region, date of sale and the information on the sale (resulting from the date). Note that the figures are formatted.

The goal to achieve

At the beginning we set ourselves an easy goal, in order to make aquiring information about Pivot Tables nice and easy:

### What is the value of sales by individual regions and years?

The task that we need to do can be easily accomplished using other built-in Excel functions, let’s say SUM.IFS. function. My goal is to show the possibilities of a Pivot Table, not to convince anyone that this is the only appropriate tool for summarizing and analyzing data. Nevertheless this is a great tool.

Creating a Pivot Table

Set the active cell in the source data. This is select any cell on the data out of which you want to create a Pivot Table. Then, on the Insert tab of the Tables group select the command Pivot Table. If you click on the upper part of the Pivot Table icon, then immediately the dialog box Create a Pivot Table will be displayed. If you click on the arrow under the icon, you will have to choose from the available commands the one about creating a Pivot Table.

![image63](../Images/image63.jpg)

In the Create Pivot Table dialog box, in which Excel automatically detected and entered the range of the source data in the field Select a table or range. To place the Pivot Table in the new worksheet, leave the default selection in the part of the dialog box referring to the position of the Pivot Table report.

![image100](../Images/image100.png)

After confirmation the Pivot Table is ready to work. The new worksheet with an empty Pivot Table has been inserted. On the right side there appeared the Pivot Table Field List, below which there are areas of the Pivot Table. Additionally, on the ribbon there appeared a group of contextual tabs Pivot Table Tools, which include cards Options and Design.

![image58](../Images/image58.jpg)

Pivot Table Areas

### Report filter

In this area we place fields from the PivotTable Field List, which are used to filter data. The values of the fields located in the filter will not be visible in the PivotTable.

### Row labels

Labels placed in rows, like row headers in an ordinary table.

### Column labels

The labels placed in columns, like column headers in an ordinary table.

### Values

The values of the fields located in this area will be summed up. Besides summing up, we can perform other activities on them, but you will learn more about them later on. To sum up the values of the fields located in the area of value, it is necessary that these values are recognized by Excel as numbers.

Placing fields in PivotTable areas

We can place the fields in the PivotTable areas in several ways. One of them is to select the chosen fields in the PivotTable Field List, the fields will be placed in areas selected by Excel. Pay attention to the field of Years, which shows the number representing the year in date. This field has been placed in the area of values, and the values in column Years have been summed up!

![image43](../Images/image43.jpg)

After selecting the fields we can change their position and the way of summing up the field, but a faster way is to place the fields in the appropriate areas right away. A more convenient and a faster way is to drag fields from the PivotTable Field List to the selected areas. Click any mouse button (it does not matter whether left or right) on the selected area and drag it to the selected area. Let’s recall the set purpose: What is the value of sales grouped by individual regions and years? We are interested in the fields Sales , Region  and Years . The order of placing them in the table can be varied. To achieve the goal that was set earlier we need to do the following: 1. Drag the Sales  field to the Values area

![image47](../Images/image47.jpg)

2\. Drag the field Region to the area Rows

![image11](../Images/image11.jpg)

3\. Drag the field Years to the area Columns

![image39](../Images/image39.jpg)

Finished! Pivot Table has been prepared. The goal has been achieved. We value sales broken down by regions and years, however, these data are difficult to read.

### Modifying Pivot Table

We created a PivotTable in Excel that displays a summary of the values in column with the sales data broken down by region (placed in rows) and years (placed in columns). The new goal to achieve Early formatting of the data source from which you create a PivotTable does not affect the format of the data in the pivot table. The data in the PivotTable is displayed in the general format. How do you change the format of the data for each field to have useful information is displayed in a clear manner? How do you change the format of the data for each field? Display format can be changed in several ways. In this section we will describe the most commonly used ones.

Calling the Settings dialog box values.

1\. Left-click on the box located in the area of values and select Settings in the value field. 2. Set the active cell in the pivot table in the data for this field. We can also set up a cell in the row or column totals, and in the cell, which displays the name of the function used for the field (in our case this cell is the cell with the entry Sum of Sales.) It is important that on the Options tab in the group Active box was displayed name fields, which change the format of the displayed data is affected. When you select a cell on the Options tab in the group Active box, click on the Value Field Settings.

![image98](../Images/image98.jpg)

Change the format of data displayed.

When you click on the Settings value field will show the Settings dialog box values.

![image109](../Images/image109.png)

We can change the way data summary (e.g. The sum of these values on the counter) but we will not do it this example. Click on the button Number Format. A window appears Format Cells, which will be visible only card numbers. We can now format the data for the selected field according to their own needs. In this case, I am changing the category on the numerical decimal places I set to 0 and turn on the grouping of numbers after 3 digits by checking the Use 1000 Separator (,).

![image102](../Images/image102.png)

Finished! Once approved, the data is formatted pivot table is as follows.

![image106](../Images/image106.jpg)

### Summary

In the lesson it has been presented how to use pivot tables to let you quickly, easily and clearly summarize and analyze large data sets. Modification of displayed results also does not cause problems. Of course, this does not cover the whole subject pivot tables in Excel. We encourage you to exercise your own research as well. In the attached files PivotTable-Data.xls – data for lesson TEST: WSI-INTERNET-TEST-EXCEL-PIVOT-TABLES.pdf SXXXXX-WSI-INTERNET-TEST-EXCEL-PIVOT-TABLES.xlsx Scoring max 6 Point for each task
