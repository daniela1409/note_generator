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
 
 
 Para las consultas desde Postman al backend, se usa lo siguiente:

1. Encontrar todos los lab cases
  Method=GET
  URL: http://localhost:8080/lab-case/

2. Guardar lab cases
  Method=POST
  URL: http://localhost:8080/lab-case
  Body/Json:
  {
    "name": "case 1"
  }
 
3. Editar lab cases
    Method=PUT
    URL: http://localhost:8080/lab-case/1
    Body/Json:
    {
      "name": "case 1"
    }
 
4. Encontrar notes por lab case
   method=GET
   url=http://localhost:8080/note/1
   
5. Guardar note
   method=POST
   url=http://localhost:8080/note/
    Body/Json:
  {
      "note" : "segunda nota",
      "lab_case_id" : 1
  }
 
5. Editar note
   method=POST
   url=http://localhost:8080/note/
    Body/Json:
    {
        "note" : "segunda nota",
        "lab_case_id" : 1
    }

  
