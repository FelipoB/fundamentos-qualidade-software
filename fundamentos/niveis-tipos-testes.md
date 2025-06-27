# Níveis e Tipos de Teste de Software

## Descrição

Este documento aborda os principais **níveis** e **tipos de teste** utilizados na garantia da qualidade de software. A proposta é apresentar os conceitos de forma objetiva e alinhada com os pilares do QA: criatividade, pensamento analítico e comunicação clara.

---

## 1. Níveis de Teste

Os níveis de teste representam diferentes momentos no ciclo de desenvolvimento em que os testes podem ser aplicados, cada um com objetivos específicos.

### 1.1 Teste Unitário

- **O que é:** Testa unidades individuais do código, geralmente funções ou métodos.
- **Responsável:** Desenvolvedores.
- **Objetivo:** Garantir que cada unidade funcione isoladamente como esperado.
- **Pilar associado:** Pensamento analítico.

### 1.2 Teste de Integração

- **O que é:** Testa a comunicação entre módulos ou componentes do sistema.
- **Responsável:** Desenvolvedores ou QAs, dependendo da estratégia.
- **Objetivo:** Identificar falhas na troca de dados entre partes do sistema.
- **Pilar associado:** Pensamento analítico.

### 1.3 Teste de Sistema

- **O que é:** Valida o comportamento do sistema como um todo, com base nos requisitos.
- **Responsável:** QA.
- **Objetivo:** Verificar se o sistema atende às funcionalidades esperadas.
- **Pilar associado:** Comunicação clara.

### 1.4 Teste de Aceitação

- **O que é:** Confirma se o sistema atende às expectativas do cliente ou usuário final.
- **Responsável:** Cliente, PO ou QA com foco em negócio.
- **Objetivo:** Validar que a entrega tem valor e está pronta para produção.
- **Pilar associado:** Comunicação clara.

---

## 2. Tipos de Teste

Os tipos de teste classificam os testes conforme sua **natureza ou objetivo específico**. Um único nível de teste pode abranger vários tipos simultaneamente.

### 2.1 Teste Funcional

- **Foco:** Comportamento do sistema em relação aos requisitos.
- **Exemplos:** Login, cálculo de frete, cadastro de usuário.

### 2.2 Teste Não Funcional

- **Foco:** Qualidade interna do sistema, como desempenho, segurança e usabilidade.
- **Exemplos:** Teste de carga, stress, acessibilidade, compatibilidade.

### 2.3 Teste de Regressão

- **Foco:** Verificar se uma nova alteração afetou funcionalidades que antes estavam corretas.
- **Quando usar:** Após correções de bugs ou novas entregas.
- **Pilar associado:** Pensamento analítico.

### 2.4 Teste de Exploração

- **Foco:** Descobrir problemas sem seguir scripts definidos.
- **Como aplicar:** Com liberdade, criatividade e curiosidade.
- **Pilar associado:** Criatividade.

### 2.5 Teste de Usabilidade

- **Foco:** Avaliar a facilidade de uso, acessibilidade e experiência do usuário.
- **Exemplos:** Fluxos claros, mensagens compreensíveis.
- **Pilar associado:** Comunicação clara.

### 2.6 Teste de Segurança

- **Foco:** Verificar vulnerabilidades, permissões e proteção contra acessos indevidos.
- **Importância:** Crítico para sistemas com dados sensíveis.
- **Pilar associado:** Pensamento analítico.

---

## 3. Relação com os Pilares do QA

| Tipo ou Nível de Teste | Criatividade | Pensamento Analítico | Comunicação Clara |
|------------------------|--------------|----------------------|--------------------|
| Teste Unitário         |              | Sim                  |                    |
| Teste de Integração    |              | Sim                  |                    |
| Teste de Sistema       |              | Sim                  | Sim                |
| Teste de Aceitação     |              |                      | Sim                |
| Teste de Regressão     |              | Sim                  |                    |
| Teste Exploratório     | Sim          | Sim                  |                    |
| Teste de Usabilidade   |              |                      | Sim                |

---

## 4. Considerações Finais

Entender os níveis e tipos de teste é essencial para aplicar uma **estratégia de qualidade eficaz**. Saber quando, como e por que testar permite priorizar riscos, economizar tempo e entregar valor de forma contínua.

Ao dominar esses conceitos e relacioná-los com os pilares da atuação de um QA, você fortalece sua capacidade de analisar sistemas, comunicar com clareza e propor testes que vão além do básico.

---

## 5. Referências e Links Úteis

- ISTQB Glossary:  
  https://glossary.istqb.org/en_US/search

