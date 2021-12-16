- capire le differenze delle tipologie di esercizio , Join , Group by



1. Selezionare il voto più basso dato ad ogni appello d'esame 
    ```
    SELECT MIN(`vote`) as `lowest_vote`, `exam_id` FROM `exam_student` GROUP BY `exam_id`;
    ```

2. Contare gli appelli d'esame del mese di luglio raggruppati per giorno
    ```
    SELECT COUNT(*) as `exams_number`, DAY(`date`) as `day` FROM `exams` WHERE MONTH(`date`) = 7 GROUP BY `day`;
    ```



3. Contare 
    ```
    SELECT 
    





