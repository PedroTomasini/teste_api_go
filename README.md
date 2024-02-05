# API de Gerenciamento de Alunos

Este documento apresenta uma visão geral da API de Gerenciamento de Alunos, um sistema desenvolvido em Go que utiliza o framework Gin para roteamento e manipulação de requisições HTTP. A API possibilita a execução de operações CRUD (Criar, Ler, Atualizar, Deletar) em um banco de dados de alunos.

## Características

- **Criação de Registros:** Permite a adição de novos registros de alunos.
- **Leitura de Registros:** Possibilita a consulta de registros existentes.
- **Atualização de Registros:** Permite a modificação de informações de alunos.
- **Exclusão de Registros:** Facilita a remoção de registros de alunos.

## Tecnologias Utilizadas

- **Go (versão 1.13 ou superior)**
- **Gin Web Framework**
- **GORM (ORM para Go)**
- **PostgreSQL**

## Configuração do Banco de Dados

Para utilizar a API, siga as seguintes instruções para criar e configurar o banco de dados:

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
git clone https://github.com/seu-usuario/teste_api_go.git
```

## Documentação de Testes e CI

### Testes Automatizados

Os testes automatizados desempenham um papel crucial na garantia da qualidade do código e na identificação de problemas antes da implantação. O arquivo `main_test.go` contém os testes, que são estruturados para validar diferentes aspectos da API.

#### Estrutura dos Testes

- `TestVerificaStatusCodeDaSaudacaoComParametro`: Verifica o status `200 OK` e a mensagem correta na rota de saudação.
- `TestListaTodosOsAlunosHanlder`: Testa a rota de listagem de alunos, garantindo que retorne o status `200 OK`.
- `TestBucaAlunoPorCPFHandler`: Confirma o funcionamento correto da busca de aluno por CPF.
- `TestBuscaAlunoPorIDHandler`: Verifica se a busca de aluno por ID retorna o aluno correto e o status `200 OK`.
- `TestDeletaAlunoHandler`: Testa a rota de deleção de aluno, assegurando seu funcionamento adequado.
- `TestEditaUmAlunoHandler`: Verifica se a edição de um aluno é realizada corretamente.

#### Execução dos Testes

```bash
go test -v ./...
```

### Integração Contínua (CI)

O fluxo de trabalho de CI está definido no arquivo `.github/workflows/go.yml` e automatiza a execução de testes e verificações sempre que há um novo código enviado ao repositório.

#### Etapas do Fluxo de Trabalho de CI

1. Configuração do ambiente de execução.
2. Instalação das dependências.
3. Execução dos testes automatizados.
4. (Opcional) Outras verificações, como linting ou análise de código.

#### Gatilhos de Execução

O CI é configurado para ser executado nos seguintes eventos:

- Push para a branch principal (geralmente main ou master).
- Pull requests para a branch principal.

#### Resultados

Os resultados da execução do CI são exibidos no GitHub, na seção "Actions" do repositório. Em caso de falhas, é recomendável corrigir os problemas identificados antes de prosseguir com a fusão de código.

Para contribuições e melhorias nos testes ou na rotina de CI, consulte o arquivo CONTRIBUTING.md.

## Contribuindo

Para contribuir com o projeto:

1. Fork o repositório.
2. Crie um novo branch (git checkout -b feature/nova-funcionalidade).
3. Faça suas alterações.
4. Commit suas mudanças (git commit -am 'Adiciona nova funcionalidade').
5. Push para o branch (git push origin feature/nova-funcionalidade).
6. Crie um Pull Request.

Consulte CONTRIBUTING.md para diretrizes de contribuição detalhadas.

## Licença

Este projeto está licenciado sob a Licença MIT - veja o arquivo LICENSE para detalhes.

## Autores

Nome do Autor - PedroTomasini
