1. Clonar el repositorio
2. Abrir el proyecto en el IDE de preferencia. Normalmente los IDES para proyectos Spring Boot son Netbeans, Eclipse y Spring Boot tools
3. Crear base de datos llamada "db_note_generation":
  CREATE database db_note_generation;
4. Correr el proyecto de Springboot
5. Correr los comandos:
  USE db_note_generation;
  INSERT INTO lab_cases (name, create_at) VALUES('lab cas 1', NOW());
  INSERT INTO lab_cases (name, create_at) VALUES('lab cas 2', NOW());
  INSERT INTO lab_cases (name, create_at) VALUES('lab cas 3', NOW());
  INSERT INTO lab_cases (name, create_at) VALUES('lab cas 4', NOW());
 6. Ya la api del generador de notas debería estar corriendo
