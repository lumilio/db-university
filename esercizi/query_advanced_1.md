
---- Query GROUP BY ----

1. Contare quanti iscritti ci sono stati ogni anno 
    ```
    SELECT COUNT(*) as `numero_iscritti`, YEAR(`enrolment_date`) as `anno` FROM `students` GROUP BY `anno`;
    ```

2. Contare gli insegnanti che hanno l'ufficio nello stesso edificio
    ```
    SELECT COUNT(*) as `numero_insegnanti`, `office_address` as `edificio` FROM `teachers` GROUP BY `ufficio`;
    ```

3. Calcolare la media dei voti di ogni appello d'esame 
    ```
    SELECT AVG(`vote`) as `media_studenti` , `exam_id` FROM `exam_student` GROUP BY `exam_id`;
    ```

4. Contare quanti corsi di laurea ci sono per ogni dipartimento
    ```
    SELECT COUNT(*) as `numero_corsi_laurea`, `department_id` FROM `degrees` GROUP BY `department_id`;
    ```


---- Query JOIN ----

1. Selezionare tutti gli studenti nati nel 1990 (160) 
    ```
    ```

2. Selezionare tutti i corsi che valgono più di 10 crediti (479)
    ```
    ```

3. Selezionare tutti gli studenti che hanno più di 30 anni 
    ```
    ```

4. Selezionare tutti i corsi del primo semestre del primo anno di un qualsiasi corso di laurea (286)
    ```
    ```

5. Selezionare tutti gli appelli d'esame che avvengono nel pomeriggio (dopo le 14) del 20/06/2020 (21)
    ```
    ```

6. Selezionare tutti i corsi di laurea magistrale (38) 
    ```
    ```

7. Da quanti dipartimenti è composta l'università? (12)
    ```
    ```

8. Quanti sono gli insegnanti che non hanno un numero di telefono? (50)
    ```
    ```

