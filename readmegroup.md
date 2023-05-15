### contare quanti iscritti ci sono stati ogni anno

-SELECT YEAR(`students`.`enrolment_date`) AS `enrollment_year`, COUNT(*) FROM `students` GROUP BY YEAR(`students`.`enrolment_date`);

### conta gli inseganti che lavorano nello stesso edificio

-SELECT `teachers`.`office_address` AS `office_address`, COUNT(*) FROM `teachers` GROUP BY `teachers`.`office_address`;

### fare la media dei voti di ogni appello d'esame

- SELECT `exam_student`.`exam_id` AS `exam`, AVG(`exam_student`.`vote`) AS `vote_average` FROM `exam_student` GROUP BY `exam` ASC ORDER BY AVG(`exam_student`.`vote`);

### contare quanti corsi di laurea ci sono per ogni dipartimento

- SELECT `departments`.`name` AS `department_name`, COUNT(`degrees`.`id`) AS `degrees` FROM `degrees` JOIN `departments` ON `degrees`.`department_id` = `departments`.`id` GROUP BY `department_name`;

