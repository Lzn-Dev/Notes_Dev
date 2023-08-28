
### Comment connecter Spring à ma base de donnée ? (MYSQL)

1. A copié dans le fichier *application.properties*
```	
MYSQL_HOST=localhost:8889  
MYSQL_DATABASE=laboitealivre  
# -----  
spring.datasource.url=jdbc:mysql://${MYSQL_HOST}/${MYSQL_DATABASE}  
spring.datasource.username=root  
spring.datasource.password=root  
spring.datasource.driver-class-name=com.mysql.cj.jdbc.Driver  
# -------
```
  2. Dans les dependencies du fichier *build.gradle*
```
runtimeOnly 'mysql:mysql-connector-java:8.0.29'  
implementation 'org.springframework.boot:spring-boot-starter-data-jpa'
```
