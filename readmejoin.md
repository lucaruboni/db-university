### seleziona tutti gli studenti iscritti al corso di laurea in economia

- SELECT `students`.`name` AS `student_name`, `students`.`surname` AS `student_surname`, `students`.`registration_number` AS `student_registration_number`, `degrees`.`name` AS `degree_name` FROM `students` JOIN `degrees` ON `students`.`degree_id` = `degrees`.`id` WHERE `degrees`.`name` = 'Corso di Laurea in Economia';

### seleziona