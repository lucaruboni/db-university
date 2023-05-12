### studenti nati nel 1990

- SELECT * FROM `students` WHERE YEAR(`date_of_birth`) = 1990;


### corsi che hanno + di 10 cfu

- SELECT * FROM `courses` WHERE cfu > 10;

### studenti che hanno + di 30 anni

-SELECT * FROM `students` WHERE YEAR(CURRENT_TIMESTAMP()) - YEAR(`date_of_birth`) > 30;

### corsi del primo semestre del primo anno

- SELECT * FROM `courses` WHERE `period` = 'I semestre' AND `year` = 1;

### appelli d'esame pomeridiani del 20/06/2020

- SELECT * FROM `exams` WHERE HOUR(`hour`) >= 14 AND `date` = '2020/06/20';

### tutti i corsi di laurea magistrale

- SELECT * FROM `degrees` WHERE `level` = 'magistrale';

### quanti dipartimenti ha l'università?

- SELECT * FROM `departments`

### quanti sono gli insegnanti che non hanno un numero di telefono?

- SELECT * FROM `teachers` WHERE `phone` IS NULL;