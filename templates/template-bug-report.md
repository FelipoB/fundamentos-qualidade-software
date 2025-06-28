# IEEE 829 (Standard for Test Documentation)
Embora seja um padrão mais antigo, o IEEE 829 fornece uma base sólida para documentar defeitos e relatórios de teste. Elementos como ID, título, descrição, passos para reproduzir, resultado esperado, resultado obtido e ambiente são derivados diretamente desse padrão.

# Scrum e DevOps
No contexto ágil e de CI/CD, o template já prevê:

Rastreabilidade com casos de teste (CT-XX)

Link com pipeline (status, build)

Organização para evidência visual (screenshot, vídeo)

Registro de ciclo de vida do bug (Aberto → Corrigido → Encerrado)
 
 # Princípios de comunicação clara (um dos pilares do QA)
O modelo é direto, objetivo e evita ambiguidade, algo essencial para que Devs, POs e stakeholders consigam entender o defeito sem interpretações erradas. Isso também reduz o retrabalho.


# Template – Bug Report

Este é o modelo oficial para registro de defeitos identificados em ambientes de desenvolvimento, homologação ou produção.

---

## ID do Bug
BUG-001

## Título
Erro ao salvar formulário de cadastro com campos obrigatórios preenchidos

## Descrição
Ao tentar salvar o formulário de cadastro com todos os campos obrigatórios preenchidos, o sistema retorna um erro 500, impedindo o salvamento correto dos dados.

## Reproduzível?
- [x] Sim, sempre  
- [ ] Às vezes  
- [ ] Não consegui reproduzir

---

## Passos para Reproduzir

1. Acessar a página de cadastro: `https://staging.sistema.com.br/cadastro`
2. Preencher todos os campos obrigatórios:
   - Nome: João Teste
   - E-mail: joao+bug001@teste.com
   - Senha: `Teste@123`
3. Clicar no botão "Cadastrar"

---

## Evidências

- Screenshot:  
  `evidencias/bug-001/screenshot.png`

- Vídeo (opcional):  
  `evidencias/bug-001/video.mp4`

---

## Resultado Esperado
Usuário cadastrado com sucesso e redirecionado para a tela de boas-vindas.

## Resultado Obtido
Mensagem de erro: `HTTP 500 - Internal Server Error`

---

## Ambiente

| Item            | Valor                                  |
|-----------------|----------------------------------------|
| URL             | https://staging.sistema.com.br         |
| Ambiente        | Homologação                            |
| Navegador       | Google Chrome 124                      |
| Sistema Operacional | Windows 11                         |
| Data/Hora       | 28/06/2025 - 10:32                     |
| Versão do Build | 1.0.0-rc.05                            |

---

## Severidade
- [x] Alta (impede uso da funcionalidade principal)  
- [ ] Média (afeta funcionalidade secundária)  
- [ ] Baixa (erro estético ou sem impacto funcional)

## Prioridade
- [ ] Alta  
- [x] Média  
- [ ] Baixa

---

## Status do Bug
- [x] Aberto  
- [ ] Em Análise  
- [ ] Em Correção  
- [ ] Corrigido  
- [ ] Rejeitado  
- [ ] Retestado  
- [ ] Encerrado

---

## Teste Relacionado
CT-05 – Cadastro de novo usuário

---

## Responsável Técnico
`@usuario-dev`  
Time: Squad App

---

## Comentários Adicionais
- Este erro também ocorre no endpoint `/cadastro/empresa`
- Testado com dados válidos e inválidos — erro persiste
- Log de erro anexado na pasta `logs/bug-001/`

---
