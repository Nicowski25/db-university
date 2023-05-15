//Query 1
SELECT students.name, students.surname 
FROM students 
INNER JOIN degrees 
ON students.degree_id = degrees.id 
WHERE degrees.name = 'Corso di Laurea in Economia'; 