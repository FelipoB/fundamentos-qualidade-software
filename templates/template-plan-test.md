# Template – Plano de Testes

Este modelo serve como base para criar planos de testes manuais ou automatizados em projetos de software. Ele cobre os principais elementos necessários para garantir rastreabilidade, clareza e alinhamento entre QA, time de desenvolvimento e stakeholders.

---

## 1. Identificação

**Plano de Teste:** Teste de Cadastro de Usuário  
**Projeto:** Sistema Web de Gestão  
**Autor:** Felipo Blanc  
**Data de Criação:** 28/06/2025  
**Versão:** 1.0

---

## 2. Objetivo

Descrever a abordagem e o escopo dos testes relacionados ao cadastro de usuário no sistema, garantindo que os critérios funcionais e não funcionais sejam validados antes da liberação para o ambiente de produção.

---

## 3. Escopo dos Testes

### Funcionalidades incluídas
- Cadastro de usuário pessoa física
- Validação de campos obrigatórios
- Validação de regras de senha
- Confirmação de e-mail

### Funcionalidades excluídas
- Recuperação de senha
- Cadastro de usuário pessoa jurídica

---

## 4. Tipos de Teste

- Teste Funcional Manual  
- Teste de Regressão  
- Teste de Integração  
- Teste de Interface (UI)  
- Teste de API (com Postman)

---

## 5. Estratégia de Teste

Os testes serão divididos em dois ciclos principais:

- Ciclo 1: Teste funcional com cobertura de 100% dos casos críticos
- Ciclo 2: Regressão e reteste de defeitos encontrados no ciclo 1

Ambiente de homologação será utilizado para execução dos testes manuais e de API.

---

## 6. Critérios de Entrada

- Funcionalidade implementada e integrada
- Ambiente de homologação disponível
- Plano de testes revisado e aprovado
- Dados de teste disponíveis

---

## 7. Critérios de Saída

- Todos os testes críticos com status "Aprovado"
- Nenhum defeito bloqueante ou crítico pendente
- Documentação de evidência publicada
- Checklist de release preenchido

---

## 8. Critérios de Aceitação

- Funcionalidades funcionam conforme regras de negócio
- Respostas da API seguem o contrato Swagger
- Campos obrigatórios validados com mensagens corretas
- Design e UI compatíveis com protótipos aprovados

---

## 9. Dados de Teste

- Usuário válido com CPF
- E-mails em diferentes domínios
- Senhas válidas e inválidas
- Usuário já cadastrado (para teste de duplicidade)

---

## 10. Ferramentas Utilizadas

- Postman  
- Cypress  
- DBeaver  
- GitHub Actions  
- Jira (para bugs e rastreio)

---

## 11. Ambiente de Teste

| Ambiente   | URL                                  |
|------------|---------------------------------------|
| Homologação | https://app-hmg.exemplo.com          |
| Banco de Dados | PostgreSQL 15                     |
| Navegadores | Chrome, Firefox, Edge               |
| Dispositivos | Desktop e Android 13 (mobile)       |

---

## 12. Riscos e Dependências

- Atrasos na entrega da funcionalidade pelo time de desenvolvimento
- Dependência de integração com serviço externo de e-mail
- Dados de teste inconsistentes entre builds

---

## 13. Cronograma

| Atividade              | Responsável     | Data       |
|------------------------|------------------|------------|
| Elaboração do plano    | QA               | 28/06/2025 |
| Execução ciclo 1       | QA + Dev         | 01/07/2025 |
| Execução ciclo 2       | QA               | 03/07/2025 |
| Encerramento e entrega | QA + PO          | 05/07/2025 |

---

## 14. Anexos

- Casos de teste (arquivo: `CT-cadastro-usuario.md`)  
- Evidências de execução  
- Relatórios de cobertura

---

# Modelos de Plano de Testes

## a) Tradicional (Waterfall)
Utiliza o modelo completo com escopo, plano de execução e rastreabilidade formal. Ideal para projetos com requisitos bem definidos desde o início.

## b) Ágil
Plano simplificado, iterativo, com foco em testes por sprint. Muitas vezes integrado no board (Jira, Trello) e baseado em critérios de aceitação.

## c) Automatizado
Foco em estratégias de scripts, ferramentas, CI/CD, cobertura e tipos de testes automatizados (API, UI, regressão).

## d) Exploratório
Plano informal baseado em sessões exploratórias, com objetivo, duração, notas rápidas e descobertas. Usado em sessões de investigação.

---

# Como usar

1. Copie este modelo para o repositório `/docs/test-plans/`
2. Renomeie com o nome da funcionalidade ou módulo testado
3. Preencha as seções conforme o contexto do projeto
4. Compartilhe o link com o time no canal de QA

