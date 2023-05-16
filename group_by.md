//query 1
SELECT AVG(vote) as vote_avg, exam_id
FROM exam_student
GROUP BU exam_id 

//query 2
SELECT COUNT (*) as courses_number, department_id
FROM degrees
GROUP BY department_id
