# Data Normalization and Entity-Relationship Diagramming

## Courses
|course_id   |course_name                       |
-------------------------------------------------
|1           |Data normalization                |
|2           |Single table queries              |
|3           |Python and pandas                 |
|4           |Spreadsheet aggregate functions   |

## Professors
professor_id    professor_name      professor_email
1               Melvin              l.melvin@foo.edu
2               Logston             e.logston@foo.edu
3               Nevarez             i.nevarez@foo.edu

## Classrooms
classroom_id    classroom_name  
1               WWH 101   
2               60FA 314
3               WWH 201

## Sections
section_id  course_id   professor_id    classroom_id    
1           1           1               1
2           2           2               2
3           3           2               2   
4           4           3               3

## Assignments
assignment_id   section_id  assignment_topic    due_date    relevant_reading   1               1           Data normalization  23.02.21    Deumlich Chapter 3
2               2           Single table queries18.11.21    Dümmlers Chapter 11 3               3           Python and pandas   05.05.21    Dümmlers Chapter 14
4               4           Spreadsheet agg fn  04.07.21    Zehnder Page 87

## Students assignments

student_id  assignment_id   grade   
1           1               80
7           2               25
4           1               75
2           3               92
2           4               65


I seperated courses, professors, classrooms, sections, assignments, and students assignments into different tables giving each a primary key.I worked on eliminating any dependencies found in the intitial table, thus allowing this to be 4NF, such as through creating a seperated professors table, creating different tables for sections and assignments, thus we can ensure that each non-prime attribute only depends on the candidate keys of the table.