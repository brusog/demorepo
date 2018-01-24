These terms are explained in the EDX course on **SQL Databases**. [Here](https://courses.edx.org/courses/course-v1:Microsoft+DAT215.1x+1T2018/course/) is the link to the Course.

#Some Terms
##What is an UnNormalized Data?
Imagine an excel sheet containing details about a school.
It has a lot of information related to the different classes, students, subjects and other things.
This kind of data can be an example of **UnNormalized data**


##What is Normalization?
Normalization is a process in Database design where we look at the data and segregate the data into individual tables and relate the tables. Tables are  called as *Entities* in DB terminology.
When we normalize a data, we end up with an *Entity-Relationship* diagram and create individual Tables which are related with each other.

##What is De-Normalization?
*Normalization is **NOT** the opposite of Normalization*
De-Normalization is a process where we change the table structure to make it more easy and efficient to Query. 
Imagine a DB table which captures the Sales data for a company. On a daily basis whenever goods are sold there will be entries made to the Sales table. There can be continous updates to the Sales data. So, the design of this Sales table will be Normalized design.
Now, imagine a table representing Old or Archived Sales data. We would not expect this table to experience updates. However, we would like to use this Sales data to be queried much more frequently and updated very very rarely. So the design of this table will be De-Normalized design.

>De-normalized database schemas are suitable for frequent Queries
>Normalized database schemas are suitable for frequent inserts and updates
