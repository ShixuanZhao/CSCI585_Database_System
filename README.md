# CSCI585_Database_System
1.Student
Each student has a unique ID.With the id, we can find the books(or no book) that the student borrowed from library. And we can track his registration record. He can choose many courses. Also, during his study, he can book study room. Many students are allowed to book one room. Students corresponding to many rate id. 

2.Registration_Record
The table is relational table between students and classes.Actually, it represents a student can take many courses, and a course can be chosed by multiple students. Also, it can record the other attribute, like semester ot register time. 

3.Classes
It is super class for Coding_Class and Project.The symbol is "d"(I do not find this symbol in draw.io).It has only two subclass. And they are not overlapping.

4.Reference_Book
With FK library id and student id, we cna know this book belong to which library and it was borrowed by whom. The duration is a constant.

5.Room_Schedule
I suppose student must book a room for study or project representation. And in a schedule, it maybe involve many rooms.
  
6.Rate
A student can have many rate report because he can take many courses. For each report. it includes Instructor_ID, Instructor_Score and Class_ID, Class_Score.
  
7.Group
A group can contain many student. For a student he has group id as FK to track which group he belongs to.
And each group take charge of one project.

8.Coding_Class
It is a subclass for Class

9.Project
It is a subclass for Class. A project has multiple parts(materials).

10.Instructor
An Intestructor can assign many textbooks. Also a textbook can also assigned by diffenent instructor.

11.TextBook
A Textbook can be used by many coding class. Only for coding class not for project. I suppose for project, students do not need textbooks.

12.Parts
It is the super class for Micro-controller and Hardware. And the two subclass are disjoint and it is complete.

13.Micro-controller
It is a subclass for Parts

14.Hardware
It is a subclass for Parts

15.Programming_Language
A programming language can be taught in many classes. And some diffcult language can not be taught in class.

16.Order_Record
For a part, it can cause many order record because it can be purchased from different suppliers or different quantity.

17.Supplier
For a supplier, he can sale many product which can cause many transction record.

18.Library
Given a library id, I can track all the books in it.

19.Room
The room can be booked at different time, so it can cause many schedules.
