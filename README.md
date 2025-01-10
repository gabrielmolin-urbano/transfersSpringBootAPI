# Transfers API

Este é um projeto Java baseado no framework **Spring Boot 3.4.1**, utilizando Java 23. O objetivo desta API é fornecer funcionalidades para gerenciamento de transferências, utilizando uma arquitetura moderna e robusta.

## Tecnologias e Dependências

Este projeto utiliza as seguintes bibliotecas e tecnologias:

### **Spring Boot Starter Web**
- Utilizado para criar APIs RESTful de forma rápida e eficiente.
- Fornece suporte a configurações simplificadas e uma poderosa integração com o ecossistema Spring.

### **Spring Boot Starter Data JPA**
- Biblioteca para acesso e manipulação de dados.
- Utiliza **JPA (Java Persistence API)**, que abstrai o banco de dados relacional e simplifica as operações de CRUD.
- Permite o uso de **Hibernate**, uma poderosa implementação de JPA, para gerenciar o mapeamento objeto-relacional (ORM).
- Facilita a criação de consultas complexas com o uso de **JPQL** ou **Criteria API**.

**Por que JPA?**
- Reduz a quantidade de código boilerplate necessário para manipulação de dados.
- Permite o uso de anotações para configurar facilmente o relacionamento entre entidades.
- Oferece suporte a transações e caching integrado.

### **H2 Database**
- Um banco de dados em memória utilizado para desenvolvimento e testes.
- Não requer instalação ou configuração adicional.
- Permite executar rapidamente testes unitários ou de integração com os dados persistidos diretamente na memória.
- A console web do H2 facilita a visualização e manipulação dos dados durante o desenvolvimento. (Acesse: `http://localhost:8080/h2-console`).

### **Lombok**
- Simplifica o código ao gerar automaticamente métodos como `getters`, `setters`, `toString`, `equals` e `hashCode`.
- Reduz significativamente a verbosidade do código, permitindo focar na lógica de negócios.

### **ModelMapper**
- Biblioteca para mapeamento automático entre objetos Java.
- Ideal para conversões rápidas entre DTOs (Data Transfer Objects) e entidades JPA.
- Facilita a separação de responsabilidades e promove um código mais limpo e organizado.

### **Spring Boot DevTools**
- Ferramenta para acelerar o desenvolvimento.
- Inclui suporte a reinicialização automática do servidor ao salvar alterações no código.
- Melhora a experiência do desenvolvedor.

### **Spring Boot Starter Test**
- Fornece bibliotecas essenciais para testes, incluindo JUnit, Mockito e AssertJ.
- Permite a escrita de testes unitários e de integração robustos.

## Requisitos

- **Java 23** ou superior.
- **Maven** para gerenciar as dependências.

## Configuração

1. Clone o repositório:
   ```bash
   git clone https://github.com/seu-usuario/transfersApi.git
   ```

2. Acesse o diretório do projeto:
   ```bash
   cd transfersApi
   ```

3. Execute o projeto:
   ```bash
   mvn spring-boot:run
   ```

Segue o código formatado no padrão para copiar e colar no seu README:

## Acessando o Banco de Dados H2

1. Inicie o projeto.  
2. Acesse o console web do H2 em: [http://localhost:8080/h2-console](http://localhost:8080/h2-console)  
3. Use as seguintes credenciais:  
   - **JDBC URL:** `jdbc:h2:mem:testdb`  
   - **Usuário:** `sa`  
   - **Senha:** *(deixe em branco)*  

## Estrutura do Projeto

- **`src/main/java`**: Contém o código fonte da aplicação.  
- **`src/main/resources`**: Contém configurações como `application.properties`.  
- **`src/test`**: Contém testes unitários e de integração.  

---

Este projeto foi criado com foco na simplicidade, escalabilidade e manutenção. Fique à vontade para contribuir!  