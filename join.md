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
SELECT students.name, students.surname, degrees.*, departments.name
FROM students
JOIN degrees ON degrees.id = students.degree_id
JOIN courses ON courses.degree_id = courses.id
JOIN departments ON departments.id = degrees.department_id
ORDER BY students.surname, students.name

//Query 5
SELECT degrees.name, courses.name, teachers.name, teachers.surname
FROM courses 
JOIN degrees ON degrees.id = courses.degree_id
JOIN course_teacher ON course_teacher.course_id = courses.id
JOIN teachers ON teachers.id = course_teacher.teacher_id
ORDER BY degrees.names

//Query 6
SELECT teachers.name, teachers.surname, courses.name, departments.name
FROM course_teacher
JOIN teachers ON teachers.id = course_teacher.teacher_id
JOIN courses ON courses.id = course_teacher.course_id
JOIN degrees ON degrees.id = courses.degree_id
JOIN departments ON departments.id = degrees.department_id
WHERE departments.name = 'Dipartimento di Matematica'

//Query 7
