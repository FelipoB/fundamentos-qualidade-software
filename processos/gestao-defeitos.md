# Gestão de Defeitos (Bug Tracking)

## Descrição

Este documento apresenta o ciclo completo de vida de um defeito (bug), boas práticas para sua gestão e a importância da comunicação eficaz entre QA, desenvolvedores e stakeholders. Um processo bem definido de gestão de defeitos melhora a eficiência da equipe e garante a qualidade contínua do produto.

---

## 1. O que é um Defeito?

Um **defeito** (ou bug) é qualquer desvio entre o comportamento esperado e o comportamento real de um sistema, identificado durante os testes, uso real ou revisão de código.

---

## 2. Ciclo de Vida de um Defeito

O ciclo de vida de um defeito descreve as etapas pelas quais ele passa, desde sua identificação até sua resolução final.

### Fases mais comuns

| Etapa           | Descrição                                                              |
|-----------------|------------------------------------------------------------------------|
| Novo            | O defeito foi registrado e está aguardando triagem.                   |
| Em triagem      | Avaliação inicial para determinar severidade, prioridade e validade.  |
| Aberto          | O bug foi aceito e será tratado pelo time de desenvolvimento.         |
| Em progresso    | A correção está sendo desenvolvida.                                   |
| Corrigido       | O defeito foi corrigido e está pronto para ser validado.              |
| Em reteste      | O QA está testando novamente para confirmar a correção.               |
| Fechado         | O defeito foi validado como resolvido.                                |
| Reaberto        | O problema voltou ou não foi corrigido corretamente.                  |
| Rejeitado       | O defeito foi considerado inválido ou fora de escopo.                 |

---

## 3. Severidade vs. Prioridade

| Conceito    | Definição                                                                 | Exemplo                                  |
|-------------|---------------------------------------------------------------------------|------------------------------------------|
| Severidade  | Impacto técnico no sistema. Reflete a gravidade do defeito.               | Um erro que impede o login é alta severidade. |
| Prioridade  | Urgência para correção. Define quando o defeito deve ser tratado.         | Um erro visual em produção pode ter alta prioridade. |

**Importante:** Um defeito pode ter alta severidade e baixa prioridade — e vice-versa.

---

## 4. Boas Práticas na Abertura de Defeitos

Um bom relato de defeito deve conter:

- Título claro e objetivo
- Descrição completa do problema
- Passos para reproduzir
- Comportamento esperado vs. comportamento atual
- Ambiente de teste (versão, navegador, sistema operacional)
- Evidências (prints, vídeos, logs)
- Histórico de tentativas ou ocorrências

### Exemplo de relato

**Título:** [Cadastro] Botão "Cadastrar" desabilitado mesmo com e-mail válido

**Descrição:**  
Ao preencher todos os campos do formulário de cadastro com dados válidos, o botão "Cadastrar" continua desabilitado.

**Passos para reproduzir:**

1. Acessar a página de cadastro  
2. Preencher todos os campos obrigatórios  
3. Informar um e-mail válido (ex: usuario@teste.com)  
4. Tentar clicar no botão "Cadastrar"

**Comportamento esperado:**  
Botão "Cadastrar" habilitado ao preencher todos os dados válidos.

**Comportamento atual:**  
Botão permanece desabilitado.

**Ambiente:**  
Versão 1.0.5 | Navegador Chrome 126 | Android 13

---

## 5. Ferramentas de Gestão de Defeitos

| Ferramenta       | Descrição                                 |
|------------------|--------------------------------------------|
| Jira             | Muito utilizada em times ágeis.            |
| GitHub Issues    | Ideal para projetos colaborativos.         |
| Trello           | Visual e leve, útil para times pequenos.   |
| Azure DevOps     | Com integração a pipelines e testes.       |
| TestRail / qTest | Integram testes e defeitos.                |

---

## 6. Pilares do QA Aplicados na Gestão de Defeitos

| Pilar               | Aplicação prática                                                  |
|---------------------|--------------------------------------------------------------------|
| Pensamento analítico| Analisar impacto, logs, rastrear causa raiz e sugerir soluções.   |
| Comunicação clara   | Relatar bugs de forma objetiva, detalhada e compreensível.        |
| Criatividade        | Explorar cenários fora do óbvio para encontrar falhas ocultas.     |

---

## 7. Métricas Importantes

- Número de defeitos por sprint ou release  
- Taxa de reabertura  
- Tempo médio de resolução de bugs  
- Defeitos por módulo ou funcionalidade  
- Porcentagem de bugs encontrados por tipo de teste  
- Bugs em produção vs. detectados em QA  

---

## 8. Considerações Finais

A gestão de defeitos vai além de apenas registrar bugs. É uma atividade estratégica que envolve clareza na comunicação, análise crítica do sistema e comprometimento com a melhoria contínua da qualidade do produto.

---

## 9. Referências

- [Atlassian – Bug Reports](https://www.atlassian.com/software/jira/features/bug-tracking)  
