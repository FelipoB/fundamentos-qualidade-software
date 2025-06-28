#  Templates de Casos de Teste

Este diretório reúne diferentes modelos de **casos de teste** para serem usados conforme o tipo de teste, estratégia de QA e maturidade do time/projeto.

---

##  1. Template Padrão de QA Manual

Usado para testes funcionais manuais, regressão simples e testes exploratórios documentados.

### Estrutura recomendada

- **ID e Título**
- **Objetivo**
- **Referências**
- **Pré-condições**
- **Passos de Execução**
- **Dados de Teste**
- **Resultado Esperado**
- **Resultado Obtido**
- **Status**
- **Correções Realizadas**
- **Pós-condições**

Arquivo sugerido:  
`templates/template-test-case.md`

---

##  2. Template BDD (Behavior Driven Development)

Usado com frameworks como Cucumber, Behave ou SpecFlow. Ideal para times que trabalham com Product Owner e Devs usando critérios de aceitação colaborativos.

### Exemplo Gherkin

Feature: Cadastro de usuário

- **Scenario: Cadastro com dados válidos**
- Given que estou na tela de cadastro
- When eu preencho os campos obrigatórios
- And clico em "Cadastrar"
- Then vejo a mensagem "Cadastro realizado com sucesso"

Arquivo sugerido:  
`templates/template-bdd.md`

---

##  3. Template para Testes Automatizados

Usado para documentar os testes automatizados escritos em código.

### Estrutura recomendada

- **Nome do Teste Automatizado**
- **Framework/Ferramenta**
- **Pré-condições**
- **Tags/Identificadores**
- **Caminho no repositório**
- **Resultado Esperado**
- **Resultado Obtido**
- **Status no Pipeline**
- **Link para relatório ou evidência**

Arquivo sugerido:  
`templates/template-automated-test.md`

---

##  4. Template para Regressão

Usado em suítes de regressão executadas periodicamente.

### Estrutura recomendada

- **ID e Título**
- **Funcionalidade**
- **Criticidade (Alta/Média/Baixa)**
- **Frequência de Execução**
- **Passos de Teste**
- **Resultado Esperado**
- **Data da Última Execução**
- **Responsável**
- **Observações**

Arquivo sugerido:  
`templates/template-regression-suite.md`

---

##  5. Template para Teste de API

Usado com Postman, Swagger, Insomnia ou testes automatizados de API via script.

### Estrutura recomendada

- **Nome do Teste**
- **Endpoint (URL)**
- **Método HTTP (GET, POST, etc.)**
- **Headers**
- **Autenticação**
- **Payload de Entrada**
- **Códigos de Resposta Esperados**
- **Validações no Corpo da Resposta**
- **Resultado Esperado**
- **Resultado Obtido**
- **Ferramenta Utilizada**

Arquivo sugerido:  
`templates/template-api-test.md`

---

##  6. Template para Smoke Test

Usado para validar rapidamente se os fluxos principais da aplicação estão "vivos" após uma nova build.

### Estrutura recomendada

- **ID**
- **Funcionalidade**
- **Ação Básica**
- **Resultado Esperado**
- **Resultado Obtido**
- **Status**
- **Observações**

Arquivo sugerido:  
`templates/template-smoke-test.md`

---

##  7. Template para Testes de Performance

Usado com JMeter, k6, Gatling, Locust e ferramentas similares.

### Estrutura recomendada

- **Cenário Testado**
- **Ferramenta Utilizada**
- **Usuários Virtuais**
- **Tempo de Execução**
- **TPS Esperado**
- **Tempo Médio de Resposta**
- **Percentual de Erros Tolerado**
- **Gráficos ou Logs**
- **Resultado Obtido**
- **Conclusão**

Arquivo sugerido:  
`templates/template-performance-test.md`

---

##  Sugestão de Estrutura de Pastas

templates/
├── template-test-case.md
├── template-bdd.md
├── template-automated-test.md
├── template-api-test.md
├── template-smoke-test.md
├── template-regression-suite.md
└── template-performance-test.md

---

##  Dicas

- Todos os templates podem ser adaptados ao seu fluxo.
- Use o mesmo padrão de nome para facilitar leitura: `CT-XX`, `API-XX`, `AUTO-XX`.
- Para evidências, crie subpastas como `evidencias/CT-01/`.

---
