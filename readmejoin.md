### seleziona tutti gli studenti iscritti al corso di laurea in economia

- SELECT `students`.`name` AS `student_name`, `students`.`surname` AS `student_surname`, `students`.`registration_number` AS `student_registration_number`, `degrees`.`name` AS `degree_name` FROM `students` JOIN `degrees` ON `students`.`degree_id` = `degrees`.`id` WHERE `degrees`.`name` = 'Corso di Laurea in Economia';

### seleziona tutti i corsi di laurea magistrale nel dipartimento di neuroscienze

- SELECT `degrees`.`level` AS `degree_level`, `departments`.`name` AS `department_level` FROM `degrees` JOIN `departments` ON `degrees`.`department_id` = `departments`.`id` WHERE `departments`.`name` = 'Dipartimento di Neuroscienze' AND `degrees`.`level` =    'magistrale';

### seleziona tutti i corsi di laurea tenuti dal prof fulvio amato

- SELECT `courses`.`name` AS `course_name`, `teachers`.`name` AS `teacher_name`, `teachers`.`surname` AS `teacher_surname`, `teachers`.`id` AS `teacher-id` FROM `course_teacher` JOIN `courses` ON `course_teacher`.`course_id` = `courses`.`id` JOIN `teachers` ON `course_teacher`.`teacher_id` = `teachers`.`id` WHERE `teachers`.`id` = 44;