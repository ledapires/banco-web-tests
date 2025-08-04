# Banco Web Tests

Este projeto contém testes automatizados para uma aplicação bancária utilizando Cypress e JavaScript.

## Objetivo
O objetivo deste repositório é apresentar, de forma prática, como estruturar, organizar e executar testes automatizados de ponta a ponta (E2E) em aplicações web, utilizando o Cypress. O projeto cobre desde a configuração inicial até a geração de relatórios, incluindo a criação de comandos customizados para facilitar a manutenção e reutilização de código.

## Estrutura do Projeto
- **cypress/e2e/**: Testes end-to-end (login, transferência, etc.)
- **cypress/fixtures/**: Dados de teste (ex: credenciais)
- **cypress/support/**: Comandos customizados e configurações
- **cypress/reports/**: Relatórios de execução dos testes
- **cypress/screenshots/**: Capturas de tela dos testes
- **cypress.config.js**: Configuração do Cypress
- **package.json**: Dependências e scripts do projeto

## Pré-requisitos
- Node.js instalado
- npm instalado
- A API [banco-api](https://github.com/juliodelimas/banco-api) em execução
- A aplicação wem [banco-web](https://github.com/juliodelimas/banco-web) em execução

## Instalação
1. Clone o repositório:
   ```bash
   git clone https://github.com/ledapires/banco-api-tests
   ```
2. Instale as dependências:
   ```bash
   npm install
   ```

## Executando os Testes
- Para rodar os testes em modo headless:
  ```bash
  npx cypress run
  ```
- Para abrir o Cypress em modo interativo:
  ```bash
  npx cypress open
  ```

## Relatórios
Os relatórios em HTML são gerados em `cypress/reports/html/index.html` após a execução dos testes.

## Estrutura dos Testes
- Testes de login: Verificam autenticação com dados válidos e inválidos.
- Testes de transferência: Validam operações de transferência bancária.

## Personalização
- Adicione novos testes em `cypress/e2e/`
- Adicione dados de teste em `cypress/fixtures/`
- Comandos customizados podem ser criados em `cypress/support/commands/`

## Suporte
Para dúvidas ou sugestões, abra uma issue neste repositório.
