# API de Gerenciamento de Alunos

Esta API é um sistema de gerenciamento de alunos desenvolvido em Go, utilizando o framework Gin para roteamento e manipulação de requisições HTTP. O sistema permite realizar operações CRUD (Criar, Ler, Atualizar, Deletar) em um banco de dados de alunos.

## Características

- Criação de novos registros de alunos.
- Leitura de registros existentes.
- Atualização de registros de alunos.
- Exclusão de registros de alunos.

## Tecnologias

- Go (versão 1.13 ou superior)
- Gin Web Framework
- GORM (ORM para Go)
- PostgreSQL

## Configuração do Banco de Dados

Instruções para criar e configurar o banco de dados necessário para a API:

1. Instale e inicie o PostgreSQL.
2. Crie um novo banco de dados chamado `alunos_db`.
3. Execute os scripts SQL localizados em `scripts/sql` para criar as tabelas necessárias.

## Instalação

### Pré-requisitos

- Go instalado (1.13+)
- PostgreSQL instalado e em execução
- Conhecimento básico de Go e bancos de dados SQL

### Clonando o Repositório

```bash
git clone https://github.com/seu-usuario/teste_api_go.git```

Instalando Dependências
```go mod tidy```

Uso
Para iniciar a API, execute:
```go run main.go```

A API estará disponível em http://localhost:8080.

Testes
Os testes automatizados podem ser executados com o seguinte comando:
```go test ./... -v```

Testes Unitários
Descrição dos testes unitários e como eles são organizados no projeto.

Testes de Integração
Descrição dos testes de integração e como eles interagem com o banco de dados.

Integração Contínua (CI)
Descrição da rotina de CI configurada para o projeto, incluindo:

Plataforma de CI utilizada (GitHub Actions, Travis CI, etc.).
Etapas do pipeline de CI (build, test, deploy).
Como os resultados são reportados e visualizados.
Contribuindo
Para contribuir com o projeto, siga estas etapas:

Fork o repositório.
Crie um novo branch (git checkout -b feature/nova-funcionalidade).
Faça suas alterações.
Commit suas mudanças (git commit -am 'Adiciona nova funcionalidade').
Push para o branch (git push origin feature/nova-funcionalidade).
Crie um Pull Request.
Consulte CONTRIBUTING.md para diretrizes de contribuição detalhadas.

Licença
Este projeto está licenciado sob a Licença MIT - veja o arquivo LICENSE para detalhes.

Autores
Nome do Autor - PedroTomasini

