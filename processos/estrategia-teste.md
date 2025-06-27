# Estratégia de Teste

## Descrição

A estratégia de teste é um documento essencial que define a abordagem, escopo, recursos e cronograma das atividades de teste de software. Ela serve como guia para garantir que os testes sejam realizados de forma eficiente, cobrindo os riscos mais relevantes e assegurando a qualidade do produto entregue.

---

## 1. Objetivos da Estratégia

- Garantir que os requisitos funcionais e não funcionais sejam validados.
- Identificar e mitigar riscos relacionados à qualidade.
- Proporcionar visibilidade sobre o progresso e cobertura dos testes.
- Estabelecer padrões de qualidade e critérios de aceitação.
- Facilitar a comunicação entre os membros do time de desenvolvimento e QA.

---

## 2. Escopo da Estratégia

A estratégia de teste define:

- As funcionalidades que serão testadas.
- As que não serão testadas (fora do escopo).
- Os níveis de teste aplicados (unitário, integração, sistema, aceitação).
- As responsabilidades dos envolvidos no processo.

---

## 3. Abordagens de Teste

- **Baseado em requisitos**: os testes são derivados a partir das histórias de usuário, critérios de aceite e documentação técnica.
- **Baseado em risco**: priorização dos testes conforme a probabilidade e o impacto de falhas.
- **Exploratório**: testes executados com base na experiência e intuição do testador.
- **Automatizado**: criação de scripts para execução recorrente dos testes.
- **Manual**: execução controlada de testes com intervenção humana.
- **Comportamental (BDD)**: uso de linguagem natural para descrever o comportamento esperado.

---

## 4. Tipos e Níveis de Teste

- **Testes funcionais**
  - Unitário
  - Integração
  - Sistema
  - Aceitação
- **Testes não funcionais**
  - Performance
  - Segurança
  - Usabilidade
  - Compatibilidade
- **Testes de regressão**
- **Testes exploratórios**
- **Testes de fumaça (Smoke Tests)**

---

## 5. Critérios de Entrada e Saída

### Critérios de Entrada

- Funcionalidade implementada e entregue para QA
- Ambientes de teste disponíveis e estáveis
- Dados de teste preparados
- Requisitos documentados e compreendidos

### Critérios de Saída

- Todos os testes planejados executados
- Defeitos críticos e bloqueantes resolvidos
- Relatórios de testes publicados
- Critérios de aceite atendidos

---

## 6. Ambientes e Dados de Teste

- Ambiente de homologação (staging) configurado
- Scripts de carga de dados
- Dados sensíveis anonimizados
- Separação clara entre ambientes de desenvolvimento, homologação e produção

---

## 7. Ferramentas de Apoio

| Categoria              | Ferramentas                                |
|------------------------|--------------------------------------------|
| Automação frontend     | Cypress, Playwright, Selenium              |
| Testes de API          | Postman, Rest Assured, Karate              |
| Testes de performance  | JMeter, k6                                 |
| CI/CD                  | GitHub Actions, Jenkins                    |
| Gerenciamento de testes| TestRail, Zephyr, Xray                     |
| Versionamento          | Git, GitHub, Bitbucket                     |

---

## 8. Métricas de Qualidade

- Cobertura de testes (automatizados e manuais)
- Defeitos encontrados por tipo/teste
- Tempo médio de resolução de bugs
- Percentual de testes com sucesso por build
- Taxa de falhas em produção
- Rácio de reabertura de defeitos

---

## 9. Comunicação e Relatórios

A estratégia de teste prevê o uso de relatórios objetivos e periódicos que devem incluir:

- Status dos testes (executados, falhados, bloqueados)
- Tabela de bugs por severidade
- Tabela de cobertura por tipo de teste
- Indicadores de performance dos testes automatizados

---

## 10. Riscos e Mitigações

| Risco potencial                       | Ação de mitigação                                   |
|--------------------------------------|-----------------------------------------------------|
| Ambiente de testes instável          | Automatizar verificações e ter backups configurados |
| Falta de dados de teste              | Criar massa com geradores ou bancos fictícios       |
| Requisitos mal definidos             | Realizar refinamentos com time de produto           |
| Alto volume de mudanças              | Automatizar testes de regressão                     |

---

## 11. Pilares do QA aplicados

| Pilar               | Aplicação prática                                                   |
|---------------------|---------------------------------------------------------------------|
| Criatividade        | Exploração de cenários alternativos e testes fora do esperado       |
| Pensamento analítico| Definição de prioridades, análise de cobertura e impacto de falhas  |
| Comunicação clara   | Relatórios claros, documentação acessível e triagens bem descritas  |

---

## 12. Exemplo de Estratégia Aplicada

**Projeto:** Plataforma de agendamento médico online  
**Escopo:**  
- Validação do fluxo completo de agendamento  
- Testes de compatibilidade em navegadores  
- Testes de API entre front e back-end  
- Performance sob alta carga

**Abordagem:**  
- Testes manuais exploratórios nas primeiras sprints  
- Criação de suíte automatizada com Cypress  
- Testes de regressão a cada entrega  
- Postman + Newman para APIs REST

**Ferramentas:** GitHub, GitHub Actions, Cypress, Postman, PostgreSQL, Confluence

**Critérios de saída:**  
- 100% dos testes críticos executados  
- Zero defeitos críticos em aberto  
- Execução automatizada na pipeline

---

