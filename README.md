# Testes de API na linguagem GO
Os testes são fundamentais para garantir a qualidade e confiabilidade do código. Neste projeto, testes unitários foram implementados cobrindo os casos críticos.

⚙️ Tecnologias utilizadas
Framework de testes

Jest - Framework de testes em JavaScript
Assertions

Chai - Biblioteca de assertions
Testes de integração

SuperTest - Testes de API REST
Cobertura de testes

nyc - Gera reports de cobertura
✅ Testes implementados
Testes unitários
src/tests/unit/Calculator.spec.js - Testes unitários da classe Calculator
src/tests/unit/ShoppingCart.spec.js - Testes unitários da classe ShoppingCart
Testes de integração
src/tests/integration/auth.int.spec.js - Fluxo de autenticação
src/tests/integration/products.int.spec.js - Endpoints de produtos
Cobertura de testes
A cobertura de testes é monitorada pelo nyc e relatórios são gerados a cada execução dos testes.

O objetivo é manter a cobertura de testes unitários e integração acima de 90%.

🚀 Executando os testes
# Testes unitários 
npm run test:unit

# Testes de integração
npm run test:int

# Todos os testes
npm test



O comando npm test executa tanto os testes unitários quanto os de integração, gerando um relatório de cobertura.

Os testes são executados em pipeline de CI a cada push e pull request.

📈 Cobertura de testes
A cobertura atual dos testes unitários é:

O relatório de cobertura detalhado pode ser conferido em coverage/index.html.

✅ Status do teste de integração contínua
O status do teste de integração contínua pode ser conferido na aba Actions do repositório.
🐞 Reportando issues
Encontrou um bug nos testes? Por favor abra uma issue descrevendo:

Onde ocorre o bug (em qual arquivo de teste)
Comportamento esperado
Comportamento atual
Exemplo:

Arquivo: src/tests/unit/Calculator.spec.js

Comportamento esperado:
- Chamada de somar(1, 2) deve retornar 3

Comportamento atual:
- Chamada está retornando 5



✨ Contribuindo
Contribuições são bem-vindas! Por favor siga estas etapas:

Faça um fork deste repositório
Crie uma branch com sua feature (git checkout -b feature/MinhaFeature)
Faça commit das suas alterações (git commit -m 'Adicionando MinhaFeature')
Faça push para a branch (git push origin feature/MinhaFeature)
Abra um Pull Request
📝 Licença
Este projeto está sob a licença MIT. Consulte o arquivo LICENSE para mais detalhes.

🧪 TDD
Este projeto segue a abordagem de TDD (Test Driven Development). Os testes são desenvolvidos antes da implementação.

Isso garante que:

A cobertura de testes seja alta desde o início
O design da aplicação seja orientado a testabilidade (SOLID)
Regressões sejam evitadas
⚡️ Próximos passos
Funcionalidades previstas:

Aumentar a cobertura de testes unitários para 95%
Adicionar testes E2E com Cypress
Configurar teste de mutação com Stryker
Adicionar teste de performance com k6
Implementar teste A/B
Sinta-se à vontade para contribuir com alguma dessas funcionalidades!