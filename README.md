# Sistema de Controle de Ponto e Acesso

## Descrição

O **Sistema de Controle de Ponto e Acesso** é uma aplicação backend desenvolvida em Java com Spring Boot, projetada para registrar entradas e saídas de funcionários, gerando relatórios de ponto. O projeto utiliza Spring Data JPA para persistência em banco H2, aplicando padrões de projeto como Repository e boas práticas de desenvolvimento de APIs REST.

## Funcionalidades

- Registro de entradas e saídas de funcionários com data e hora.
- Consulta de histórico de registros por funcionário.
- Geração de relatórios de horas trabalhadas.
- Endpoints REST com validações de entrada.
- Persistência de dados com JPA e banco H2.

## Tecnologias Utilizadas

- **Java**: Linguagem principal.
- **Spring Boot**: Framework para APIs REST.
- **JPA/Hibernate**: Persistência com banco H2.
- **Postman**: Testes de endpoints.
- **Git**: Versionamento.
- **Maven**: Gerenciamento de dependências.

## Pré-requisitos

- Java 17 ou superior
- Maven 3.8+
- Postman (para testes)
- Git

## Instalação e Execução

1. Clone o repositório:
   ```bash
   git clone https://github.com/bcstaslva/controle-ponto.git
   ```
2. Navegue até o diretório do projeto:
   ```bash
   cd controle-ponto
   ```
3. Compile e execute com Maven:
   ```bash
   mvn spring-boot:run
   ```
4. Acesse a API em `http://localhost:8080`.
5. Use a coleção do Postman em `/docs/postman-collection.json` para testar.

## Endpoints Principais

- `POST /registros`: Registra entrada/saída de funcionário.
- `GET /registros/funcionario/{id}`: Consulta histórico de registros.
- `GET /relatorios/funcionario/{id}`: Gera relatório de horas.
- `POST /funcionarios`: Cria novo funcionário.

## Como Contribuir

1. Faça um fork do repositório.
2. Crie uma branch (`git checkout -b feature/nova-funcionalidade`).
3. Commit suas alterações (`git commit -m 'Adiciona nova funcionalidade'`).
4. Push para a branch (`git push origin feature/nova-funcionalidade`).
5. Abra um Pull Request.

## Autor

Bruno Costa da Silva  
[GitHub](https://github.com/bcstaslva) | [E-mail](mailto:bcstaslva@gmail.com)
