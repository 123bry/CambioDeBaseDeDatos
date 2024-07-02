# Cambiar de base de datos de h2 a una relacional

Para iniciar con este cambio primero modificamos en application properties
- spring.datasource.url: Este define la URL de conexión a tu base de datos MySQL.
- spring.datasource.username y spring.datasource.password: Son las credenciales para acceder a MySQL. 
     Usuario: Bryan
     Contraseña: 0951@Bry 
- spring.datasource.driver-class-name: Nos ayuda a especificar la clase del driver de MySQL.
- spring.jpa.database-platform: Configura el dialecto de MySQL para Hibernate.
- spring.jpa.show-sql=true: Habilita la impresión de las consultas SQL generadas por Hibernate en la consola.

![image](https://github.com/123bry/CambioDeBaseDeDatos/assets/99741524/420bd31e-40f8-4d10-96cf-7255a9d1291a)


------------------------------ 
En la sección pom.xml. Se agrego la <dependency> para mysql-connector-java, para que Spring Boot pueda usar el conector MySQL.

![image](https://github.com/123bry/CambioDeBaseDeDatos/assets/99741524/8193b70c-7eb8-47bc-b091-38afe73e6c37)
![image](https://github.com/123bry/CambioDeBaseDeDatos/assets/99741524/7c3af36f-844f-4009-8f12-d0fdeb1b59ad)
![image](https://github.com/123bry/CambioDeBaseDeDatos/assets/99741524/08af0163-1a4b-444a-a432-a957c51c9bc6)


-------------------------------
Prueba en la base de datos

![image](https://github.com/123bry/CambioDeBaseDeDatos/assets/99741524/759cacbc-af44-4e90-9a4d-d276e763d14c)


-------------------------------
Prueba en Postman
- http://localhost:8896/hotels 

![image](https://github.com/123bry/CambioDeBaseDeDatos/assets/99741524/68b94b82-3ea3-4add-aac6-7281794f9902)


