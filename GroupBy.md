## 1. Contare quanti iscritti ci sono stati ogni anno

- SELECT 
-   COUNT(*) number_subs,
-   YEAR(enrolment_date) year_enrolment
- FROM university_db.students
- GROUP BY YEAR(enrolment_date)

## 2. Contare gli insegnanti che hanno l'ufficio nello stesso edificio

- SELECT COUNT(*) teachers_number,
- office_address
- FROM university_db.teachers
- GROUP BY office_address;

## 3. Calcolare la media dei voti di ogni appello d'esame

## 4. Contare quanti corsi di laurea ci sono per ogni dipartimento
