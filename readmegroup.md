### contare quanti iscritti ci sono stati ogni anno

-SELECT YEAR(`students`.`enrolment_date`), COUNT(*) FROM `students` GROUP BY YEAR(`students`.`enrolment_date`);

### 