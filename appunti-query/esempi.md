
1. Selezionare il voto più basso dato ad ogni appello d'esame 
    ```
    SELECT MIN(`vote`) as `lowest_vote`, `exam_id` FROM `exam_student` GROUP BY `exam_id`;
    ```

2. Contare gli appelli d'esame del mese di luglio raggruppati per giorno
    ```
    SELECT COUNT(*) as `exams_number`, DAY(`date`) as `day` FROM `exams` WHERE MONTH(`date`) = 7 GROUP BY `day`;
    ```

3. Selezionare tutti i corsi di laurea del corso di laurea di informatica
    ```
    SELECT `courses`.`id` , `courses`.`name` as nome_corso , `degrees`.`name` as nome_corso_di_laurea ,  `courses`.`description` ,  `courses`.`period` , `courses`.`year`
    FROM `courses`
    JOIN `degrees` ON `courses`.`degree_id` = `degrees`.`id`
    WHERE `degrees` . `name` = 'Corso di Laurea in Informatica';
    ```

4. Selezionare le informazioni del corso con id=144, con tutti relativi appelli d'esame 
    ```
    SELECT `courses`.* , `exams`.`id` , `exams`.`date` , `exams`.`hour`
    FROM `courses`
    JOIN `exams` ON `courses`.`id` = `exams` . `course_id`
    WHERE `courses`.`id` = 144;
    ```
    
5. Selezionare a quale dipartimento appartiene il Corso di Laurea in Diritto dell'Economia 
    ```
    SELECT `departments`.*
    FROM `departments`
    JOIN `degrees` ON `departments`.`id`= `degrees`.`department_id`
    WHERE `degrees`.`name` = 'Corso di Laurea in Diritto dell\'Economia' ;
    ```







