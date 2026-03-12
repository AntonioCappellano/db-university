## 1. Selezionare tutti gli studenti iscritti al Corso di Laurea in Economia (68)
- SELECT 
    students.id student, 
    degrees.name degrees_name
- FROM 
    university_db.students
- JOIN 
    university_db.degrees ON degree_id = degrees.id
- WHERE 
    degrees.name = 'Corso di Laurea in Economia';

## 2. Selezionare tutti i Corsi di Laurea Magistrale del Dipartimento di Neuroscienze (1)
- SELECT 
    degrees.name
- FROM 
    university_db.degrees
- INNER JOIN 
    university_db.departments ON degrees.department_id = departments.id
- WHERE 
    departments.name = 'Dipartimento di Neuroscienze'
    AND degrees.level = 'magistrale'; 

## 3. Selezionare tutti i corsi in cui insegna Fulvio Amato (id=44) (11)
- SELECT courses.name
- FROM university_db.courses
- INNER JOIN university_db.course_teacher ON courses.id = course_teacher.course_id

- WHERE course_teacher.teacher_id = 44


## 4. Selezionare tutti gli studenti con i dati relativi al corso di laurea a cui sono iscritti e il relativo dipartimento, in ordine alfabetico per cognome e nome (5000)


## 5. Selezionare tutti i corsi di laurea con i relativi corsi e insegnanti (1317)

## 6. Selezionare tutti i docenti che insegnano nel Dipartimento di Matematica (54)

## 7. BONUS: Selezionare per ogni studente il numero di tentativi sostenuti per ogni esame, stampando anche il voto massimo. Successivamente,filtrare i tentativi con voto minimo 18

