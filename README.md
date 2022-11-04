# ParcialCVDS

### Wilmer Arley Rodriguez
Antes de comenzar con el parcial, vamos a clonar el repositorio remoto para poderlo trabajar localmente y asi poder realizar los cambios que queramos.

![image](https://user-images.githubusercontent.com/77862048/199873385-b01a404a-6e4c-47f2-8edb-e595dbcf4937.png)

![image](https://user-images.githubusercontent.com/77862048/199873438-267a1aaa-cad1-45aa-81f4-7631400e6942.png)

Como se puede ver ya tenemos el proyecto clonado y listo para poder trabajar.
### Primer Punto.
1. A partir de la especificación hecha en los métodos consultarPacientesPorId y consultarMenoresConEnfermedadContagiosa de la fachada de servicios (la parte lógica de la aplicación), implemente sólo una prueba (la que considere más importante para validar las especificaciones y los criterios de aceptación). Siga el esquema usado en ServicesJUnitTest para poblar la base de datos volátil y verificar el comportamiento de las operaciones de la lógica.

- Observamos primero lo que deberia hacer cada método.

![image](https://user-images.githubusercontent.com/77862048/199833918-b5d8bc2f-8d08-4919-868c-3eb21d3807a6.png)

- Basados en lo que nos dice la documentación de los métodos construimos las pruebas sin aun tener en cuenta la lógica.

![image](https://user-images.githubusercontent.com/77862048/199834097-b4fb4faf-ee53-4b8a-8d74-235f2819a9a2.png)

![image](https://user-images.githubusercontent.com/77862048/199840137-0a74a9b6-bf33-4a4f-8a6f-cc1991a1402f.png)

- Como aun no hemos hecho la lógica las pruebas fallaran:

![image](https://user-images.githubusercontent.com/77862048/199840260-0bfdca9b-94c7-4cf8-ab01-be0bad451876.png)

- Implementamos la logica correspondiente:

![image](https://user-images.githubusercontent.com/77862048/199872970-9970d84e-b174-4703-919b-f3983b1a14a4.png)
![image](https://user-images.githubusercontent.com/77862048/199873131-e0e4107e-7367-4378-a876-b45e99272957.png)
![image](https://user-images.githubusercontent.com/77862048/199873212-39e18a98-5421-4985-8019-b383614faf39.png)


- Y en el PacienteMapper.xml ponemos las siguientes consultas:

![image](https://user-images.githubusercontent.com/77862048/199855135-59c428af-2c0b-4d03-bbd6-d29504efc7f1.png)

![image](https://user-images.githubusercontent.com/77862048/199855164-86a909f1-83b0-4f89-98f3-3aed2eb09918.png)

- Ejecutamos de nuevo las pruebas y vemos que ahora si pasan.

![image](https://user-images.githubusercontent.com/77862048/199855239-67ff915a-e7dd-4307-9255-7edb91c62795.png)

2. Implemente la historia de usuario #1, agregando todo lo que haga falta en la capa de presentación, lógica y de persistencia. La vista debe implementarse en consultaPaciente.xhtml.

- La mayor parte de la logica ya se hizo en el punto anterior con los test, sin embargo se agrego algo mas en los beans que fue los siguiente:

![image](https://user-images.githubusercontent.com/77862048/199870458-3d83f778-0ce2-4be6-891c-c69f52cb49b9.png)

- El archivo xhtml quedo de la siguiente forma:

![image](https://user-images.githubusercontent.com/77862048/199870798-11fca27c-111f-4127-a576-0a29cc8c1ded.png)


- Iniciamos el servicio de tomcat y consultamos:

![image](https://user-images.githubusercontent.com/77862048/199870535-84fcfda1-c5a5-42ef-a467-f48c01e1baa9.png)

3. Implemente la historia de usuario #2, agregando todo lo que haga falta en la capa de presentación, lógica y de persistencia. La vista debe implementarse en consultarMenoresEnfermedadContagiosa.xhtml.

- Al igual que en el anterior punto no cambiaremos mucho de la lógica ya que fue realizado en el primer punto, solo haremos los siguientes cambios en el Bean:

![image](https://user-images.githubusercontent.com/77862048/199872629-f19eda38-bb50-49be-b579-81d5265db5ea.png)

- El archivo xhtml quedaria de la siguiente forma:

![image](https://user-images.githubusercontent.com/77862048/199872653-990fe79d-8ed0-4e6a-9af2-aa991bfbccf8.png)

- Iniciamos el servicio de tomcat y realizamos la consulta para verificar que todo este bien implementado:

![image](https://user-images.githubusercontent.com/77862048/199872689-2be618cd-92e0-48a9-9721-08b5f1bdb1dd.png)

- Por ultimo compilaremos todo el proyecto para verificar que todo este en correcto funcionamiento y haremos push al repositorio remoto

![image](https://user-images.githubusercontent.com/77862048/199873599-f3aa060c-88cb-4866-84bf-c4dd7c4c0a78.png)

![image](https://user-images.githubusercontent.com/77862048/199873626-df52d279-ce37-490e-8a4c-274e9b344396.png)

![image](https://user-images.githubusercontent.com/77862048/199874093-9d6748ff-b42f-405b-aa2c-f2c48dba37ae.png)


