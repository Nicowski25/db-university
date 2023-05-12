//query 1
SELECT date_of_birth FROM students where date_of_birth BETWEEN '1990-1-1' AND '1990-12-31';

//query 2
SELECT cfu FROM courses WHERE cfu > 10;

//query 3
SELECT date_of_birth 
FROM students 
WHERE date_of_birth < '1993-05-12'; 

//query 4
SELECT period, year 
FROM `courses` 
WHERE period = 'I semestre' AND year = '1'; 

//query 5
SELECT hour, date 
FROM exams 
WHERE hour > '14:00:00' AND date = '2020-06-20'; 

//query 6
SELECT level 
FROM degrees 
WHERE level = 'magistrale'; 
