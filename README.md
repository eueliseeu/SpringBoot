
## Spring Boot

Este projeto é uma aplicação Spring Boot para gerenciar uma lista de funcionários com funcionalidades básicas de CRUD e paginação. A aplicação fornece uma API RESTful que pode ser utilizada para realizar operações..

### Estrutura do Projeto

O projeto é estruturado da seguinte forma:
https://mega.nz/file/dWhEwZSR#l2zo_mvr1mRBsJ7pIQ1GGiJck21UApaZxKQGs8mV4hk
```
src/
├── main/
│   ├── java/
│   │   └── com/
│   │       └── eueliseeu/
│   │               ├── controllers/
│   │               │   └── EmployeeController.java
│   │               ├── models/
│   │               │   └── Employee.java
│   │               ├── repositories/
│   │               │   └── EmployeeRepository.java
│   │               └── services/
│   │                   └── EmployeeService.java
│   └── resources/
│       ├── application.properties
│       └── static/
└── test/
    └── java/
        └── com/
            └── exemplo/
                └── funcionarios/
                    └── EmployeeControllerTests.java
```

### Configuração

1. **Pré-requisitos**
   - Java 17 ou superior.
   - Maven 3.6 ou superior (ou Gradle, dependendo da sua configuração).
   - Banco de Dados (H2, PostgreSQL, etc.) configurado no `application.properties`.

2. **Configuração do Banco de Dados**
   - Configure o banco de dados no arquivo `application.properties`.
   - Exemplo para PostgreSQL:
     ```properties
     spring.datasource.url=jdbc:postgresql://localhost:5432/seubanco
     spring.datasource.username=seuusuario
     spring.datasource.password=suasenha
     ```

3. **Executando a Aplicação**
   - Compile e execute a aplicação usando Maven ou Gradle:
     ```bash
     ./mvnw spring-boot:run
     ```
     ou
     ```bash
     ./gradlew bootRun
     ```

   - A aplicação será iniciada em `http://localhost:8080`.

### Testes

Os testes unitários e de integração estão localizados em `src/test/java/com/exemplo/funcionarios/EmployeeControllerTests.java`.

Para executar os testes:
```bash
./mvnw test
```
ou
```bash
./gradlew test
```

### Licença

Este projeto está licenciado sob a [MIT License](LICENSE).
