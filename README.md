# Configuração do Banco de Dados

No arquivo `application.properties`, configure os seguintes parâmetros para conectar ao banco de dados PostgreSQL:

```properties
# Informações da aplicação
spring.application.name=agendar

# Configuração do banco de dados
spring.datasource.url=jdbc:postgresql://localhost:5432/agenda
spring.datasource.username=postgres
spring.datasource.password=postgres

# Configurações do JPA
spring.jpa.hibernate.ddl-auto=update
spring.jpa.show-sql=true
```

### Modelo para salvar um usuário e um evento

#### Usuário

    {
        "cpf": "",
        "nome": "",
        "email": "",
        "dataNascimento": ""
    }

#### Evento

    {
        "nome": "",
        "descricao": "",
        "organizacao": "",
        "dataInicio": "",
        "dataFim": ""
    }
