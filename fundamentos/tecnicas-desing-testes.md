# Técnicas de Design de Teste

## Descrição

Este documento apresenta as principais técnicas para a criação de casos de teste eficazes. As técnicas são divididas em três grandes grupos: baseadas em especificação (caixa preta), baseadas em estrutura (caixa branca) e baseadas em experiência. Cada técnica é explicada com exemplos práticos e sua relação com os pilares do QA: criatividade, pensamento analítico e comunicação clara.

---

## 1. Técnicas Baseadas em Especificação (Caixa Preta)

Estas técnicas focam nos requisitos e especificações do sistema, sem considerar a estrutura interna do código.

### 1.1 Partição de Equivalência

- Consiste em dividir o domínio de entrada em classes de dados equivalentes que devem ser tratados da mesma forma pelo sistema.
- Exemplo: Para um campo idade, classes podem ser: valores abaixo de 18, entre 18 e 65, acima de 65.
- Objetivo: Reduzir o número de casos de teste mantendo cobertura efetiva.

### 1.2 Análise de Valor Limite

- Baseia-se na ideia de que erros ocorrem mais frequentemente nos limites dos valores de entrada.
- Testa valores no limite inferior, superior e logo fora desses limites.
- Exemplo: Se a idade válida é entre 18 e 65, testar 17, 18, 65 e 66.
- Objetivo: Detectar erros relacionados a limites e condições extremas.

### 1.3 Tabela de Decisão

- Usa tabelas para representar combinações de condições de entrada e suas ações correspondentes.
- Exemplo: Regras para aprovação de crédito baseadas em renda, idade e histórico.
- Objetivo: Garantir cobertura de combinações lógicas complexas.

### 1.4 Casos de Uso

- Baseia-se em fluxos típicos de usuários para criar testes que reflitam o comportamento real.
- Exemplo: Fluxo de compra em um e-commerce.
- Objetivo: Validar cenários reais e garantir que funcionalidades atendam às expectativas do usuário.

---

## 2. Técnicas Baseadas em Estrutura (Caixa Branca)

Estas técnicas consideram o funcionamento interno do sistema, o código-fonte e a lógica.

### 2.1 Cobertura de Declaração

- Garante que cada linha ou declaração do código seja executada pelo menos uma vez.
- Objetivo: Detectar código que nunca é executado.

### 2.2 Cobertura de Decisão

- Garante que todas as decisões (ex: if/else) tenham suas ramificações testadas.
- Objetivo: Validar todos os caminhos lógicos.

### 2.3 Caminho Básico

- Testa todos os caminhos possíveis entre decisões dentro de uma função ou módulo.
- Objetivo: Garantir que nenhuma lógica esteja sem verificação.

---

## 3. Técnicas Baseadas em Experiência

Estas técnicas se apoiam no conhecimento, intuição e criatividade do testador.

### 3.1 Teste Exploratório

- O testador explora o sistema de forma livre, sem roteiros rígidos, buscando encontrar falhas inesperadas.
- Pilar: Criatividade em ação.
- Ideal para encontrar bugs em áreas novas ou pouco documentadas.

### 3.2 Teste Ad Hoc

- Testes informais, sem planejamento formal.
- Usados para rápidas verificações e experimentações.

### 3.3 Checklist de Testes

- Listas simples de verificações a serem feitas.
- Garantem que pontos importantes não sejam esquecidos.
- Pilar: Comunicação clara — facilita compartilhamento com o time.

---

## 4. Relação com os Pilares do QA

| Técnica                   | Criatividade | Pensamento Analítico | Comunicação Clara |
|---------------------------|--------------|----------------------|-------------------|
| Partição de Equivalência  |              | Sim                  |                   |
| Análise de Valor Limite   |              | Sim                  |                   |
| Tabela de Decisão         |              | Sim                  |                   |
| Casos de Uso              |              |                      | Sim               |
| Cobertura de Declaração   |              | Sim                  |                   |
| Cobertura de Decisão      |              | Sim                  |                   |
| Caminho Básico            |              | Sim                  |                   |
| Teste Exploratório        | Sim          |                      |                   |
| Teste Ad Hoc              | Sim          |                      |                   |
| Checklist de Testes       |              |                      | Sim               |

---

## 5. Considerações Finais

A combinação das técnicas apresentadas oferece uma base sólida para a criação de casos de teste completos e eficientes. Saber quando aplicar cada técnica, alinhado aos pilares do QA, permite que o testador seja mais eficaz, criativo e claro em sua comunicação.
