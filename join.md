//Query 1
SELECT students.name, students.surname 
FROM students 
INNER JOIN degrees ON students.degree_id = degrees.id 
WHERE degrees.name = 'Corso di Laurea in Economia'; 

//Query 2
SELECT degrees.name, degrees.level, departments.name
FROM degrees 
JOIN departments ON degrees.department_id = departments.id
WHERE degrees.level = 'magistrale' AND departments.name = 'Dipartimento di Neuroscienze';

//Query 3
SELECT courses.name , teachers.name, teachers.surname, teachers.id
FROM course_teacher
JOIN teachers ON teachers.id = course_teacher.teacher_id 
JOIN courses ON course_teacher.course_id = courses.id
WHERE teachers.name = 'Fulvio'
AND teachers.surname = 'Amato'
AND teachers.id = 44;

//Query 4
//Query 5
//Query 6
//Query 7