//Query 1
SELECT students.name, students.surname 
FROM students 
INNER JOIN degrees 
ON students.degree_id = degrees.id 
WHERE degrees.name = 'Corso di Laurea in Economia'; 

//Query 2
SELECT degrees.name, degrees.level, departments.name
FROM degrees 
JOIN departments
ON degrees.department_id = departments.id
WHERE degrees.level = 'magistrale' AND departments.name = 'Dipartimento di Neuroscienze';

//Query 3
//Query 4
//Query 5
//Query 6
//Query 7